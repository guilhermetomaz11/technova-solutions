
# 🗓️ Parte 2: Roteiro de Execução e Atividades Específicas por Sprint

O desenvolvimento do portal da TechNova será realizado em **2 Sprints**. Todas as especificações técnicas do que você deve construir estão detalhadas nas tarefas de cada Sprint abaixo:

---

## 🛠️ SPRINT 1: Planejamento, Estrutura Semântica & Marcação HTML5
**Foco da Sprint:** Desenhar o layout, organizar a arquitetura de pastas e construir **toda a estrutura semântica e funcional em HTML5** (`index.html`), validando o código no W3C antes de aplicar qualquer estilo visual.

### 📌 Atividades Específicas da Sprint 1:

#### [ ] Tarefa 1.1 – Planejamento Visual (Wireframe)
- Ler o Briefing da TechNova e desenhar o **Wireframe de Baixa Fidelidade** (croqui à mão no papel) ou **Média Fidelidade** (no Figma).
- Delimitar claramente no rascunho a distribuição espacial do Cabeçalho, Conteúdo Principal (Hero, Sobre, Serviços, Blog, Contato) e Rodapé.
- Salvar uma foto ou exportação do wireframe na pasta do projeto (`wireframe.png`).

#### [ ] Tarefa 1.2 – Arquitetura de Pastas, Esqueleto HTML5 e Metadados de SEO
- Criar a pasta raiz do projeto (`technova-seu-nome/`) com as subpastas `css/` e `img/` (nomes padronizados em letras minúsculas, sem espaços ou acentos).
- Criar o arquivo `index.html` com a estrutura fundamental: `<!DOCTYPE html>`, `<html lang="pt-BR">`, `<head>`, `<title>` e `<body id="topo">`.
- Configurar no `<head>` os metadados obrigatórios:
  - `<meta charset="UTF-8">`
  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  - `<meta name="description" content="Descrição institucional da TechNova Solutions para SEO">`
- Documentar todas as seções do código-fonte utilizando **comentários estruturados** (`<!-- Seção X -->`).

#### [ ] Tarefa 1.3 – Marcação do Cabeçalho (`<header>`) e Hero Section (`<main>`)
- **No `<header>`:** Inserir a marca da TechNova e estruturar o menu de navegação dentro da tag `<nav>` utilizando lista não ordenada (`<ul>` e `<li>`) com links de âncora internos (`href="#inicio"`, `#sobre`, `#servicos`, `#blog`, `#contato`).
- **Na Hero Section (`<section id="inicio" class="hero">`):**
  - Criar o título de impacto principal da startup utilizando a única tag `<h1>` da página, acompanhada de parágrafo descritivo (`<p>`) e botão de Chamada para Ação (*Call to Action - CTA*).
  - Estruturar o container da **Galeria / Carrossel de Destaques** utilizando tags semânticas `<figure>` e `<figcaption>` para pelo menos 3 serviços/soluções em destaque.

#### [ ] Tarefa 1.4 – Marcação das Seções "Sobre Nós & Equipe" e "Catálogo de Serviços"
- **Na Seção Sobre Nós (`<section id="sobre">`):**
  - Estruturar o texto da história da startup e criar os 3 blocos de **Missão, Visão e Valores** respeitando a hierarquia de títulos (`<h2>`, `<h3>`) e destaques semânticos (`<strong>`, `<em>`).
  - Estruturar a **Grade de Especialistas** usando tags `<article>` para pelo menos **3 membros da equipe** (contendo tag `<img>` com `alt` descritivo, nome `<h4>`, cargo e resumo).
- **Na Seção de Serviços (`<section id="servicos">`):**
  - Criar a lista/grade de soluções tecnológicas da TechNova (mínimo de 3 cards `<article>`).
  - Construir a **Tabela Comparativa de Planos (`<table>`)** contendo obrigatoriamente:
    1. Legenda `<caption>` e agrupamentos `<thead>`, `<tbody>` e `<tfoot>`.
    2. Cabeçalhos acessíveis `<th scope="col">` e `<th scope="row">`.
    3. Pelo menos **uma mesclagem de colunas (`colspan`)** e **uma mesclagem de linhas (`rowspan`)**.

#### [ ] Tarefa 1.5 – Marcação da Seção "Blog & Central de Notícias" (`<section id="blog">`)
- Criar um campo visual de pesquisa de artigos (`<input type="search" placeholder="Pesquisar artigos...">`) e navegação por categorias.
- Estruturar pelo menos **3 artigos tecnológicos** usando a tag `<article>`, contendo: container de imagem de capa, etiqueta (`<span>`) de categoria, data de publicação (`<time>`), autor, título (`<h3>`), resumo e link *"Ler artigo completo"*.

#### [ ] Tarefa 1.6 – Marcação da Seção "Contato & Localização" e do Rodapé (`<footer>`)
- **Na Seção de Contato (`<section id="contato">`):**
  - Construir o **Formulário Corporativo (`<form>`)** agrupado com `<fieldset>` e `<legend>`, garantindo que **todos os campos possuam `<label for="...">` vinculado ao `id` do respectivo campo** e validação nativa:
    1. Nome Completo (`<input type="text" id="nome" required placeholder="...">`)
    2. E-mail Institucional (`<input type="email" id="email" required placeholder="...">`)
    3. Telefone / WhatsApp (`<input type="tel" id="telefone" required placeholder="...">`)
    4. Assunto do Atendimento (`<select id="assunto" required>` com opções `<option>`)
    5. Mensagem Detalhada (`<textarea id="mensagem" rows="5" required placeholder="..."></textarea>`)
    6. Aceite de Privacidade (`<input type="checkbox" id="aceite" required>`)
    7. Botão de Envio (`<button type="submit">Enviar</button>`)
  - Estruturar ao lado um bloco `<aside>` com `<address>` contendo os dados institucionais e a incorporação visual do mapa/localização da empresa (`<iframe>` ou imagem de mapa).
- **No Rodapé (`<footer>`):** Inserir direitos autorais, menu de links úteis, área de redes sociais e o link de âncora `<a href="#topo">↑ Voltar ao Topo</a>`.

#### [ ] Tarefa 1.7 – Publicação Inicial no GitHub Pages e Validação W3C da Sprint 1
- Criar o repositório público no GitHub (`technova-solutions`), enviar a estrutura inicial da Sprint 1 e ativar o **GitHub Pages** (`Settings > Pages > Branch: main`).
- Copiar a URL pública gerada (`https://seu-usuario.github.io/technova-solutions/`) e validá-la diretamente no [W3C Markup Validation Service (Validate by URI)](https://validator.w3.org/), corrigindo todos os erros de sintaxe ou semântica antes de iniciar a Sprint 2.