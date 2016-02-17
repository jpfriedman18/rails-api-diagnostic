# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
  A backend allows data to be stored and persist regardless of what is happening
  on the client side of an application. It also allows different clients using
  and app to interact with each other
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
  The model is used to get data from a database
```

Which layer in the MVC pattern communicates with the model?

```bash
  The controller communicates with the model
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
  Because it is 2016 and we make single-page apps
```

What does C.R.U.D stand for?

```bash
  Create
  Read
  Update
  Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
  The Model uses CRUD actions to interact with the database
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
  - The GET request is routed to the correct controller for people
  - The people controller sends the GET request to the correct model
  - The model finds the person with id:1
  - The model sends all data on that person instance back to the controller
  - The controller sends the data it receives from the model to the browser
    as JSON
```

What is the command to generate a new rails-api app?

```bash
rails-api new some_app -T --database=postgresql
```

What is the command to start an instance of a rails server?

```bash
  rails server
  or rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
  - rake db:create
  - rake db:migrate
  - rake db:drop
```

What is the command to scaffold a pet with a name and an age?

```bash
  rails-api g scaffold pet name:string age:integer
```

List two advantages of using serializers? (2 bullet points)

```bash
  - Serializers improve data security, as only certain specified attributes
    can be sent to clients via JSON
  - They also allow us to send nice clean JSON responses to queries
```
