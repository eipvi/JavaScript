# Boolean e Conditionals.

In JavaScript, a boolean is a data type that can have only two values: true or false. The boolean type is used to express logical conditions and control the flow of program execution.

Boolean values are often used in control structures, such as conditional statements (if-else, switch) and loops (while, for), to determine which code blocks should be executed based on a condition.

## Conditionals: if and else.

Check if an expression is true with if, otherwise else will be activated.

### Example 1

```
var possuiGraduacao = true;

if(posuiGraduacao) {
  console.log('Possui graduação');
} else {
  console.log('Não possui graduação');
}
```

Result: It will return "Has a degree" and will not execute the else statement.

The value inside the parentheses will always be evaluated as FALSE or TRUE.

### Example 2

```
var possuiGraduacao = true

if(possuiGraduacao) {
  console.log('É VERDADEIRO');
  var x = 10;
} else {
  console.log('É FALSO');
}

console.log(x)
```

Result: It will return "It is true" and the number "10". Since possuiGraduacao is true, the code block for X will be executed.

### Example 3

If the if statement is not true, it tests the else if statement.

```
var possuiGraduacao = true;
var possuiDoutorado = false;

if(possuiDoutorado)
console.log('Possui graduação e doutorado');
} else if(possuiGraduacao)
console.log('Possui graduação,mas não possui doutorado');
} else {
  console.log('Não possui graduação');
}
```

Result: It returns 'Has a degree, but does not have a doctorate' because the first condition is false and in the next condition "possuiGraduacao" is true, thus finalizing the result.

### Example 3

```
var nome = '';

if(nome) = ''
  console.log(nome);
} else {
  console.log('Nome não existente');
}
```

Result: Name does not exist. This result occurs because the string is empty.

## Operadores lógicos &&

&& It compares if one expression and the other are true.

```
true && true; //true
true && false; //false
false && true; //false
'Gato' && 'Cão'; //'Cão'
(5 - 5) && (5 + 5); //0
'Gato' && false; //false
(5 >= 5) && (3 < 6); //true
```

If both values are true, it will return the last value checked. If any value is false, it will return false and will not continue checking the next values.

### Example 1

```
var condicional = (5 - 10)) & (5 + 5);
if(condicional) {
  console.log('Verdadeiro', condicional);
} else {
  console.log('Falso');
}
```

Respost: 10, "Verdadeiro".

## Operadores lógicos ||

It compares if either one expression or the other is true.

```
true || true; //true
true || false; //true
false || true; //true
'Gato' || 'Cão'; //'Gato'
(5 - 5) || (5 + 5); //10
'gato' || false; //Gato
(5 >= 5) || (3 < 6); //true
```

Result: It returns the first true value it encounters.

## Switch

With the switch statement, you can check if a variable is equal to different values using case. If it matches a case, you can perform some actions and use the keyword break to exit the switch statement. The default value will be executed if none of the previous cases are true.

```
var corFavorita = 'Azul';

switch (corFavorita)
  case 'Azul':
    console.log('Olho para o céu.')
    break;
  case 'Vermelho':
     console.log('Olhe para rosas.')
    break;
  case 'Amarelo':
     console.log('Olhe para o sol.')
    break;
  default:
  console.log('Feche os olhos.')
```

Result: "Olho para o céu".

### Example 1

```
var minhaIdade = 27;
var idadePrimo = 22;

if (minhaIdade > idadePrimo) {
  console.log('É maior');
} else if (minhaIdade === idadePrimo) {
  console.log('É igual');
} else {
  console.log('É menor');
}
```

Result: "É maior"

### Example 2

```

if (('Gato === 'gato') && (5 > 2)) {
  console.log('Verdadeiro');
} else {
  console.log('Falso');

```

Result: "Falso"
