## Exercise 1 - requests library
**Goal**: become familiar with the requests library  
**Purpose**: interacting programmatically with an API

### Assignment
Print the status code and response for the following API calls:
- GET knockknock
- GET books
- GET one book
- POST a book
- POST auth

You can find a description of the APIs in `API-docs.md`.

Don't forget to explore and generate some error responses.     

### The requests library
The requests library allows you to send API requests with `requests.get(<url>)`,
`requests.post(url, json=<python_dictionary>)`, etc.  
This will return a `response` object with (among other things) the following attributes:
- `response.status_code`: http status code of the response
- `response.text`: the response body as plain text
- `response.json()`: parses a json response body to a a Python dictionary

Use `python <your_file>.py` to run your code.

Docs for the requests library: http://docs.python-requests.org/en/master/