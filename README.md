# ModuloAPI1

[![.NET](https://img.shields.io/badge/.NET-8.0-blue)](https://dotnet.microsoft.com/)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-2019-CC2927)](https://www.microsoft.com/pt-br/sql-server/sql-server-2019)
[![Entity Framework](https://img.shields.io/badge/Entity%20Framework-7.0-5C2D91)](https://docs.microsoft.com/en-us/ef/core/)

# API de Contatos em .NET C#

Bem-vindo à API de Contatos! Este repositório contém um projeto de API desenvolvido em .NET C# com operações CRUD básicas. A API utiliza o Entity Framework para integração com um banco de dados SQL Server e a documentação da API é gerada com Swagger.

## Funcionalidades

- **CRUD de Contatos**: Criação, Leitura, Atualização e Exclusão de contatos.
- **Integração com SQL Server**: Utilização do Entity Framework para mapeamento objeto-relacional.
- **Documentação com Swagger**: Interface interativa para explorar e testar os endpoints da API.

## Estrutura da Classe Contato

A API possui uma classe `Contato` com os seguintes campos:

- `int Id`: Identificador único do contato.
- `string Nome`: Nome do contato.
- `string Telefone`: Número de telefone do contato.
- `bool Ativo`: Indica se o contato está ativo.

## Tecnologias Utilizadas

- .NET C#
- Entity Framework
- SQL Server
- Swagger

## Pré-requisitos

- .NET SDK
- SQL Server
- Visual Studio ou Visual Studio Code

## Configuração do Projeto

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/api-contatos-dotnet.git
    cd api-contatos-dotnet
    ```

2. Configure a string de conexão com o SQL Server no arquivo `appsettings.json`:
    ```json
    {
      "ConnectionStrings": {
        "DefaultConnection": "Server=seu_servidor;Database=sua_base_de_dados;User Id=seu_usuario;Password=sua_senha;"
      }
    }
    ```

3. Execute as migrações do Entity Framework para criar o banco de dados:
    ```bash
    dotnet ef database update
    ```

4. Inicie a aplicação:
    ```bash
    dotnet run
    ```

## Endpoints da API

### Criar um novo contato

- **POST** `/api/contatos`
    ```json
    {
      "nome": "João Silva",
      "telefone": "123456789",
      "ativo": true
    }
    ```

### Obter todos os contatos

- **GET** `/api/contatos`

### Obter um contato por ID

- **GET** `/api/contatos/{id}`

### Atualizar um contato

- **PUT** `/api/contatos/{id}`
    ```json
    {
      "id": 1,
      "nome": "João Silva",
      "telefone": "987654321",
      "ativo": true
    }
    ```

### Excluir um contato

- **DELETE** `/api/contatos/{id}`

## Documentação da API

Após iniciar a aplicação, você pode acessar a documentação interativa do Swagger em:

http://localhost:{porta}/swagger


## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.


---

Feito com ❤️ por Rafael Santos(https://github.com/Pit-Bull22)



