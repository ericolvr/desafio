# Objetivo

Criar uma aplicação para gerenciar uma lista de Pessoas ( person ).<br>
Utilize algúm framework Python de sua escolha. Essa aplicação deverá ser um CRUD e contemplar testes unitários.<br><br>

## Estrutura do Person ##
```
  {
    "id": 8,
    "age": "21",
    "type": "female",
    "action": "eat",
    "date": "2024-09-19T03:12:53.829184"
  }

```

## Endpoints e Verbos ##
**/persons** - **GET**<br>
Deverá exibir uma lista com todos os registros paginados<br><br>

**/persons/action** - **GET**<br>
Deverá exibir todos os registros usando o campo **action** como filtro, devem ser paginados

**/persons/** - **POST**<br>
Você pode encontrar um json com os registros ma serem inseridos nesse endreço:<br>
http://ksksksksksks

Existe uma regra:<br>
Quando os campos (**age**, **type** e **action**) forem iguais e o campo date for superior a 30 minutoso registro deverá ser inserido

Esse endpoint receberá os **alerts** enviados pela aplicação em anexo e deverá ser responsável pela inclusão no banco de dados. Nessa aplicação existem registros similares, mas que **diferem pelo horário**, campo **created**.<br>
Aqui temos uma regra:<br>
- campos (**type** e **equipment**) forem iguais a algum registro já existente, mas com o horário **superior** a **30 minutos** deve-se **atualizar(update)** esse registro existente.<br>

Do contrário inserir um novo registro.



