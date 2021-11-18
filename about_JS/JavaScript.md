# JavaScript

## Primitive Data Types:

- String → (Text)

  ### String Manipulation

  ```jsx
  let string = 'string'
  string.charAt() or string[] //returns an index from the string.
  string.indexOf() //returns in which index the part of the string wanted starts.
  string.indexOf('string', 3) //with a number after, you start the point of the index search inside the string.
  string.lastIndexOf() //does the search backwards.
  string.replace('string', 'outraString') // replaces one part of the string for another.
  string.length //returns the size of the string.
  string.slice(0, 5) //returns a sliced part of the string.
  string.split('', 2) //returns in an array the results without the part inside the '' and after the comma sets the number of words of the string you want.
  string.toUpperCase() //puts the string into upper case.
  string.toLowerCase() //puts the string into lowercase.
  ```

- Number → (Numbers)

  Números seguem o padrão → IEEE 754-2008

  ```jsx
  let num = 1
  num = num.toString() //turns the value into a string for good.
  num.toString() //turns the value into a string only in the same line of the code, not from there and foward.
  num.soString(2) //show the binary form of that number.
  num.toFixed(/*number of wished decimal places*/)
  Number.isInteger(num) //check if the number is an integer
  Number.isNaN(num) //check if the variable is NaN(Not a Number)
  parseInt(num) //converges the number to an intenger.
  parseFloat(num) //converges the number to a floating number.
  ```

- Boolean → (True - False)
- Undefined and Null → (**Undefined** can only be set by the language itself, whereas **Null** can be set manually)

----

## Operadores

- Aritméticos

  Ordem de precedência:

  > ()

  > **

  > / * %

  > - - 

  5 + 2 = 7 /Soma

  5 - 2 = 3 /Subtração

  5 * 2 = 10 /Multiplicação

  5 / 2 = 2.5 /Divisão

  5 % 2 = 2 /Resto da divisão (para na vírgula)

  5 ** 2 = 25 /Potencialização

- Atribuição

  > **= Atribuição Simples**

  > **v = v + n** = **Auto-Atribuição  /  v += n = recebe ele mesmo**

  > V++ = **Incremento +1**  / ++V = **Pré-Incremento**

- Relacionais

  - < Menor

  - > Maior

  - <= Menor ou Igual

  - > = Maior ou Igual

  - == Igualdade de valor

  - === Igualdade de valor e tipo

  - != Diferente de valor

  - !== Diferente de valor e tipo

- Lógicos

  - ! Não
  - && And / Conjunção
  - || Or / Disjunção

- Ternário

  Se chama Ternário pois é dividido em 3 partes

  > teste ? true : false

  ```javascript
  média = 5
  média > 7 ? 'Aprovado':'Reprovado'
  ```

-----

## Condição Simples

```javascript
if(condição){
		true
}
```

## Condição Composta

```javascript
if(condição){
		true
}else{
		false
}
```

## Condição Aninhada

```javascript
if(condição1){
	bloco1
}else if(condição2){
		bloco2
	}else if(condição3){
			bloco3
	}
}
```

## Condição Múltipla

```javascript
switch(expressão) {
	case valor1:
	bloco1
	break

	case valor2:
	bloco2
	break

	case valor3:
	bloco3
	break

	default: //como se fosse o else
	bloco4
	break
}
```

----

## Repetições

```jsx
while(condição){ 
	bloco
} /* Repetição com teste lógico no íncio */
example:
var c = 1
while (c <= 10){
  console.log(`Hello, world ${c}`)
  c++
}
do{
	bloco
}while(condição)
/* Repetição com teste lógico no final */
example:
var c = 1
do{
  console.log(`Hello, world! ${c}`)
  c++
}while(c <= 10)
```

## Repetição com variável de controle

Inicialização

Teste Lógico

Incremento

```jsx
for(inicio ; teste ; incremento){
		BLOCO
}

example:

for(var c = 1/*inicio*/ ; c <= 10 /*teste lógico*/ ; c++ /* incremento */){
		BLOCO
}
```

------

> Sempre que for fazer uma repetição de X número até Y número, é preciso criar um contador(c)

-----

## Array

