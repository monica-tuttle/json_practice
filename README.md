# JSON Processing
JSON is a data interchange format used widely on The Internet and supported by most programming languages

## Encoding Python objects in JSON
We can create a Python dictionary and then encode it using JSON and write to a file:
```
bookshelf = {}
bookshelf["The Things They Carried by Tim O'Brien"] = 'Fiction
bookshelf['Thinking, Fast and Slow by Daniel Kahneman'] = 'Psychology'
bookshelf["E-books"] = ['Sapiens: A Brief History of Humankind', ('Learning the Vi and Vim', 'BASH Guide')]

```
with open('bookshelf.json', 'w') as books_file:
    books_file.write(json.dumps(bookshelf))
```
