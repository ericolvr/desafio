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
Você pode encontrar um json com os registros à serem inseridos nesse endereço:<br>
[http://ec2-34-230-24-198.compute-1.amazonaws.com/records](http://ec2-3-87-113-128.compute-1.amazonaws.com/records)

Regra:<br>
Quando os campos (**age**, **type** e **action**) forem iguais, e o campo **date** for superior a **30 minutos** o registro deverá ser inserido.<br>
Caso o campo **date** for inferior a **30 minutos**, deve-se pegar o registro mais recente cujo os campos (**age**, **type** e **action**) são os mesmos e atualiza-lo.