```jsx
var a/*array*/ = [a, b, c/*valor*/]/*elementos*/ 
a.[0, 1, 2/*indices*/]
var b [1, 2, 3]

var a = [a/*0*/, b/*1*/, c/*2*/, d/*3*/]
var a[4] = x /* cria a posição 4 no array e adicionar o valor x, agora a = [a, b, c , d, x]*/
a.push(y) /*cria mais uma posição no final do array e automaticamente define ela e coloca o valor y */
a.pop() /*remove o último valor do array*/
a.unshift() /*Adiciona um ou mais elementos no INICIO do array e retorno o valor atual do array*/
a.shit() /*remove o elemento no INICIO do array e retorna o que foi removido*/
a.length /* checa o tamanho do array*/
a.sort() /* ordena */
var c = a.concat(b)/*Concatena dois arrays*/
a.slice(0/*indice inicial*/,2/*indice final*/ ) /*fatia o array retornando apenas os valores indicados no indíce determinado*/
a.splice(0/*posição a ser mexida*/, 0/*quantos elementos vão ser removidos*/, 'olá'/*adição de um novo elemento no array*/) /*adiciona e remove elementos no array*/
a.map(value => value * 2)/*retorna um novo array, a partir da expressão passada no parâmetro*/
a.flat(/*paramêtro indica a profudindade a ser concatenada*/)  /*retorna um novo array com todos os elementos de um sub-array concatenados de forma recursiva de acordo com a depth*/
a.keys()/*retorna um Array Iterator que contém as chaves para cada elemento do array*/
a.values()/*retorna um Array iterator que contém os valores para cada elemento do array*/
a.entries()/* Retornar um array iterator que contém os pares chave/valor para cada elemento do array*/
a.find()/* retorna o primeiro item de um array que satisfaz a condição*/
a.findIndex()/*retorna o indice do primeiro item que satisfaz a condição*/
a.filter()/*retorna um novo array com todos os elementos que satisfazem a condição*/
a.indexOf()/*retorna o index de um elemento desejado*/
a.lastIndexOf()/*retorna o último index do elemento desejado*/
a.includes()/*retorna um boolean verificando se determinado elemento existe no array*/
a.some()/*retorna um boolean verificando se pelo menos um item de um array satisfaz a condição*/
a.every()/*retorna um boolean veririficando se todos os itens de um array satisfazem a condição*/
a.reverse()/*inverte a ordem do array*/
a.join()/*junta todos os elementos de um array, separados por um delimitador e retorna um string*/

for(var c in a){ /* repetição para variaveis compostas*/
		console.log(a[c])
}
```

> Um array é uma variável composta que tem vários elementos, cada elemento é composto por um valor e cada valor tem sua chave de identificação(indíce)



----

## Funções

- São **ações** executadas assim que são **chamadas** ou em decorrência de algum **evento**
- Uma função pode receber **parâmetros** e retornar um **resultado**

```jsx
function ação(parametro, parametro){
			bloco
			return x //retorno
}

ação(parametro) //chamada

function ação(n=0 /*parametro pré-definido*/)
```

## Arrow Functions

```js
const arrowFn = () => 'Code Here';
const arrowFn2 = () => {
    //Mais de uma expressão
    return 'Code Here'
}
```





-----

## Objeto Math

```jsx
let num1 = 9.9208390283
Math.floor(num1) // rounds the number to the lowest form.
Math.ceil(num1) // rounds the number to the highest form.
Math.round() // rounds to the nearest number.
Math.max() // takes the highest number from where you are asking for.
Math.random() // gives a random number between 0 - 1
Math.random() * (10 - 5) + 5; // how to set between which numbers you want.
```

----

## Currying

É uma técnica de transformar uma função com vários parâmetros em uma função que recebe apenas um parâmetro e também uma nova função e assim sucessivamente.

## Hoisting

O código JavaScript é executado em duas fases. Primeiro, é feito o **parsing**, em que são vasculhadas declarações de variáveis, funções e parâmetros. Só depois é feito a execução de fato.

O efeito disso é que é como se as declarações de variáveis fossem levantadas para o topo da função ou arquivo em que estão definidas.

----

