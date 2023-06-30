# Sistema-de-Gerenciamento-de-Tarefas-API
Para a API funcionar em seu computador você deve verificar se o mySql está iniciado e em seguida ativar o serve no terminal do projeto.

```bash
php artisan serve
```

Para testar API utilize uma ferramenta como o Postman ou o Insomnia
# As operações realizadas são:

Listar todas as tarefas:
<br>Método: GET
<br>URL: http://localhost:8000/api/tasks

Obter detalhes de uma tarefa específica:
<br>Método: GET
<br>URL: http://localhost:8000/api/tasks/{id}
<br>Substitua {id} pelo ID da tarefa desejada.

Criar uma nova tarefa:
<br>Método: POST
<br>URL: http://localhost:8000/api/tasks
<br>Corpo (em JSON):
```Json
{
  "title": "Tarefa 1",
  "description": "Descrição da tarefa 1",
  "completed": false
}
```
Atualizar os dados de uma tarefa existente:
<br>Método: PUT
<br>URL: http://localhost:8000/api/tasks/{id}
<br>Substitua {id} pelo ID da tarefa que deseja atualizar.
<br>Corpo (em JSON):
```Json
{
  "title": "Tarefa atualizada",
  "description": "Nova descrição",
  "completed": true
}

```
