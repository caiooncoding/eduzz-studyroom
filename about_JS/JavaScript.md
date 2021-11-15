# JavaScript

## Currying

É uma técnica de transformar uma função com vários parâmetros em uma função que recebe apenas um parâmetro e também uma nova função e assim sucessivamente.

## Hoisting

O código JavaScript é executado em duas fases. Primeiro, é feito o **parsing**, em que são vasculhadas declarações de variáveis, funções e parâmetros. Só depois é feito a execução de fato.

O efeito disso é que é como se as declarações de variáveis fossem levantadas para o topo da função ou arquivo em que estão definidas.

----

# Operadores

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

# Condição Simples

```javascript
if(condição){
		true
}
```

# Condição Composta

```javascript
if(condição){
		true
}else{
		false
}
```

# Condição Aninhada

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

# Condição Múltipla

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

------

# Repetições

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

for(
```

------

> Sempre que for fazer uma repetição de X número até Y número, é preciso criar um contador(c)

------

# Array

```jsx
var a/*array*/ = [a, b, c/*valor*/]/*elementos*/ 
a.[0, 1, 2/*indices*/]

var a = [a/*0*/, b/*1*/, c/*2*/, d/*3*/]
var a[4] = x /* cria a posição 4 no array e adicionar o valor x, agora a = [a, b, c , d, x]*/
a.push(y) /*cria mais uma posição no array e automaticamente define ela e coloca o valor y */
a.length /* checa o tamanho do array*/
a.sort() /* ordena */

for(var c in a){ /* repetição para variaveis compostas*/
		console.log(a[c])
}
```

> Um array é uma variável composta que tem vários elementos, cada elemento é composto por um valor e cada valor tem sua chave de identificação(indíce)

------

# Funções

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
