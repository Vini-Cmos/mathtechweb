# MathTech Web 🚀

![MathTech](img/capa-mathtech.jpg)

## Matemática Aplicada à Informática

O **MathTech Web** é um projeto educacional desenvolvido para a disciplina **Web Design**, do curso Técnico em Desenvolvimento de Sistemas.

O projeto apresenta conceitos matemáticos fundamentais utilizados na computação, com destaque para sistemas de numeração, lógica matemática e suas aplicações na área de tecnologia.

---

# Objetivo do projeto

O MathTech Web busca integrar:

- Design de interfaces;
- Prototipação;
- Desenvolvimento Web;
- Conteúdo educacional;
- Controle de versão;
- Publicação de sites.

---

# Processo de desenvolvimento

## 1. Prototipação no Figma 🎨

O projeto teve início com a criação de um protótipo visual no Figma.

Nesta etapa foram definidos:

- identidade visual;
- organização das páginas;
- hierarquia dos conteúdos;
- experiência do usuário (UX);
- elementos gráficos;
- distribuição das informações.

O protótipo serviu como referência para as etapas seguintes do projeto.

---

## 2. Desenvolvimento no Lovable 🤖

Após a criação do protótipo, foi desenvolvida uma versão interativa utilizando a plataforma **Lovable**.

Nesta etapa foram trabalhados:

- estrutura visual;
- organização dos conteúdos;
- navegação;
- laboratório interativo;
- experiência do usuário;
- integração de recursos educacionais.

Aplicação desenvolvida no Lovable:

https://mathtechmatematicaplicadainformtica.lovable.app/

---

## 3. Desenvolvimento Web com HTML5, CSS3 e JavaScript 💻

Para a disciplina Web Design, o projeto foi adaptado para uma estrutura tradicional de desenvolvimento Web.

Foram utilizados:

- HTML5;
- CSS3;
- JavaScript;
- páginas HTML separadas;
- folha de estilos compartilhada;
- estrutura organizada de arquivos;
- layout responsivo.

A versão atual mantém a identidade visual definida no projeto original e reproduz, em HTML, CSS e JavaScript, os principais recursos presentes no protótipo e na versão desenvolvida no Lovable.

---

# Estrutura atual do projeto

```text
mathtechweb/
│
├── index.html
├── sobre.html
├── sistemas.html
├── multimidia.html
├── interlab.html
├── cadastro.html
│
├── css/
│   └── estilo.css
│
└── img/
    ├── logo.svg
    ├── capa-mathtech.jpg
    ├── hero-home.jpg
    └── serie-thumb.png
```

---

# Páginas do site

## Início

Apresenta o projeto **Matemática Aplicada à Informática**, seus principais conteúdos e o acesso às demais áreas do site.

## Projeto

Apresenta o objetivo do MathTech, sua proposta educacional e as principais etapas de desenvolvimento.

## Sistemas

Apresenta os principais sistemas de numeração utilizados na computação:

- Decimal;
- Binário;
- Octal;
- Hexadecimal.

A página também possui uma tabela comparativa com bases, símbolos, exemplos e aplicações.

## Multimídia

Apresenta a série educacional **Matemática Aplicada à Informática — Sistemas de Numeração**.

A página utiliza a capa da série e disponibiliza acesso direto à playlist oficial no YouTube.

Playlist:

https://www.youtube.com/playlist?list=PLfN8Om1CaVfU

## Inter-Lab

O **Inter-Lab** é o laboratório interativo do MathTech.

Ele reúne três recursos:

- conversor de sistemas numéricos;
- demonstração de lógica matemática;
- quiz rápido.

O conversor permite transformar um número decimal em:

- binário;
- octal;
- hexadecimal.

A demonstração de lógica permite alterar os valores das proposições **P** e **Q** e observar os resultados das operações:

- AND;
- OR;
- NOT.

O quiz apresenta questões relacionadas aos conteúdos estudados no projeto e informa a pontuação obtida.

## Cadastro

Apresenta um formulário HTML5 com campos comuns de cadastro, como:

- nome completo;
- data de nascimento;
- e-mail;
- telefone;
- cidade;
- estado;
- senha;
- confirmação de senha;
- aceite dos termos.

---

# Evolução do Projeto — Atividade Avaliativa 5

Nesta etapa, o MathTech Web foi ampliado com novos recursos e melhorias de interface.

Foram aplicados conceitos trabalhados na disciplina Web Design, incluindo:

- navegação entre páginas;
- HTML5 semântico;
- CSS externo;
- formulários HTML5;
- tabelas;
- multimídia;
- responsividade;
- organização de arquivos;
- padronização visual;
- interatividade com JavaScript.

Também foi realizada a unificação visual das páginas para que todas façam parte de um único site, mantendo:

