# Portfólio Pessoal | Guilherme Oliveira Santos

**Aluno:** Guilherme Oliveira Santos
**Curso:** Técnico em Desenvolvimento de Sistemas (ETEC Itaquera II)

## Descrição do portfólio

Site pessoal que apresenta o Guilherme como estudante de Desenvolvimento de Sistemas e Técnico em Mecânica (Operador CNC II). A página dá mais destaque à área de Desenvolvimento de Sistemas e mostra também a experiência na indústria, que traz precisão e atenção aos detalhes para a programação.

## Tecnologias utilizadas

- HTML5
- CSS3
- Bootstrap 5.3 (via CDN)
- JavaScript
- Git e GitHub
- GitHub Pages

## Repositório e site

Repositório: https://github.com/oliveirasantosguilherme5-developer/portfolio

## Link do site publicado

https://oliveirasantosguilherme5-developer.github.io/portfolio/

## Como o projeto funciona

O site é uma página única, dividida em seções:

- **Perfil:** apresentação inicial com nome, área de atuação e um cartão de código com resumo.
- **Sobre mim:** texto sobre a trajetória em tecnologia e mecânica.
- **Habilidades:** etiquetas com as habilidades, separadas em Desenvolvimento de Sistemas e Mecânica (recurso novo).
- **Projetos:** cartões com os programas em Python do GitHub (calculadora de consumo de energia, desconto progressivo, consumo de água, pesquisa de satisfação e nível de água), o próprio portfólio e a experiência em usinagem, usando o grid e os cards do Bootstrap.
- **Formação e experiência:** linha do tempo com cursos e empregos.
- **Contato:** e-mail, telefone, LinkedIn e localização.

O menu de navegação usa a navbar do Bootstrap, com links de âncora para cada seção. No celular ele vira um menu recolhível e fecha sozinho depois do clique. O Scrollspy do Bootstrap destaca no menu a seção que está na tela.

## Recurso novo: seção de habilidades com efeitos de hover

Foi adicionada uma seção nova de **Habilidades**, que não existia no projeto feito em aula. Ela lista as habilidades em etiquetas, em dois grupos: Desenvolvimento de Sistemas (azul) e Mecânica e indústria (cinza). Ao passar o mouse sobre uma etiqueta, ela sobe levemente, ganha sombra e muda para a cor de destaque.

Também foram acrescentados efeito de elevação nos cartões de projetos, uma linha do tempo de formação e experiência e o fechamento automático do menu no celular.

### Como foi implementado

- **HTML:** cada grupo é uma lista (`ul.skill-list`) com a classe `d-flex flex-wrap gap-2` do Bootstrap, e cada habilidade é um `li.skill-tag`.
- **CSS:** `.skill-tag` tem bordas arredondadas e `transition` para `transform`, `background-color` e `box-shadow`. No `:hover`, a etiqueta recebe `translateY(-3px)`, sombra e a cor de destaque. Para quem prefere menos movimento, `prefers-reduced-motion` desativa a transição.
- **JavaScript (`script.js`):** fecha o menu recolhível no celular quando um link é clicado, usando a classe `Collapse` do Bootstrap.

## Estrutura de arquivos

```
portfolio/
├── index.html
├── style.css
├── script.js
└── README.md
```

## Como publicar no GitHub Pages

1. Crie um repositório público chamado `portfolio`.
2. Envie os quatro arquivos para a raiz do repositório.
3. Em **Settings > Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
4. Aguarde alguns minutos e acesse o link gerado.
