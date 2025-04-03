# API de Autenticação

Este é um projeto de API de autenticação simples, utilizando Flask, SQLAlchemy e Flask-Migrate para gerenciamento do banco de dados.

## Tecnologias Utilizadas
- Python
- Flask
- Flask-SQLAlchemy
- Flask-Migrate
- SQLite
- Flask-CORS

## Como Instalar e Executar

1. Clone o repositório:
   ```sh
   git clone https://github.com/stonedyy/API-Auth.git
   cd API-Auth
   ```

2. Crie um ambiente virtual e ative:
   ```sh
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate  # Windows
   ```

3. Instale as dependências:
   ```sh
   pip install -r requirements.txt
   ```

4. Inicialize o banco de dados:
   ```sh
   flask db upgrade
   ```

5. Execute a aplicação:
   ```sh
   flask run
   ```

A API estará disponível em `http://127.0.0.1:5000/`

## Endpoints Disponíveis

### Cadastro de Usuário
- **URL:** `/register`
- **Método:** `POST`
- **Body:**
  ```json
  {
    "username": "seu_usuario",
    "password": "sua_senha"
  }
  ```
- **Resposta de Sucesso:**
  ```json
  {
    "message": "User registered successfully"
  }
  ```

### Login
- **URL:** `/login`
- **Método:** `POST`
- **Body:**
  ```json
  {
    "username": "seu_usuario",
    "password": "sua_senha"
  }
  ```
- **Resposta de Sucesso:**
  ```json
  {
    "message": "Login successful"
  }
  ```
- **Resposta de Erro:**
  ```json
  {
    "error": "Invalid username or password"
  }
  ```

## Como Contribuir

1. Faça um fork do repositório
2. Crie uma nova branch: `git checkout -b minha-feature`
3. Faça suas alterações e commit: `git commit -m 'Adicionando nova feature'`
4. Envie para o repositório remoto: `git push origin minha-feature`
5. Abra um Pull Request

---

Projeto desenvolvido para aprendizado de APIs com Flask. 🚀
