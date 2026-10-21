# JavaScript Object Notation (JSON)

## What is JSON?

JSON (Javascript Object Notation) is a lightweight data interchange format. It uses key-value pairs and is similar to object literals in JavaScript.

The basic syntax consists of curly braces {}

for objects and square brackets [] for arrays.

- JSON is a **text format** for storing and exchanging data.
- JSON stands for **JavaScript Object Notation**.
- JSON syntax is similar to **JavaScript object syntax**.
- JSON is **language independent**.

## What Is JSON Used For?

- JSON is used to **send, receive** and **store data**.

- JSON is **integrated into JavaScript** and many other programming languages.

- The **JSON.parse()** method converts JSON text into JavaScript values.

- The **JSON.stringify()** method converts a JavaScript value into JSON text.

## Create JSON Objects/Arrays

You can create JSON objects and arrays in JavaScript using their respective literal syntax.

```js
// JSON Object
const person = {
  name: "Sujon Ahmed",
  age: 27,
  email: "sujonahmed5284@gmail.com",
};

// JSON Array
const fruits = ["Apple", "Banana", "Orange", "Mango"];
```

## Parse JSON

To convert a JSON string into a Javascript object, you can use JSON.parse().

```js
const jsonString = '{"name": "Sujon Ahmed", "age": 24}';

const person = JSON.parse(jsonString);

console.log(person.name); // Output: Sujon Ahmed
```

## Stringify JS objects to JSON

To convert a JavaScript Object into a JSON string, you can use JSON.stringify().

```js
const person = {
    name: "Sujon Ahmed"
    age: 24
};

const jsonString = JSON.stringify(person);

console.log(jsonString);
// Output: '{"name": "Sujon Ahmed", "age": 24}'
```

## Nested JSON

JSON supports nested structures, allowing you to create complex data hierarchies.

```js
{
    "name": "Sujon Ahmed",
    "age": 24,
    "address": {
        "city": "Dhaka City",
        "zipCode": "1207"
    }
}
```

## Working with JSON Arrays

JSON array can contain multiple values of different types, including other objects or arrays.

```js
[
  {
    name: "Sujon Ahmed",
    age: 24,
  },
  {
    name: "Riman",
    age: 25,
  },
];
```

_NB: JSON is not a JavaScript object._

Because the JSON format is syntactically identical to JavaScript, a JavaScript program can easily convert JSON data into native JavaScript values.

JavaScript has a built in function for converting JSON strings into JavaScript values:

**JSON.parse()**

JavaScript also has a built in function for converting JavaScript values into a JSON strings:

**JSON.stringify()**

## Converting JSON to JavaScript

Before JavaScript can work with JSON text, the text has to be converted into a JavaScript value.

The JSON.parse() method converts JSON text into a JavaScript value:

```js
const jsonString = '{"name": "Sujon Ahmed", "age": 24}';
const person = JSON.parse(jsonString);
console.log(person.name); // Output: Sujon Ahmed
```

After parsing, the properties can be accessed with normal JavaScript object syntax.

The JSON.parse() method does not always return an object.

It returns the JavaScript value represented by the JSON text.

## Converting JavaScript to JSON

The JSON.stringify() method converts a JavaScript value into JSON text:

```js
const person = {
  name: "Sujon Ahmed",
  age: 24,
};

const jsonString = JSON.stringify(person);
```

## JSON Round Trip

```
JSON text

🠇

JSON.parse()

🠇

JavaScript value

🠇

JSON.stringify()

🠇

JSON text
```

## Storing Data

When storing data, the data has to be a certain format.

Regardless of where you choose to store data, text is always a handy format.

JSON makes it possible to store JavaScript values as text.

```
You can receive pure text from a server and use it as a JavaScript object.

You can send a JavaScript object to a server in pure text format.

You can work with data as JavaScript objects, with no complicated parsing and translations.
```

## JSON Files

JSON data can be stored in a file.

JSON files normally use the .json file extension.

```json
customer.json
{
  "name": "Sujon Ahmed",
  "age": 24,
  "email": "sujon.ahmed@example.com"
}
```

- The file type for JSON files is ".json"
- The MIME type for JSON text is "application/json"

## JSON Is Language Independent

JSON was inspired by JavaScript object syntax, but it is not limited to JavaScript.

Code for reading and generating JSON data can be written in any programming language.

- JSON is text only and language independent
- JSON makes it easy to send data between computers
