# Criando um catálogo de jogos usando boas práticas de arquitetura com .NET
Cliente: Pode ser uma API, Angular, front-end, etc
Middleware: São componentes de software que tratam request e response
Controller: É o componente que recebe requests e produz responses
Services: É responsável pela lógica de negócio, orquestra chamadas ao banco de dados ou até mesmo outros serviços
Repository: É responsável pelo acesso ao banco de dados
DTO: Data Transfer Object é a representação do dado trafegado, comumente é utilizado para representar o Json do request e response
Entity: É a representação da tabela no banco de dados

## Criar o projeto
- Visual Studio
- ASP.NET Core Web Application
- ASP.NET Core Web API
- Configurar o HTTPS
- Habilitar o OpenAPI

## Visual Studio - Adicionar recursos
### Criar Controller
Clique com o botão direito > Adicionar Controller > API Controller Empty 

## Conexão com o banco de dados
No arquivo `appsettings.json` na linha `10` a `12` foi adicionado o path do banco de dados para fazer a conexão com o arquivo `JogoSqlServerRepository.cs`
