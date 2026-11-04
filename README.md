# MathTech Web

## Matemática Aplicada à Informática

O MathTech Web é um projeto educacional que relaciona matemática, informática, design de interfaces e desenvolvimento Web. A versão final reúne seis páginas HTML, uma folha de estilos compartilhada e recursos interativos implementados com JavaScript.

Este documento descreve os arquivos presentes em `MathTech_Atividade_Final.zip`.

## Objetivos

- Apresentar fundamentos matemáticos relacionados à computação.
- Explorar sistemas de numeração e operações lógicas por meio de exemplos e ferramentas interativas.
- Aplicar HTML5, CSS3 e JavaScript em um site acadêmico.
- Organizar conteúdos com navegação, listas, tabelas, formulários e recursos visuais.
- Manter uma identidade visual compartilhada entre as páginas.

## Páginas do site

| Página | Arquivo | Conteúdo |
|---|---|---|
| Início | `index.html` | Apresentação, aplicações da matemática, tópicos da disciplina e conteúdo programático |
| Projeto | `sobre.html` | Proposta, objetivos e etapas de desenvolvimento |
| Sistemas | `sistemas.html` | Bases decimal, binária, octal e hexadecimal, com tabela comparativa |
| Multimídia | `multimidia.html` | Capa da série e acesso externo a vídeo e playlist no YouTube |
| Inter-Lab | `interlab.html` | Conversor de bases, demonstração lógica e quiz |
| Cadastro | `cadastro.html` | Formulário demonstrativo com campos e validações nativas do HTML5 |

## Funcionalidades

### Página inicial

Apresenta aplicações da matemática em algoritmos, inteligência artificial, criptografia e programação. Inclui navegação por âncoras, lista de tópicos, tabela de organização dos conteúdos em quatro bimestres e atalhos para o laboratório e a multimídia.

### Sistemas de numeração

Apresenta as bases e os símbolos de cada sistema, exemplos e aplicações.

| Sistema | Base | Símbolos | Exemplo |
|---|---:|---|---|
| Decimal | 10 | 0 a 9 | 26₁₀ |
| Binário | 2 | 0 e 1 | 11010₂ |
| Octal | 8 | 0 a 7 | 32₈ |
| Hexadecimal | 16 | 0 a 9 e A a F | 1A₁₆ |

Os quatro exemplos representam o mesmo valor em bases diferentes.

### Laboratório interativo

#### Conversor

- Converte uma entrada decimal para binário, octal e hexadecimal.
- Exibe também o valor decimal convertido.
- Aceita valores que resultem em inteiros não negativos seguros para o tipo `Number`, conforme `Number.isSafeInteger()`.
- Apresenta mensagens de validação.
- Permite converter pelo botão ou pela tecla Enter.
- Possui botão para limpar a entrada e os resultados.

#### Lógica matemática

Permite alternar as proposições P e Q e observar os resultados de:

- P E Q — AND.
- P OU Q — OR.
- NÃO P — NOT.

Os resultados são atualizados ao alterar os controles.

#### Quiz

Apresenta cinco questões de múltipla escolha sobre sistemas de numeração, lógica, símbolo de pi, conjuntos e combinatória.

Inclui correção, pontuação de 0 a 5, destaque de alternativas e botão para reiniciar. É uma ferramenta de autoestudo: o gabarito está no HTML e as pontuações não são armazenadas.

### Multimídia

A página utiliza a imagem `img/serie-thumb.png` como capa da série e oferece dois acessos externos:

- Capa: https://youtu.be/EYyfI9s_CMM
- Botão da playlist: https://www.youtube.com/playlist?list=PLfN8Om1CaVfU

A série é apresentada na interface como um conjunto de dez aulas. A versão final não contém player incorporado: os links abrem o YouTube em outra aba. A disponibilidade e a composição desses recursos externos não foram verificadas nesta documentação.

### Formulário de cadastro

Inclui nome, nascimento, e-mail, telefone, cidade, estado, senha, confirmação de senha e aceite dos termos.

Utiliza `label`, `fieldset`, `legend`, `required`, `minlength`, `autocomplete` e tipos específicos de entrada. Possui botões para enviar e limpar o formulário.

> O cadastro é demonstrativo. O formulário usa `action="#"` e `method="post"`, sem integração com backend, banco de dados ou autenticação. Não há comparação entre senha e confirmação. Não utilize dados pessoais ou senhas reais nos testes.

## Estrutura da versão final

```text
MathTech_Atividade_Final/
├── cadastro.html
├── index.html
├── interlab.html
├── multimidia.html
├── sistemas.html
├── sobre.html
├── css/
│   └── estilo.css
└── img/
    ├── capa-mathtech.jpg
    ├── hero-home.jpg
    ├── logo.svg
    └── serie-thumb.png
```

O ZIP também contém a pasta `.git`, omitida da árvore por não fazer parte dos recursos exibidos pelo site. Este README é um documento adicional e não estava presente no compactado original.

## Tecnologias

| Tecnologia | Aplicação |
|---|---|
| HTML5 | Estrutura, navegação, conteúdo, tabelas e formulários |
| CSS3 | Identidade visual, componentes, transições e adaptação de layout |
| JavaScript | Conversão de bases, operações lógicas e correção do quiz |

O projeto não utiliza framework, gerenciador de pacotes ou etapa de compilação. O JavaScript do laboratório está incorporado em `interlab.html`.

## Interface e responsividade

A interface compartilha cabeçalho, menu, rodapé, tipografia e paleta em azul-marinho, azul, ciano e tons claros.

O CSS combina Flexbox e CSS Grid e inclui regras de adaptação em 920px e 650px. Os componentes utilizam cards, bordas arredondadas, sombras e efeitos de interação.

## Evolução apresentada no projeto

A página `sobre.html` descreve quatro etapas:

1. Figma: prototipação visual e organização do conteúdo.
2. Lovable + IA: transformação do protótipo em aplicação interativa por engenharia de prompts.
3. HTML5 e CSS3: reprodução acadêmica em páginas tradicionais, com JavaScript no laboratório.
4. GitHub Pages: etapa de publicação Web, associada ao uso de controle de versão.

## Como executar a versão final

1. Extraia `MathTech_Atividade_Final.zip`.
2. Abra a pasta `MathTech_Atividade_Final`.
3. Abra `index.html` em um navegador com JavaScript habilitado.
4. Utilize o menu para navegar entre as páginas.

No Git Bash do Windows, aberto na pasta extraída:

```bash
explorer.exe index.html
```

Não é necessário instalar dependências. Os recursos do laboratório são processados no navegador; os links para o YouTube exigem acesso à internet.

## Escopo e observações

- O site é uma aplicação estática de finalidade acadêmica.
- O formulário não realiza cadastro de usuários.
- Não há persistência de resultados ou pontuações.
- Após uma tentativa inválida no conversor, os resultados anteriores permanecem visíveis.
- Alterar uma alternativa após corrigir o quiz não atualiza a pontuação até uma nova correção.
- A presença de regras responsivas não substitui testes em diferentes dispositivos.
- A versão publicada no GitHub Pages depende da configuração do repositório; não foi confirmada sua equivalência ao ZIP final.

## Autoria

Cosme Vinicius Menezes de Oliveira.

Projeto acadêmico MathTech — 2026.

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
