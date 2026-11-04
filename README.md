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
