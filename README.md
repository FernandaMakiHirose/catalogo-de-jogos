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

## Sobre a Autora
Oi, eu sou a Fernanda! Estou aqui para contribuir com meu conhecimento e espero poder ajudar no desenvolvimento profissional de cada um de vocês.

[![Linkedin Badge](https://img.shields.io/badge/-Fernanda_Maki_Hirose-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)](https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)  [![Gmail Badge](https://img.shields.io/badge/-femahi2020@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:femahi2020@gmail.com)](mailto:femahi2020@gmail.com)
