# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash

A backend server lets you store and retrieve data across clients.

```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash

Model

```

Which layer in the MVC pattern communicates with the model?

```bash

Controller

```

Why don't we use views in our interpretation of the MVC pattern?

```bash
We're using Rails as an API for single page applications, rather than using multiple pages that reload when we make a new request to the server. 

```

What does C.R.U.D stand for?

```bash
Create Read Update Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller
```

List at least 5 standard actions that C.R.U.D corresponds to?

```bash
create index show update destroy
```

A user action fires a `GET` request for `/persons/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
- the server communicates that GET request and the request path to the router
- the router interprets GET /persons/1 into a controller action to show a person with an ID of 1
- the controller talks to the Person model to get the necessary data from the people table in the database
- the model gives that data to the controller
- the controller passes that data to the view
- the server passes everything in the view (client-side resources like HTML & images + the data) back to the client, so the user can see it 

```

What is the command to generate a new rails-api app?

```bash
rails-api new [appname]
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails s
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
In Rails:

- db:drop
- db:create
- db:migrate



```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bundle exec rails-api g scaffold pet name:string age:integer
```
