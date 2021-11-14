# Conceitos Básicos de HTML

## Abertura e Fechamento de tag e o que as compõe:

![Estrutura HTML](https://i.imgur.com/CDRx3va.png)

``` html
<tipoDeElemento atributo="titulo">Conteúdo</tipoDeElemento
```

#### Estrutura Básica:

```html
<!DOCTYPE html>
<html> <!---abertura da Tag do elemento HTML--->
<head> <!---Informações que o navegador possa necessitar--->
    <meta>
    <title></title><!---Título da Aba--->
</head>
<body><!---Conteúdo da Página--->
</body>
</html>
```

#### Semântica:

**A semântica nos permite descrever mais precisamente o nosso conteúdo**

```html
<section>
```

Representa uma seção genérica de conteúdo quando não houver um elemento mais específico para isso.

```html
<header>
```

É o cabeçalho da página ou de uma seção da página e normalmente contém logotipos, menus, campos de busca.

```html
<article>
```

Representa um conteúdo independente e de maior relevância dentro de uma página, como um post de blog, uma notícia em uma barra lateral ou um bloco de comentários. Um article pode conter outros elementos, como header, cabeçalhos, parágrafos e imagens.

```html
<aside>
```

É uma seção que engloba conteúdos relacionados ao conteúdo principal, como artigos relacionados, biografia do autor e publicidade. Normalmente são representadas como barras laterais.

```html
<footer>
```

Esse elemento representa o rodapé do conteúdo ou de parte dele, pois ele é aceito dentro de vários elementos, como article e section e até do body. Exemplos de conteúdo de um <footer> são informações de autor e *links* relacionados.

```html
<h1>-<h6>
```

Eles não foram criados na versão 5 do HTML e nem são específicos para semântica, mas servem para esse propósito. São utilizados para marcar a importância dos títulos, sendo **h1** o mais importante e **h6** o menos.

```html
<p></p>
```

Para textos maiores e mais densos usamos o elemento p, que representa um parágrafo, porém não suporte apenas texto, podemos adicionar imagens, código, vídeos e outros tipos de conteúdo dentro dele.

```html
<a></a>
```

Um outro elemento interessante e extremamente necessário na web é o ***a*** - que significa anchor/âncora, ele representa um hyperlink, é ele que interliga vários conteúdos e páginas na web.

Os atributos principais são o ***href e o target***.

**href** representa o hyperlink para onde a anchor aponta, pode ser uma página de site, um e-mail, até mesmo telefone.

***OBS***: *os dois últimos precisam dos prefixos mailto: e tel:, respectivamente.*

**target** serve para abrir os links em outra aba do navegador usando o valor _blank.

#### Imagens

A web também é feita de imagens e para representá-las temos o elemento

```html
<img>
```

O elemento img é bem simples, contendo apenas 2 atributos próprios, o *src* e o *alt*.

O src é obrigatório e guarda o caminho para a imagem que você quer mostrar na página.

O alt não é obrigatório mas é altamente recomendado por melhorar a acessibilidad	e, ele mostra a descrição da imagem caso ela não carregue e leitores de tela usam esse atributo para descrever a imagem para o usuário saber o que ela significa.

#### Listas

Listas servem para agrupar uma coleção de itens, como uma lista de ingredientes ou, como será no nosso caso, uma lista com contatos.

##### O elemento ul

```html
<ul></ul>
```

O elemento ***ul*** cria uma lista não ordenada, onde a ordem dos elementos não é importante, e é representada com pontos, círculos ou quadrados.

```html
<ol></ol>
```

O ***ol*** serve para criar listas ordenadas, nessas a ordem importa, portanto elas são representadas com números, algarismos romanos ou letras.

```html
<li></li>
```

E o elemento li é um item dentro de uma dessas listas. Um ***li*** pode conter vários tipos de conteúdos, como parágrafos, imagens e até outras listas.