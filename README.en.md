# Welcome to the ES6 and Unit Tests project repository!

### README Translations:

-   [English](/README.en.md)
-   [Portuguese](/README.md)

* * *

## 👨‍💻 What was developed:

-   In this project, I implemented several functions in the resolution of the proposed requirements and/or unit tests to guarantee that the implementations of the functions are correct, according to what was being requested in each statement.

    In this project, I was able to:

-   Write unit tests using the NodeJS Jest module to verify the correct functioning of the functions;

-   Write functions so that they meet already implemented tests;

-   Write tests and functions using a test-driven development approach.

    The implemented functions are inside the folder`src`and their respective tests are in the folder`tests`. The file names also follow a defined order. Basically, test files have the name of the target file (feature file) plus the name`.spec.js`.

    Each function has a comment block on its first lines explaining what work the function is supposed to do.

# Mandatory Requirements

* * *

### 1. Implement the function`average`

<details>
  <summary>A função average recebe um array de tamanho variável e retorna a média dos valores recebidos. Caso a função receba algum valor não numérico ou um array vazio, o valor `undefined` deve ser retornado.</summary><br/> 
  
  Todos os resultados devem ser arredondados para valores inteiros. Ex: 4,6 vira 5; 1,3 vira 1. O arquivo `average.spec.js` contém os testes para `average` já implementados. Implemente a função no arquivo `src/average.js` de forma que ela atenda aos testes propostos.

**What will be tested:**

-   It will be validated if, when receiving an array of numbers, the function`average`returns the average of its values;
-   It will be validated if, when receiving an array that contains non-numeric values, the function`average`Returns`undefined`;
-   It will be validated if, when receiving an empty array, the function`average`Returns`undefined`.

</details>

* * *

### 2. Implement the test cases for the function`numbers`

<details>
  <summary>A função `numbers` recebe um array de tamanho variável e retorna `true` se todos os parâmetros forem do tipo 'number' e `false` caso contrário.</summary><br/> 
  
  Essa função já está implementada no arquivo `src/numbers.js`. Escreva pelo menos quatro testes para essa função para garantir que a implementação de `numbers` está correta.

**What will be tested:**

-   It will be validated if in the function test`numbers`, the function returns is`true`when the array passed by parameter contains only numbers.

</details>

* * *

### 3. Implement the function`vqv`

<details>
  <summary>Use template literals para escrever uma função que recebe o seu nome e a sua idade e retorna o parágrafo descrito abaixo:</summary><br/>

