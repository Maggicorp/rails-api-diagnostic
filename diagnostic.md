# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
The backend stores information and data so that it can stored and retrieved after a user logs on and off and back on again.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
// your response here
```

Which layer in the MVC pattern communicates with the model?

```md
The controller communicates with the model.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
We don't use views because they aren't as absolutely necessary as it is to undrestand the relationship between teh contrller and the model.
```

What does C.R.U.D stand for?

```md
Create, Read, Update, Delete```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
CRUD methods are executed by the controlled.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
index/get request for all items in the database
a index/get request for one item in the database
a patch request to edit one item in the database
a create/post request to all a new item to the database
a destroy request to get ride of one thing in the database
a destory request to get rid of everything in the database

```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1.) Get request connect to route which specifies a get method on the people controller
2.) People controller uses defined get method and takes in the params 1
3.) People controller connects to the people model to retrieve the person with :id 1.
4.) people model return data back to the controller who returns it to the servers where the client can see the a represenation of the data in people at id 1.
```

What is the command to generate a new rails-api app?

```bash
rails new new_app
```

What is the command to start an instance of a rails server?

```bash
rails server ```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
DROP DATABASE OldDB
CREATE DATABASE NewDB
bin/rails db:migreate
rake db:seed

```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold NewPet name:string age:integer```
