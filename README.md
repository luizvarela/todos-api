# Todos API

```

bundle install
rails s

```

You can use https://httpie.org/ to test the endpoints.

```

# GET /todos
$ http :3000/todos
# POST /todos
$ http POST :3000/todos title=Mozart created_by=1
# PUT /todos/:id
$ http PUT :3000/todos/1 title=Beethoven
# DELETE /todos/:id
$ http DELETE :3000/todos/1

```

```

# POST /todos
$ http POST :3000/todos title=Mozart created_by=1
# GET /todos/:todo_id/items
$ http :3000/todos/2/items
# POST /todos/:todo_id/items
$ http POST :3000/todos/2/items name='Listen to 5th Symphony' done=false
# PUT /todos/:todo_id/items/:id
$ http PUT :3000/todos/2/items/1 done=true
# DELETE /todos/:todo_id/items/1
$ http DELETE :3000/todos/2/items/1

```
