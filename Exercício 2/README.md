# Exercício 2: HTML Semântico vs Blocos Genéricos

## Diferença entre `<div>` e HTML Semântico

A principal diferença entre usar blocos genéricos (como `<div>` e `<span>`) e usar elementos semânticos (como `<header>`, `<main>`, `<article>`) está no **significado** que cada tag carrega e em como os navegadores, motores de busca (SEO) e tecnologias assistivas interpretam a página.

* **Blocos Genéricos (`<div>` e `<span>`):** São tags "sem significado" (semântica neutra). Elas servem puramente como contêineres para agrupar elementos e aplicar estilos com CSS ou manipulações com JavaScript. O navegador não faz ideia do que tem dentro de uma `<div>` a menos que ele leia o conteúdo de texto.
* **HTML Semântico:** Introduzido com força no HTML5, utiliza tags que descrevem claramente o seu papel na estrutura do documento. Elas informam o significado do bloco tanto para o desenvolvedor quanto para a máquina. Isso melhora drasticamente a **acessibilidade** (ajudando leitores de tela para pessoas com deficiência visual) e o **SEO** (ajudando o Google a indexar melhor as partes importantes do seu site).

---

## Exemplo Prático

### 1. Estrutura com Blocos Genéricos (Má Prática)
No exemplo abaixo, tudo foi construído usando apenas divisões genéricas. Para entender o que cada parte faz, o navegador ou o desenvolvedor precisa ler as classes ou IDs.

```html
<div id="topo-do-site">
    <div class="menu-navegacao">
        <a href="#">Início</a>
        <a href="#">Sobre</a>
    </div>
</div>

<div id="conteudo-principal">
    <div class="bloco-noticia">
        <h2>Entendendo a Web</h2>
        <p>Aprender semântica é o primeiro passo para um código limpo.</p>
    </div>
</div>

<div id="rodape">
    <p>&copy; 2026 - Meu Site Genérico</p>
</div>

---
---

## 🏛️ Análise Teórica: Table-Based Layout (Parte 5)

### Por que o Table-Based Layout é uma técnica antiga?
Nos primórdios da web, o HTML não possuía tags de estrutura (como `main` ou `section`) e o CSS era extremamente limitado. Para conseguir alinhar elementos em colunas ou criar barras laterais fixas, os desenvolvedores usavam as propriedades de borda, alinhamento e largura das tabelas (`<table>`) para "forçar" o design visual da página.

### Dificuldades encontradas nesta adaptação:
1. **Rigidez e Responsividade:** Tabelas possuem larguras fixas por coluna. Adaptar essa estrutura para que ela fique bonita em telas de celulares modernos (responsividade) é extremamente complexo e ineficiente.
2. **Mistura de Conceitos:** O código mistura a apresentação visual (largura, cor de fundo, alinhamento direto nas tags) com os dados brutos, quebrando o princípio de separação de responsabilidades (HTML para estrutura, CSS para estilo).
3. **Acessibilidade Prejudicada:** Leitores de tela interpretam a tabela linha por linha, célula por célula. Ao ler um layout feito em tabela, o software diz ao usuário cego "Tabela com 3 linhas e 2 colunas", confundindo completamente a leitura do conteúdo real da página.

### Comparação com a Estrutura Semântica Moderna:
* **Tabelas para Layout:** Código poluído, difícil de ler, manutenção complexa (se você errar o fechamento de uma tag `</td>` ou `<tr>`, o design do site inteiro quebra) e sem significado semântico.
* **Semântica + CSS Moderno:** Código limpo e legível. Elementos como `Flexbox` e `CSS Grid` cuidam do posicionamento visual com poucas linhas no arquivo de estilo, mantendo o HTML puro, focado apenas no significado do conteúdo e completamente acessível.
