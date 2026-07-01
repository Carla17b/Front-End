# Documentação das Tags HTML Utilizadas

Este documento explica brevemente o papel de cada tag HTML aplicada no arquivo `index.html` desta etapa do exercício.

## Tags Estruturais

* `<!DOCTYPE html>`: Informa ao navegador que o documento está utilizando a versão mais recente do HTML (HTML5).
* `<html lang="pt-BR">`: A tag raiz que envolve todo o conteúdo da página. O atributo `lang="pt-BR"` define o idioma principal como português do Brasil.
* `<head>`: Contém os metadados da página (informações técnicas que não aparecem diretamente na tela para o usuário, como codificação de caracteres e título da aba).
* `<meta charset="UTF-8">`: Define a codificação de caracteres para UTF-8, garantindo que acentos e caracteres especiais do português sejam exibidos corretamente.
* `<meta name="viewport" content="...">`: Configura a página para ser responsiva, ajustando-se corretamente ao tamanho da tela de dispositivos móveis.
* `<title>`: Define o título da página que aparece na aba do navegador.
* `<body>`: Contém todo o conteúdo visível da página (textos, listas, títulos, imagens, etc.).

## Tags de Conteúdo

* `<h1>`: Define o título principal da página. Deve ser utilizado apenas uma vez por página para manter a boa semântica e SEO.
* `<h2>`: Define subtítulos secundários, ajudando a organizar o conteúdo em seções.
* `<h3>`: Define subtítulos de terceiro nível, criando uma hierarquia abaixo do `<h2>`.
* `<p>`: Utilizado para criar parágrafos de texto comum.
* `<ul>` *(Unordered List)*: Cria uma lista não ordenada (geralmente exibida com marcadores de "pontinhos").
* `<ol>` *(Ordered List)*: Cria uma lista ordenada (exibida numericamente, ideal para passos sequenciais).
* `<li>` *(List Item)*: Representa cada item individual dentro de uma lista (`<ul>` ou `<ol>`).