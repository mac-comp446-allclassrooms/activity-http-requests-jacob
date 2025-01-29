Comp 446: HTTP requests Activity
====

Instructions are [here](https://docs.google.com/document/d/1aHX-jOnk14juvNDbtVdFRhyQxh-3Cmb5HcpaIuuUMqk/edit?usp=sharing).


# Step 2 

HTTP/1.1 200 OK
Server: Werkzeug/3.1.3 Python/3.13.0
Date: Wed, 29 Jan 2025 18:41:14 GMT
Content-Type: application/json
Content-Length: 370
Connection: close

{
  "tasks": [
    {
      "description": "Milk, Cheese, Pizza, Fruit, Tylenol",
      "done": false,
      "title": "Buy groceries",
      "uri": "http://127.0.0.1:5000/todo/1"
    },
    {
      "description": "Need to find a good Python tutorial on the web",
      "done": false,
      "title": "Learn Python",
      "uri": "http://127.0.0.1:5000/todo/2"
    }
  ]
}


# Step 3

HTTP/1.1 201 CREATED
Server: Werkzeug/3.1.3 Python/3.13.0
Date: Wed, 29 Jan 2025 18:53:46 GMT
Content-Type: application/json
Content-Length: 143
Connection: close

{
  "task": {
    "description": "my description",
    "done": false,
    "title": "my title",
    "uri": "http://127.0.0.1:5000/todo/3"
  }
}


# step 4

HTTP/1.1 200 OK
Server: Werkzeug/3.1.3 Python/3.13.0
Date: Wed, 29 Jan 2025 19:11:41 GMT
Content-Type: application/json
Content-Length: 142
Connection: close

{
  "task": {
    "description": "my description",
    "done": true,
    "title": "my title",
    "uri": "http://127.0.0.1:5000/todo/3"
  }
}

# Step 5 

HTTP/1.1 200 OK
Server: Werkzeug/3.1.3 Python/3.13.0
Date: Wed, 29 Jan 2025 19:13:03 GMT
Content-Type: application/json
Content-Length: 21
Connection: close

{
  "result": true
}

after results: 
HTTP/1.1 200 OK
Server: Werkzeug/3.1.3 Python/3.13.0
Date: Wed, 29 Jan 2025 19:13:35 GMT
Content-Type: application/json
Content-Length: 370
Connection: close

{
  "tasks": [
    {
      "description": "Milk, Cheese, Pizza, Fruit, Tylenol",
      "done": false,
      "title": "Buy groceries",
      "uri": "http://127.0.0.1:5000/todo/1"
    },
    {
      "description": "Need to find a good Python tutorial on the web",
      "done": false,
      "title": "Learn Python",
      "uri": "http://127.0.0.1:5000/todo/2"
    }
  ]
}