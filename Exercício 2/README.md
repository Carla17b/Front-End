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
