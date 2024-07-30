# Projeto de Exemplo: API com Entity Framework em C#

## Descrição

Este projeto é um exemplo de uma API em C# que utiliza a Entity Framework para operações CRUD (Create, Read, Update, Delete) em uma entidade de exemplo. Ele fornece endpoints para criar, ler, atualizar e excluir registros dessa entidade.

## Requisitos

Para executar este projeto em sua máquina, você precisará das seguintes ferramentas e tecnologias:

- Visual Studio (ou outra IDE compatível com C#)
- .NET Framework instalado
- SQL Server (ou outro banco de dados compatível com a Entity Framework)

## Instalação

Git Clone:
Primeiro, clone o repositório com o seguinte comando:
git clone https://github.com/Otavio17061992/CrudWithAPI

Abra o Projeto no Visual Studio:
Abra o Visual Studio e carregue o projeto que você acabou de clonar.
Configurações de Conexão com o Banco de Dados:
Verifique se as configurações de conexão com o banco de dados no arquivo appsettings.json estão corretas. Isso é importante para garantir que a API se comunique corretamente com o banco de dados.
Execute o Aplicativo:
Execute o aplicativo para iniciar a API. Você pode fazer isso usando o seguinte comando:
dotnet run

Uso
A API possui os seguintes endpoints:

GET /api/contato: Recupera todos os registros da entidade.
GET /api/contato/{id}: Recupera um registro específico pelo ID.
POST /api/contato: Cria um novo registro.
PUT /api/contato/{id}: Atualiza um registro existente pelo ID.
DELETE /api/contato/{id}: Exclui um registro pelo ID.
Exemplo de Requisições
Aqui estão alguns exemplos de como fazer chamadas de API usando o cURL:

GET Todos os Registros:
curl -X GET http://localhost:5000/api/contato

GET Um Registro por ID:
curl -X GET http://localhost:5000/api/contato/1

POST Novo Registro:
curl -X POST -H "Content-Type: application/json" -d '{"Nome": "valor1", "Telefone": "valor2", "Ativo": "valor3"}' http://localhost:5000/api/contato

PUT Atualizar Registro Existente:
curl -X PUT -H "Content-Type: application/json" -d '{"ID": "novo-valor"}' http://localhost:5000/api/contato

DELETE Registro por ID:
curl -X DELETE http://localhost:5000/api/id

Contribuições
Contribuições são bem-vindas! Se você encontrar algum problema ou tiver sugestões para melhorias, sinta-se à vontade para criar uma issue ou enviar um pull request.

Licença
Este projeto é licenciado sob a Licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.

Autor
[João Otávio] [joaodevelopercsharp@gmail.com]
csharp
Copy code
