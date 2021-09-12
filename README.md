# Criando um catálogo de jogos usando boas práticas de arquitetura com .NET
Cliente: Pode ser uma API, Angular, front-end, etc <br>
Middleware: São componentes de software que tratam request e response <br>
Controller: É o componente que recebe requests e produz responses <br>
Services: É responsável pela lógica de negócio, orquestra chamadas ao banco de dados ou até mesmo outros serviços <br>
Repository: É responsável pelo acesso ao banco de dados <br>
DTO: Data Transfer Object é a representação do dado trafegado, comumente é utilizado para representar o Json do request e response <br>
Entity: É a representação da tabela no banco de dados

## Requisitos
- IDE
- Conhecimento em C# e .NET

## Executar o projeto
1) No arquivo `API-CatalogoJogos.csproj` em `<DocumentationFile></DocumentationFile>` coloque o path do seu computador 
2) No arquivo `appsettings.json` em:
>"Default": "Data Source=MAKI\\MSSQLSERVER02;Initial Catalog=CatalogoJogos;Integrated Security=True" 

Substitua o path: `MAKI\\MSSQLSERVER02` pelo path do seu Microsoft SQL Server Management Studio
3) Execute o projeto no Visual Studio, o projeto abrirá em: <br>
>https://localhost:44314/swagger/index.html

## Dicas
- O `guid` é usado nos métodos HTTP para gerar um id aleatório
- O `await` retorna uma lista
- `IDisposable` destrói o objeto
- Com o Middleware criado é possível adicionar mensagens de alerta ou erro para o Swagger

## Banco de dados
No arquivo `appsettings.json` foi adicionado o código: `"Default": "Data Source=MAKI\\MSSQLSERVER02;Initial Catalog=CatalogoJogos;Integrated Security=True;Connect Timeout=30"` para executar na sua máquina, substitua o código `MAKI\\MSSQLSERVER02` pelo seu path do banco de dados

## Swagger
- Cliquei com o botão direito no projeto > Propriedades > Suppress Warnings > Adicionei `1591`

## Licença
Distribuido sob a licença MIT License. Veja `LICENSE` para mais informações.

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