## Orientação a Objetos

* Herança
* Classes
* Modificadores de acesso
* Encapsulamento
* Static

### Herança

* Baseada em protótipos
* Prototype
* Constructor

Prototype é uma variável que armazena as definições do nosso objeto. Toda vez que uma variável é criada um prototype é criado também apontando o tipo da variável criada, e esse tipo é chamado de **constructor**.

proto -> prototype -> constructor

proto aponta para um prototype que é criado a partir de uma função construtora

Exemplo:

```javascript
function Animal(){
    this.qtdePatas = 4;
}
const cachorro = new Animal();
```

Um novo objeto é criado herdando o Animal.prototype.

### Classes

* Simplificação da herança do prototype
* palavra chave **class**

----

### Design Patterns

Design Patterns são soluções generalistas para problemas recorrentes durante o desenvolvimento de um software. Não se trata de um framework ou um código pronto, mas de uma definição de alto nível de como um problema comum pode ser solucionado.

***Formato de um pattern***:

* Nome
* Exemplo
* Contexto
* Problema
* Solução

***Tipos de um pattern***:

* Criação
* Estruturais
* Comportamentais

***Padrões de criação***:

Os padrões de criação são aqueles que abstraem e/ou adiam o processo de criação dos objetos. Eles ajudam a tornar um sistema independente de como seus objetos são criados, compostos e representados.

Dentro dos padrões de criação temos:

* Abstract Factory
* Builder
* Factory Method
* Prototype
* Singleton

***Padrões estruturais***:

Os padrões estruturais se preocupam com a forma como classes e objetos são compostos para formar estruturas maiores.

Dentro dos padrões estruturais temos:

* Adapter
* Bridge
* Composite
* Decorator
* Facade
* Businesse Delegate
* Flyweight
* Proxy

***Padrões comportamentais***:

Os padrões de comportamento se concentram nos algoritmos e atribuições de responsabilidades entre os objetos. Eles não descrevem apenas padrões de objetos ou de classes, mas também os padrões de comunicação entre os objetos.

Dentro dos padrões comportamentais temos:

* Chain of responsability
* Command
* Interpreter
* Iterator
* Mediator
* Observer
* State
* Strategy
* Template Method
* Visitor

### Os patters mais utilizados no JavaScript são:

* Factory
* Singleton
* Decorator
* Observer
* Module

## Factory:

Todas as funções que retornam um objeto sem a necessidade de chamá-las com o **new**, são consideradas funções Factory.

## Singleton:

O objetivo desse pattern é criar uma única instância de uma função construtora e retorná-la toda vez em que for necessário utilizá-la.

## Decorator

Uma função decorator recebe uma outra função como parâmetro e estende o seu comportamento sem modificá-la explicitamente.

## Observer

A instância(subscriber) mantém uma coleção de objetos (observer) e notifica todos eles quando ocorrem mudanças no estado.

## Module

É um pattern que possibilita organizarmos melhor o nosso código, sem a necessidade de expor uma variável global.

----

# Rest e Spread Operator

O Rest operator ou "**...**", pega todos os parâmetros de uma função e transforma em um array, enquanto o Spread operator que também se identifica como "..." pega todos os itens de um array e transforma em parâmetros para uma função

# Symbols

Well Known Symbols

To be written...

# Generators

To be written...



# Fetch, Async / Await, EventEmitter



------

# Testes

## Testes automatizado

* Testes unitários;

São testes de pequenas partes do código, como um classe, um função, etc...

* Testes integrados;

São os testes de integração de parte do seu código, como duas classes reagem juntas ou como uma função dentro de outra função pode se comportar.

* Testes funcionais.

Testes feitos como se fosse um usuário, do começo ao fim.

## Testes manuais e automatizados

* Testes de usabilidade;
* Testes de aceitação do usuário;
* Protótipos;
* Testes funcionais;
* Exemplos;
* Alpha e beta;

## Ferramentas de teste

* Teste de carga e performance;
* Testes de segurança

## TDD

É um dos pilares do Extreme Programming, consiste em testar e refatorar em pequenos ciclos, onde você escreve o teste antes do código, faz o mesmo passar e refatora o código.









