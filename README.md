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
Você pode encontrar um json com os registros ma serem inseridos nesse endereço:<br>
http://ksksksksksks

Existe uma regra:<br>
Quando os campos (**age**, **type** e **action**) forem iguais, e o campo **date** for superior a **30 minutos** o registro deverá ser inserido.<br>
Caso o campo date for inferior a 30 minutos, deve-se pegar o último registro com os campos e atualiza-lo.




