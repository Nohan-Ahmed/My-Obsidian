---
source: 
Date created: 2023-11-14
Tagged concepts:
  - JSON
Type:
  - - tamplate
tags:
  - JSON
---
## What is JSON?

- JSON stands for *JavaScript Object* Notation.
- A JSON object is a collection of key-value pairs. you simply called `JSON` is a dictionary.
- JSON is a **text format** for storing and transporting data, that is completely language-independent.

What is JavaScript Object Notation?
- JavaScript object  is a `key: value` pairs. It is similar to a Python dictionary.

##### JSON syntax is similar to the syntax for creating objects in JavaScript. 

```JSON
{
  "name": "John Doe",
  "age": 30,
  "occupation": "Software Engineer",
  "hobbies": ["Coding", "Gaming", "Reading"],
  "address": {
    "street": "123 Main Street",
    "city": "San Francisco",
    "state": "CA",
    "zip": "94105"
  }
}
```

## Data Types in JSON

In **JSON**, _values_ must be one of the following data types:
- string
- number
- object
- array
- Boolean
- null
## Accessing JSON Data
You can access JSON data using *Dot notation* and using *square* [key] brackets, same like accessing [[JavaScript object]].

> example:

```JSON
{
  "person": {
    "name": "John Doe",
    "age": 25,
    "address": {
      "city": "New York",
      "zipcode": "10001"
    },
    "hobbies": ["reading", "traveling"]
  }
}
```

```JavaScript
// Accessing the person's name
// Accessing by Dot Notation
const name = jsonData.person.name;
console.log(name); // Output: John Doe

// Accessing like python dictionary.
const name = jsonData["person"]["name"];
console.log(name); // Output: John Doe

```

## Serialization and Deserialization

JSON conversion is the process of changing data into JSON format or changing JSON format data into another format. This process is often called serialization (converting data to JSON) and deserialization (converting JSON to data). Below are examples of JSON conversion using JavaScript.
#### Serialization (Object to JSON):
The **`JSON.stringify()`** static method converts a JavaScript object to a JSON string.

```JavaScript
const person = {
  name: "John Doe",
  age: 25,
  isStudent: true
};

// Convert JavaScript object into JSON string.
const jsonString = JSON.stringify(person);
console.log(jsonString);

```

#### Deserialization (JSON to Object):
JSON.parse() is a method in JavaScript that parses a JSON string and returns the corresponding JavaScript object.

```JavaScript
const jsonText = '{"name":"John Doe","age":25,"isStudent":true}';

// convert JSON string into JavaScript object.
const personObject = JSON.parse(jsonText);
console.log(personObject);
```

## Differences between  JavaScript object and JSON

In JSON, _keys_ must be strings, written with double quotes:
```JSON
{"name":"John"}
```

In JavaScript, keys can be strings, numbers, or identifier names:
```Js
{"name":"John"}
```

