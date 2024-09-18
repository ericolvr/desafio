# Objetivo

Criar uma aplicação para gerenciar uma lista de Alertas ( alerts ).<br>
Utilize algúm framework Python de sua escolha. Essa aplicação deverá ser um CRUD e contemplar testes unitários.<br><br>

## Estrutura do Alert ##
```
{
    'type': 'critic',
    'created: 2024-08-08 00:00:00,
    'equipment': 3,
    'branch': 'Av. Paulista'
}

type = string
created = datetime
equipment = int
branch = string
```

## Endpoints e Verbos ##
**/alerts** - **GET**<br>
Deverá exibir uma lista com todos os registros paginados<br><br>

**/alerts/id** - **GET**<br>
Exibir um registro pelo campo **id**

**/alerts/branch** - **GET**<br>
Deverá exibir todos os registros usando o campo **branch** com filtro, devem ser paginados

**/alerts/** - **POST**<br>
Esse endpoint receberá os **alerts** enviados pela aplicação em anexo e deverá ser responsável pela inclusão no banco de dados. Nessa aplicação existem registros similares, mas que diferem pelo horário, campo **created**.<br><br>
Aqui temos uma regra:<br>
- campos (**type** e **equipment**) forem iguais a algum registro já existente, mas com o horário **superior** a **30 minutos** deve-se **atualizar(update)** esse registro existente.<br>

Do contrário inserir um novo registro.



