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
<h1>-<h6
```

Eles não foram criados na versão 5 do HTML e nem são específicos para semântica, mas servem para esse propósito. São utilizados para marcar a importância dos títulos, sendo **<h1>** o mais importante e **<h6>** o menos.



