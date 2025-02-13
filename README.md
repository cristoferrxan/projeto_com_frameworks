<<<<<<< HEAD
📦 Sistema de Banco de Dados para Gestão de Clientes e Produtos
Este projeto é um sistema de banco de dados desenvolvido em Python para gerenciar a entrada de clientes, cadastro de produtos, compras e preferências. Ele permite uma organização eficiente dos dados, incluindo:

✅ Cadastro e gerenciamento de clientes
✅ Registro de produtos com filtragem por tags
✅ Histórico de compras e preferências de clientes
✅ Sistema de consultas para facilitar a análise dos dados

O projeto utiliza SQLite/MySQL/PostgreSQL (especifique qual banco de dados foi usado) para armazenar os dados de forma estruturada, e bibliotecas como SQLAlchemy/Pandas/Django ORM (caso tenha usado alguma).

📌 Tecnologias utilizadas:

Python 🐍
Banco de Dados (SQLite/MySQL/PostgreSQL) 🗄️
(Adicione outras tecnologias, se necessário)
💡 Próximas implementações:

Melhorias na interface de consulta
Relatórios personalizados
Integração com API (se for o caso)
Sinta-se à vontade para contribuir ou dar sugestões! 🚀
=======
# API de Recomendação de Produtos

Este projeto é uma API criada com FastAPI para recomendação de produtos baseada no histórico de compras de usuários e preferências como categorias e tags.

## Funcionalidades

- **Criação de usuários**: Cadastro de novos usuários.
- **Cadastro de produtos**: Cadastro de produtos com nome, categoria e tags.
- **Histórico de compras**: Adicionar produtos ao histórico de compras de um usuário.
- **Recomendações de produtos**: Recomendação de produtos com base no histórico de compras e preferências do usuário.

## Tecnologias Utilizadas

- **Python 3.9+**
- **FastAPI**
- **Pydantic**
- **Uvicorn** (para rodar o servidor)
- **Pytest** (para testes automatizados)

## Instalação e Configuração

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/uranolais/boas-praticas-python-curso01.git
   cd recomendacao-produtos
   ```

2. **Crie um ambiente virtual:**
   ```bash
   python -m venv venv
   ```

3. **Ative o ambiente virtual:**
   - No Windows:
     ```bash
     venv\Scripts\activate
     ```
   - No macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Execute o servidor:**
   ```bash
   uvicorn app.main:app --reload
   ```

6. **Acesse a documentação interativa da API:**
   Abra o navegador e acesse `http://127.0.0.1:8000/docs` para visualizar e testar as rotas da API.

## Estrutura do Projeto

```bash
.
├── app
│   ├── main.py              # Arquivo principal que inicia o FastAPI
│   ├── models               # Modelos Pydantic usados pela API
│   │   ├── models_produtos.py
│   │   └── models_usuarios.py
│   ├── routers              # Arquivos contendo os roteadores de usuários e produtos
│   │   ├── routers_produtos.py
│   │   └── routers_usuarios.py
├── tests
│   └── test_api.py          # Testes para a API
├── venv                     # Ambiente virtual
├── README.md                # Instruções sobre o projeto
└── requirements.txt         # Dependências do projeto
```

## Exemplos de Uso

### Criar um usuário:

- **POST /usuarios/**
  ```json
  {
    "nome": "Usuário Teste"
  }
  ```

### Criar um produto:

- **POST /produtos/**
  ```json
  {
    "nome": "Produto Teste",
    "categoria": "Eletrônicos",
    "tags": ["tecnologia", "novo"]
  }
  ```

### Adicionar histórico de compras:

- **POST /historico_compras/{usuario_id}**
  ```json
  {
    "produtos_ids": [1, 2]
  }
  ```

### Recomendação de produtos:

- **POST /recomendacoes/{usuario_id}**
  ```json
  {
    "categorias": ["Eletrônicos"],
    "tags": ["novo"]
  }
  ```

## Rodar os Testes

Para rodar os testes unitários:

```bash
pytest tests/
```

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou relatar um problema.
>>>>>>> b14ae7a (projeto_com_frameworks)