```javascript
`Oi, meu nome é Tunico!
Tenho 30 anos,
trabalho na Trybe e mando muito em programação!
#VQV!`
```

If the function is called without any parameters, the value`undefined`must be returned. The file`vqv.spec.js`contains the tests for`vqv`already implemented. Implement the function in the file`src/vqv.js`so that it meets the proposed tests.

**What will be evaluated**

-   It will be validated if`vqv`is a function;
-   It will be validated if the function`vqv`returns string data;
-   It will be validated if the function`vqv`returns the expected phrase when passed name and age parameters;
-   It will be validated if the function`vqv`, when called without parameter, returns`undefined`.

</details>

* * *

### 4. Implement the test cases for the function`circle`

<details>

  <summary>A função `circle` recebe o raio de um círculo e retorna um objeto contendo as suas informações: Raio, Área e Circunferência. Se não for especificado um raio, a função retorna `undefined`.</summary></br>
  
  Essa função já está implementada no arquivo `src/circle.js`. Escreva pelo menos seis testes para essa função para garantir que a implementação de `circle` está correta.

**What will be evaluated**

-   It will be validated if in the function test`circle`, when receiving a radius, the function returns an object with the correct information (Radius, Area and Circumference).

</details>

* * *

### 5. Implement the function`createStudent`

<details>
<summary>A função `createStudent` recebe como parâmetro um **nome**, e retorna um objeto contendo duas chaves:</summary></br>

1.  **name**, containing the name passed as a parameter;
2.  **feedback**, containing a function that returns the phrase 'Jeez good person!' when being called.

    The file`createStudent.spec.js`contains the tests for`createStudent`already implemented. Implement the function in the file`src/createStudent.js`so that it meets the proposed tests.

    **What will be evaluated**

-   It will be validated if the function`createStudent`returns an object that contains two keys:`name`, containing the name passed as a parameter; and`feedback`, containing a function that returns the phrase 'Jeez good person!' when being called.

</details>

* * *

### 6. Implement the test cases for the function`productDetails`

<details>
  <summary>A função `productDetails` recebe duas strings que representam nomes de produtos, e retorna um array contendo dois objetos com os detalhes dos respectivos produtos:</summary></br>

```javascript
productDetails('Alcool gel', 'Máscara');
```

**Returns:**

```js
[
  {
    name: 'Alcool gel'
    details: {
      productId: 'Alcool gel123'
    }
  },
  {
    name: 'Máscara'
    details: {
      productId: 'Máscara123'
    }
  }
]
```

This function is already implemented in the file`src/productDetails.js`. Write at least five tests for this function in the file`tests/productDetails.js`to ensure that the implementation of`productDetails`it's correct.

**What will be evaluated**

-   It will be validated if in the function test`productDetails`, when receiving two strings, the function returns an array of objects and whether each object contains the necessary data.

</details>

* * *

### 7. Implement the functions`calculator`e`arrayGenerator`

<details>
  <summary>A função `calculator` recebe dois números inteiros como parâmetro e retorna um objeto com as seguintes chaves:</summary></br>
  - sum;
  - mult;
  - div;
  - sub.

For each key, assign as a value the operation corresponding to its key:

-   `sum:`returns the result of the sum of the two numbers;

-   `mult:`returns the result of multiplying the two numbers;

-   `div:`returns the result of dividing the two numbers;

-   `sub:`returns the result of subtracting the two numbers.

    Division results should always be rounded down.

    Parameters:

-   Two whole numbers.

    Behavior:

    ```javascript
    calculator(1, 2); // { sum: 3, mult: 2, div: 0, sub: -1 }
    ```

    Already the function`arrayGenerator`converts objects to arrays, of keys, values, or both. It must take two parameters:

-   the first parameter must be a string indicating the type of conversion;

-   the second parameter should be an object similar to the one returned by the calculator function you just developed.

    Parameters:

-   A string indicating the type of conversion;

-   An object of the form { sum: 3, mult: 2, div: 0, sub: -1 };

    Behavior:

    ```javascript
    arrayGenerator('keys', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 'sum', 'mult', 'div', 'sub' ]
    arrayGenerator('values', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 3, 2, 1, 0 ]
    arrayGenerator('entries', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ [ 'sum', 3 ], [ 'mult', 2 ], [ 'div', 1 ], [ 'sub', 0 ] ]
    ```

    The file`objPlayground.spec.js`contains the tests for`calculator`e`arrayGenerator`already implemented. Implement the functions in the file`src/objPlayground.js`so that it meets the proposed tests.

    **What will be evaluated**

-   It will be evaluated if the function`calculator`returns the expected values;

-   It will be evaluated if the function`arrayGenerator`returns the expected values.

</details>

* * *

### 8. Implement the function`myCounter`

<details>
  <summary>A função myCounter possui dois loops aninhados que inserem valores dentro de um array. Como podemos perceber, eles vão adicionando valores ao array até sua condição de parada.</summary></br>

fix the function`myCounter`, without eliminating any of the repeat loops, so the function returns the correct array. The file`myCounter.spec.js`contains the tests for`myCounter`already implemented. Implement the function in the file`src/myCounter.js`so that it meets the proposed tests.

**What will be evaluated**

-   It will be validated if the function`myCounter`returns the expected data according to what is implemented in the test.

</details>

* * *

### 9. Implement the test cases for the function`getCharacter`

<details>

  <summary>A função `getCharacter` recebe uma string que representa o nome de uma personagem e retorna um objeto contendo o seu nome, a sua classe e as suas frases.</summary></br>

```javascript
getCharacter('Arya');
```

**Returns:**

```javascript
{
  name: 'Arya Stark',
  class: 'Rogue',
  phrases: ['Not today', 'A girl has no name.']
}
```

This function is already implemented in the file`src/getCharacter.js`. Write at least six tests for this function in the file`tests/getCharacter.spec.js`to ensure that the implementation of`getCharacter`it's correct.

**What will be evaluated**

-   It will be validated if in the function test`getCharacter`when receiving a string, the function's return is as expected - according to the table presented in the test file.
-   It will be validated if in the function test`getCharacter`when not receiving any parameter, the function return is`undefined`.
-   It will be validated if the function test`getCharacter`checks if the parameter is case sensitive.

</details>

* * *

### 10. Implement the function`createMenu`, as well as its test cases

<details>
  <summary>Esse último requisito vai guiar você por um rico processo de Desenvolvimento Orientado a Testes ou TDD - Test Driven Development</summary></br>

Imagine the following situation: you are responsible for writing the code for a restaurant's ordering system through which it will be possible to register a menu. Once a menu has been registered, the system must provide an object that allows:

-   Read the registered menu;
-   place orders;
-   Check what was requested;
-   Add the account value.

    The structure of this code and this object is already defined and you need to implement it. You will find more details about the structure to follow and examples of the function return in the file`src/restaurant.js`.
    You should orient yourself through the topics below to ensure the proper development of the system.

    **IMPORTANT - GOOD TDD PRACTICES: START WITH FILE TEST 1`tests/restaurant.spec.js`**

1.  In the file`tests/restaurant.spec.js`, write a test that checks whether the function`createMenu()`returns an object that has the key`fetchMenu`, which has a function as its value.

2.  In the file`tests/restaurant.spec.js`, write a test that checks whether`'objetoRetornado.fetchMenu()'`returns an object whose keys are only`food`e`drink`, considering that the function`createMenu()`was called with the object:`{ food: {}, drink: {} }`.

3.  In the file`tests/restaurant.spec.js`, write a test that checks if my passed to function`createMenu()`is identical to the menu retrieved by the function`'objetoRetornado.fetchMenu()'`.

4.  In the file`src/restaurant.js`, create a function`createMenu()`which, taking an object as a parameter, returns this object with the following format: { fetchMenu: () =>ObjectPassedByParameter }.

5.  In the file`tests/restaurant.spec.js`, write a test that checks whether`'objetoRetornado.consumption'`, after creating the menu, returns an empty array.

6.  In the file`src/restaurant.js`, add to the object returned by`createMenu()`a key`consumption`which, as an initial value, has an empty array.

7.  In the file`tests/restaurant.spec.js`, write a test that checks that when calling a function associated with the key`order`in the returned object, passing a string as a parameter (like`objetoRetornado.order('coxinha')`), that string is added to the array returned in`objetoRetornado.consumption`.

8.  In the file`src/restaurant.js`, create a function, separate from the function`createMenu()`, which, when receiving a string as a parameter, adds that string to the array of`objetoRetornado.consumption`. This new function will be added to the key`order`.

9.  In the file`tests/restaurant.spec.js`, write a test that checks if when adding three orders, between drinks and food, the array`objetoRetornado.consumption`contains the ordered items.

10. In the file`tests/restaurant.spec.js`, write a test that checks whether the function`order`accepts that repeat orders be added to`consumption`.

11. In the file`tests/restaurant.spec.js`, write a test that verifies that when calling`objetoRetornado.pay()`, the sum of the prices of everything that was ordered is returned, as recorded in`objetoRetornado.consumption`.

12. In the file`src/restaurant.js`, add to the object returned by`createMenu()`a key`pay`with a function that loops through all items of`objetoRetornado.consumption`, sums their price and returns the summed value plus 10%. TIP: for this you will need to loop through both the key object`food`how much the key object`drink`.

    **What will be evaluated**

-   It will be validated if the function`createMenu()`returns the expected data.
-   It will be validated if the function test`createMenu()`checks each of the function's returns and whether these returns have the expected behavior.

</details>
