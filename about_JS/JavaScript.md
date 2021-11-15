# JavaScript

## Currying

É uma técnica de transformar uma função com vários parâmetros em uma função que recebe apenas um parâmetro e também uma nova função e assim sucessivamente.

## Hoisting

O código JavaScript é executado em duas fases. Primeiro, é feito o **parsing**, em que são vasculhadas declarações de variáveis, funções e parâmetros. Só depois é feito a execução de fato.

O efeito disso é que é como se as declarações de variáveis fossem levantadas para o topo da função ou arquivo em que estão definidas.

----

# Operadores

- Aritméticos

  ## Ordem de Precedência

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

  ```jsx
  média = 5
  média > 7 ? 'Aprovado':'Reprovado'
  ```
