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
http://your-domain-host/api/login
- username
- password

http://your-domain-host/api/register
- username
- password

# ToDo endpoint

## List all available todo (method:GET)
http://your-domain-host/api/todo/

has parameter of
 - order_by=column_name
 - direction=<ASC or DESC>

 example http://your-domain-host/api/todo/?order_by=priority&direction=DESC

## Display all completed todo (method:GET)
http://your-domain-host/api/todo/completed

## Creat new todo (method:POST)
http://your-domain-host/api/todo/

input params
  - name
  - priority
  - location
  - start_time

## Updating todo (method:PUT)
http://your-domain-host/api/todo/<id>

## Deleting todo (method:DELETE)
http://your-domain-host/api/todo/<id>