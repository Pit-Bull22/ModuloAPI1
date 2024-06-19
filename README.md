# ModuloAPI1

[![.NET](https://img.shields.io/badge/.NET-8.0-blue)](https://dotnet.microsoft.com/)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-2019-CC2927)](https://www.microsoft.com/pt-br/sql-server/sql-server-2019)
[![Entity Framework](https://img.shields.io/badge/Entity%20Framework-6.0-5C2D91)](https://docs.microsoft.com/en-us/ef/core/)

## Descrição

**ModuloAPI1** é uma API desenvolvida em .NET 8.0 com um CRUD básico para gerenciar contatos. A API utiliza o Entity Framework para integração com um banco de dados SQL Server. Cada contato possui um ID, Nome, Telefone e um status de Ativo.

## Requisitos 

- [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [SQL Server 2019](https://www.microsoft.com/pt-br/sql-server/sql-server-2019)

## Configuração do Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/ContatoAPI.git
   cd ContatoAPI

2. Configure a string de conexão no arquivo `appsettings.json`:
   
~~~~{
  "ConnectionStrings": {
    "DefaultConnection": "Server=SEU_SERVIDOR;Database=SeuBancoDeDados;User Id=SeuUsuario;Password=SuaSenha;"
  }
}
~~~~

3. Atualize o banco de dados para aplicar as migrações:

`dotnet ef database update` 

4. execute a aplicação: 

`dotnet run`


## Estrutura do Projeto

* Controllers/ContatoController.cs: Controlador com os endpoints da API.
* Models/Contato.cs: Modelo da entidade Contato.
* Data/ContatoContext.cs: Contexto do Entity Framework.
* Migrations/: Pasta contendo as migrações do Entity Framework.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

1. Fork o projeto
2. Crie sua feature branch (git checkout -b feature/nova-feature)
3. Commit suas mudanças (git commit -m 'Adiciona nova feature')
4. Push para a branch (git push origin feature/nova-feature)
5. Abra um Pull Request
