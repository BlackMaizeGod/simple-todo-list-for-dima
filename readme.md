# Lumen PHP Framework

## Documentation
This is only simple todo list REST api

User only able to access their own ToDo list.

## Endpoint

# Header
- Content-Type: application/json
- Accept: application/json
- Authorization: Bearer <token>

# Users endpoint
http://todo-list-api.local/api/login
- username
- password

http://todo-list-api.local/api/register
- username
- password

# ToDo endpoint

## List all available todo (method:GET)
http://todo-list-api.local/api/todo/

has parameter of
 - order_by=column_name
 - direction=<ASC or DESC>

 example http://todo-list-api.local/api/todo/?order_by=priority&direction=DESC

## Display all completed todo (method:GET)
http://todo-list-api.local/api/todo/completed

## Creat new todo (method:POST)
http://todo-list-api.local/api/todo/

input params
  - name (string)
  - priority (digits)
  - location (string)
  - start_time (time format 00:00)

## Updating todo (method:PUT)
http://todo-list-api.local/api/todo/<id>

## Deleting todo (method:DELETE)
http://todo-list-api.local/api/todo/<id>