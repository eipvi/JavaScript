# Functions

A function in JavaScript is a reusable block of code that can be executed when needed. It can receive parameters (values) as input, perform a set of instructions, and return a result. Functions are a fundamental part of JavaScript programming and allow you to organize your code, make it more modular, and avoid code repetition.

In JavaScript, you can define functions in various ways. The most common way is by using the function keyword followed by the function name, a list of parameters inside parentheses, and a code block inside curly braces.

Here's an example of a simple function that takes two numbers as parameters and returns their sum:

```
function somar(a, b) {
  return a + b;
}
```

In this example, the sum function takes two parameters a and b and returns their sum using the + operator. To execute this function and obtain the result, you can call it as follows:

```
var resultado = somar(2, 3);
console.log(resultado); // Output: 5
```

In the example above, the sum function is called with the arguments 2 and 3, and the return value, 5, is assigned to the result variable and then printed to the console.

Additionally, functions in JavaScript can also be assigned to variables, passed as arguments to other functions (higher-order functions), and returned by other functions. These features make functions in JavaScript very flexible and powerful.

### Example 1

```
function areaQuadrado(lado) {
  return lado * lado;
}

areaQuadrado(4) //16
areaQuadrado(5) //25
areaQuadrado(2) //4
```

### Example 2

```
function areaQuadrado(lado) {
  return lado * lado;
}

console.log(areaQuadrado(10));

```

### Example 3

Create a function that returns your full name:

```
function nomeCompleto(nome, sobrenome) {
  return `${nome} ${sobrenome}`; //ou + ' ' + sobrenome;
}
```

### Example 4

Create a function that checks if a number is even.

```
function isEven(numero) {
  var modulo = numero % 2;
  if(modulo === 0) {
    return true;
} else {
    return false;
  }
}
```

### Example 5

Create a function that returns the data type of the argument passed in it (typeof).

```
function tipoDeDedo(dado) {
  return typeof dado;
}
```

### Example 6

Parentheses () perform a function.

```
function pi() {
  return 3.14;
}

var total = 5 * pi(); //15.7
console.log(pi()) //3.14
```

## Parameters and Arguments

When creating a function, you can define parameters. When executing a function, you can pass arguments.

Separate each parameter with a comma. You can define more than one parameter or none as well.

```
function imc(peso, altura //parâmetro ) {
  const imc = peso / (altura ** 2);
  return imc;
}

imc(80, 1.80) //80 e  1.80 são argumentos
imc(60, 1.70) //60 e 1.70 são argumentos
```

## Arguments can be functions

Use addEventListener to display your full name on the console when the 'click' event occurs.

```
addEventListener('click', function() {
  console.log('Paula Vieira');
});
```
