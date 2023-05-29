# Repository JavaScript

Repository dedicated to the study of JavaScript to improve knowledge in long-term projects.

## Guide to topics covered:

### 📌 Variables and Data Types:

- Learn how to declare variables, understand data types (such as strings, numbers, and booleans), and perform basic operations with them.

```
let name = 'John';
const age = 25;
var isStudent = true;
```

### 📌Control Structures:

- Explore conditional statements (if/else, switch) and loops (for, while) to control the flow of your program.

```
if (age >= 18) {
  console.log('You are an adult.');
} else {
  console.log('You are a minor.');
}

for (let i = 0; i < 5; i++) {
  console.log(i);
}

while (isStudent) {
  console.log('Still a student');
}
```

### 📌Functions:

- Learn how to define and call functions in JavaScript, pass arguments, and return values.

```
function greet(name) {
  console.log('Hello, ' + name + '!');
}

greet('Alice');
```

### 📌Arrays:

- Understand how to work with arrays, access elements, add and remove items, and iterate over array elements.

```
let numbers = [1, 2, 3, 4, 5];

console.log(numbers[2]); // Output: 3

numbers.push(6);
numbers.pop();

```

### 📌Objects:

- Learn about objects in JavaScript, how to create them, access properties and methods, and work with nested objects.

```
let person = {
  name: 'John',
  age: 25,
  isStudent: true,
  address: {
    street: '123 Main St',
    city: 'New York'
  }
};

console.log(person.name); // Output: John
console.log(person.address.city); // Output: New York

```

### 📌DOM Manipulation:

- Explore how to interact with the HTML structure of your document using JavaScript, manipulating elements, changing content, styles, and handling events.

```
// Selecionando elementos do DOM
let titleElement = document.getElementById('title');
let buttonElement = document.getElementById('btn');

// Manipulando conteúdo do elemento
titleElement.textContent = 'Hello, DOM!';

// Adicionando um evento de clique ao botão
buttonElement.addEventListener('click', function() {
  // Alterando o estilo do título quando o botão for clicado
  titleElement.style.color = 'red';
});
```

### 📌String Manipulation:

- Learn how to manipulate strings in JavaScript, such as concatenating, splitting, replacing, and formatting text.

```
let message = 'Hello, World!';
console.log(message.length); // Output: 13

console.log(message.toUpperCase()); // Output: HELLO, WORLD!

let fullName = 'John Doe';
let firstName = fullName.split(' ')[0];

```

### 📌Event Handling:

- Understand how to handle events such as button clicks, form submissions, and keyboard events, and associate functions with these events.

```
let button = document.querySelector('button');
button.addEventListener('click', function() {
  console.log('Button clicked!');
});

```

### 📌AJAX and Asynchronous Requests:

- Learn how to make asynchronous requests using the XMLHttpRequest object or the fetch API to interact with web services and dynamically update page content.

```
// Selecionando elementos do DOM
let buttonElement = document.getElementById('btn');
let dataContainerElement = document.getElementById('data-container');

// Adicionando um evento de clique ao botão
buttonElement.addEventListener('click', function() {
  // Fazendo uma requisição AJAX
  let xhr = new XMLHttpRequest();
  xhr.open('GET', 'https://api.example.com/data', true);

  xhr.onload = function() {
    if (xhr.status === 200) {
      // Atualizando o conteúdo do elemento com os dados recebidos da requisição
      dataContainerElement.textContent = xhr.responseText;
    }
  };

  xhr.onerror = function() {
    // Exibindo uma mensagem de erro em caso de falha na requisição
    dataContainerElement.textContent = 'Failed to load data.';
  };

  // Enviando a requisição
  xhr.send();
});
```

and

```
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.log(error));

```

### 📌Error Handling:

- Understand how to handle errors and exceptions in JavaScript using try/catch, and how to throw and handle your own exceptions.

```
try {
  // Code that may throw an error
  throw new Error('Something went wrong!');
} catch (error) {
  console.log('Error:', error.message);
}

```

### 📌Date and Time Manipulation:

- Explore the functionalities to work with dates and times in JavaScript, such as creating Date objects, formatting, and manipulating dates.

```
let now = new Date();
console.log(now.toLocaleDateString()); // Output: 5/29/2023

let tomorrow = new Date();
tomorrow.setDate(tomorrow.getDate() + 1);
console.log(tomorrow.toLocaleDateString()); // Output: 5/30/2023

```

### 📌Local Storage:

- Learn how to use browser's local storage (localStorage or sessionStorage) to store data on the client-side.

```
localStorage.setItem('username', 'John');
console.log(localStorage.getItem('username')); // Output: John

localStorage.removeItem('username');

```
