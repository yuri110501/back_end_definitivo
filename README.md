# Profiles REST API

Profiles REST API course code.

This is the full source code for our course on Udemy: [Build a Backend REST API with Python & Django - Beginner](https://londonapp.dev/c1).

# My Project

## Visão Geral

Este é um projeto Django com uma API RESTful para gerenciar produtos, pedidos e clientes. A API utiliza JSON Web Tokens (JWT) para autenticação e inclui documentação interativa através do Swagger.

## Estrutura do Projeto

- **myproject/**: Pasta principal do projeto.
  - **settings.py**: Configurações do Django.
  - **urls.py**: Rotas principais do projeto.
- **core/**: Pasta do aplicativo principal.
  - **models.py**: Modelos do banco de dados para `Product`, `Order` e `Client`.
  - **serializers.py**: Serializadores para os modelos.
  - **views.py**: Views para as operações CRUD.
  - **urls.py**: Rotas do aplicativo.
- **tests/**: Pasta de testes unitários para modelos e views.

## Pré-requisitos

- Python 3.7+
- Django 5.1.4
- Django REST Framework
- drf-yasg
- djangorestframework-simplejwt

## Instalação

Crie um ambiente virtual e ative-o:

sh
python -m venv venv
source venv/bin/activate
Instale as dependências:

Instale as dependências:
sh
pip install -r requirements.txt

Aplique as migrações do banco de dados:

sh
python manage.py makemigrations
python manage.py migrate


Crie um superusuário:

sh
python manage.py createsuperuser

Inicie o servidor de desenvolvimento:

sh
python manage.py runserver



Autenticação
Para obter o token JWT:

URL: http://127.0.0.1:8000/api/token/

Método: POST

Headers: Content-Type: application/json

Body (JSON):

json
{
  "username": "yourusername
  ",
  "password": "yourpassword"
}