- mesma paleta de cores;
- mesma tipografia;
- mesmo cabeçalho;
- mesmo menu de navegação;
- mesmo padrão de cards e botões;
- mesmo rodapé;
- mesma identidade visual.

---

# Identidade visual

A interface utiliza principalmente:

- azul-marinho;
- azul tecnológico;
- branco;
- cinza claro;
- detalhes em ciano.

O objetivo visual é manter uma aparência:

- limpa;
- organizada;
- tecnológica;
- acadêmica;
- responsiva.

---

# Publicação e controle de versão

O projeto utiliza **Git** para controle de versão e **GitHub** para armazenamento do código-fonte.

Repositório:

https://github.com/Vini-Cmos/mathtechweb

Site publicado com GitHub Pages:

https://vini-cmos.github.io/mathtechweb/

---

# Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Git
- GitHub
- GitHub Pages
- Figma
- Lovable

---

# Autor

**Cosme Vinicius Menezes de Oliveira**

Projeto desenvolvido em 2026 para a disciplina **Web Design** do curso Técnico em Desenvolvimento de Sistemas.


## Atualizações específicas de css/estilo.css

Esta seção registra as diferenças da folha de estilos da versão final em relação à versão anterior consultada na branch `master`. Ela documenta alterações existentes, sem modificar o CSS.

### Padronização global

- Inclusão de `margin: 0` e `padding: 0` no seletor universal, mantendo `box-sizing: border-box`.
- Remoção global do sublinhado dos links com `text-decoration: none`.
- Criação de `--shadow-hover` para reutilizar a sombra de destaque.

### Cabeçalho e navegação

- Ajuste da sombra do cabeçalho.
- Inclusão de padding horizontal em `.nav-wrap` no layout maior.
- Efeito de deslocamento na marca em hover.
- Inclusão de sombra no símbolo da marca.
- Transição de cor nos links do menu.
- Indicador inferior animado nos links em hover e no item ativo.

### Cards e botões

- Inclusão de transições de transformação e sombra.
- Deslocamento vertical de cards e botões em hover.
- Aplicação da variável `--shadow-hover` aos cards.
- Ajustes de tipografia e espaçamento em `.topic-card`.
- Inclusão de estado de hover para `.btn-outline`.

### Layouts

- Inclusão da classe `.container-flex`, com quebra de linha e espaçamento entre componentes.
- Inclusão de regras de distribuição dos cards e adaptações em 920px e 650px.
- Manutenção dos layouts existentes com CSS Grid.

> `.container-flex` está declarada no CSS, mas não aparece nos HTMLs da versão final. Sua inclusão não significa que os conjuntos de cards existentes tenham sido convertidos de Grid para Flexbox.

### Tabelas e elementos de apoio

- Inclusão de bordas arredondadas, recorte de conteúdo e sombra nas tabelas.
- Transição e destaque das linhas em hover.
- Inclusão de sombra nos indicadores numéricos da linha do tempo.
- Efeito de hover nas tags.

### Apresentação e multimídia

- Inclusão de `pointer-events: none` na sobreposição `.hero-home::after`.
- Efeitos de deslocamento e sombra em `.video-shell`.
- Ampliação da imagem em hover.
- Animação de escala e mudança de fundo no símbolo de reprodução da capa.

Esses efeitos são visuais: não implementam um player de vídeo.

### Formulários

- Ampliação da estilização de `.form-card`, com fundo, bordas arredondadas, sombra e padding.
- Inclusão de regras para `.form-group`, `.checkbox-group` e `.form-actions`.
- Substituição da regra genérica de inputs por seletores específicos de texto, e-mail, telefone, senha e data, além de `select` e `textarea`.
- Inclusão de transições de borda e sombra.
- Ajustes de espaçamento e cursor em checkboxes e radios.
- Regras responsivas adicionais para o cartão e as ações do formulário.

> `.form-group`, `.checkbox-group` e `.form-actions` não aparecem nos HTMLs da versão final. O formulário existente utiliza `.actions`.

> O campo `type="number"` do conversor ficou fora do novo bloco específico de estilização dos campos. Esta observação documenta a versão entregue; nenhuma correção foi aplicada.

### Laboratório e quiz

- Inclusão de bordas e efeito de hover nas caixas de resultados.
- Ajuste do tamanho da fonte dos resultados.
- Inclusão de bordas nos blocos das proposições.
- Estilização adicional dos contêineres das perguntas.
- Ajuste de espaçamento dos enunciados.
- Transições e destaque de hover nas alternativas.

### Organização e responsividade

- Manutenção dos breakpoints de 920px e 650px, com regras adicionais para as novas classes.
- Remoção de comentários explicativos da versão anterior.
- Alterações de indentação e espaços em branco em grande parte do arquivo.

Nem toda linha alterada no diff representa uma mudança visual. As alterações documentadas foram identificadas por leitura do código, sem testes completos de renderização em diferentes navegadores e dispositivos.
