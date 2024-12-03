# 🚀 Replicando o Layout do YouTube - Exercício DevQuest
## 👋 Apresentação

Olá, sou Miguel, um aspirante a Desenvolvedor Web, e este projeto faz parte da minha jornada no curso de Formação de Desenvolvedor Web Fullstack (DevQuest - Dev em Dobro). Este exercício integra o módulo "Exercício CSS Avançado Parte 3 - Grid" e representa o maior desafio até o momento em minha formação.

Este README serve como um diário técnico, onde compartilho as lições aprendidas, revisões realizadas e os diversos desafios enfrentados durante o processo. O foco principal deste exercício foi aplicar conhecimentos de Grid CSS, com o uso de Flexbox como complemento, para replicar um layout inspirado no YouTube. 🎯

## 💻 Explicação do Projeto
O objetivo deste projeto foi testar meus conhecimentos em Grid CSS e, em segundo plano, Flexbox. A proposta era criar um layout semelhante ao do YouTube, utilizando um design fornecido no Figma para os alunos. Vale destacar que a página não é responsiva e o foco do projeto não foi esse.

**A aparência visual deste projeto consiste em:**

🖼️ Um layout dividido em duas colunas, com um destaque visual para um vídeo maior no lado esquerdo e um conjunto de vídeos menores no lado direito.
- **📺 Área de destaque:**

    - Um espaço retangular grande (540x220 pixels) no topo da coluna esquerda, reservado para o vídeo principal, acompanhado pelo título em negrito, um contador de visualizações e uma breve descrição do conteúdo logo abaixo.
    - A descrição utiliza texto fictício ("Lorem ipsum") para ilustrar o espaço dedicado às informações adicionais.

- 🎥 **Coluna lateral de vídeos menores**:
    - No lado direito, há uma área organizada com três vídeos menores empilhados verticalmente. Cada vídeo possui:
        - Uma miniatura quadrada (100x70 pixels) para a prévia;
        - Um título maior em destaque, seguido pelo nome do autor, número de visualizações e a data de publicação (Ex.: "há 3 semanas").
    - Acima desta seção, há um espaço publicitário retangular (270x60 pixels) que ocupa a parte superior direita.
    
💡 A estrutura do projeto busca oferecer uma hierarquia visual clara, destacando o vídeo principal ao mesmo tempo em que organiza os conteúdos adicionais. **Veja abaixo uma imagem do projeto finalizado:**


  <div>
  <img src="./src/images/project-final.jpeg" alt="Print do resultado final da página" width="100%">
</div>

## 🛠️ Linguagens Utilizadas
<div style="display: inline_block"><br>
  <img align="center" alt="HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="Markdown" height="40" width="50" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/markdown/markdown-original.svg" />
</div>

## 🏗️ Estrutura do Grid Layout
A estrutura do layout foi planejada de forma cuidadosa antes mesmo de iniciar a codificação. Durante a elaboração do código HTML, já considerava como a marcação seria distribuída no Grid Layout. Optei por usar uma tag `<main>` como contêiner principal, que abriga quatro elementos filhos diretos: `<div>`, `<header>`, `<section>` e `<aside>`. Os dois primeiros elementos formam a coluna esquerda do design, enquanto os dois últimos representam a coluna direita.

A estrutura do Grid foi criada utilizando a propriedade `display: grid;` e configurada através da propriedade `grid` (forma abreviada, de modo a reduzir a 
verbosidade do código). A grade é composta por duas colunas e três linhas: a primeira coluna é destinada à área do vídeo em destaque e suas informações, enquanto a segunda coluna abriga a propaganda e os vídeos sugeridos. As linhas no eixo vertical, embora não representem áreas fixas, desempenham um papel importante na disposição irregular do layout, garantindo que a distribuição dos elementos atenda ao design proposto no Figma.

**Abaixo, é possível observar a divisão do layout no Grid, demonstrada utilizando a ferramenta Chrome DevTools:**

  <div>
  <img src="./src/images/grid_layout.png" alt="Print da estrutura bidimensional em grade do projeto" width="100%">
</div>

## 🧗‍♂️ Desafios Enfrentados
Este projeto foi, sem dúvidas, o mais desafiador que enfrentei até agora na minha jornada de aprendizado em desenvolvimento web. Por ser minha primeira experiência prática com Grid CSS, tive dificuldade inicialmente em visualizar como a estrutura HTML se comportaria ao ser organizada em um layout bidimensional. Isso tornou a fase inicial de planejamento e codificação do HTML mais complicada.

Ao avançar para a configuração do Grid em CSS, acabei travando ao tentar organizar os elementos no layout. A falta de experiência inicial me deixou frustrado, e houve momentos em que pensei que não conseguiria concluir o projeto sozinho. Para superar esses obstáculos, busquei materiais externos, como vídeos nos canais do YouTube "Fernanda Kipper | Dev" e "TreinaWeb", o que me ajudou a consolidar melhor os conceitos de Grid CSS.

Com esse novo conhecimento, voltei ao projeto, ajustei minha estrutura HTML para facilitar o trabalho com o Grid e utilizei ferramentas tradicionais, como papel e caneta, para mapear a disposição dos elementos. Isso trouxe mais clareza e confiança, permitindo que eu estruturasse o layout de forma funcional. Após essa reorganização, o desenvolvimento fluiu bem, e consegui replicar de forma idêntica o design proposto no Figma.

Quanto ao uso de Flexbox, sua aplicação foi bem mais fácil e rápida, e não apresentou grandes desafios nem exigiu muito esforço. 


## 📚 O Que Aprendi com Este Desafio
Este projeto foi ótimo para praticar o CSS Grid, onde pude consolidar e expandir meu conhecimento sobre a manipulação de layouts em grade. A prática permitiu não apenas a memorização das propriedades do Grid, mas também uma compreensão detalhada das regras de espaçamento entre elementos, como o comportamento das margens e como o layout em grade controla suas áreas.

Revisitei anotações passadas sobre a propriedade `box-sizing: border-box;`, que simplifica o cálculo das dimensões de elementos ao incluir o padding e a borda na largura e altura especificadas. Também aprendi maneiras eficientes de estilizar elementos filhos de um contêiner, utilizando seletores como o universal (*), as pseudo-classes :is(), :where() e :scope, cada um com seus usos específicos em relação à especificidade.

Assistindo à resolução do exercício proposta pelo curso, identifiquei redundâncias no meu código, como declarações desnecessárias de `width` e `height`, e entendi como o CSS Grid já gerencia essas dimensões de forma eficiente. Além disso, absorvi um método mais fácil e prático para configurar áreas do grid: utilizar unidades proporcionais como fr e elementos como referência estrutural (neste caso, o `.propaganda`). Essa abordagem reduz a necessidade de cálculos manuais.

Essas lições, aliadas à prática e às revisões, aprimoraram significativamente minha habilidade como desenvolvedor e posso afirmar que estou pronto para desafios maiores envolvendo o CSS Grid.

## Minhas fontes de consulta para o cumprimento deste exercício
1. __Resumo das aulas do módulo "CSS Avançado Parte 3" - Grid, do curso DevQuest da Dev em Dobro.__  
[Link para a Página do Notion Referente ao Resumo deste Módulo](https://gigantic-chef-a6f.notion.site/CSS-avan-ado-Parte-3-Grid-151cd10b93ab80bd9cbfc38a31c81b0f/ "Página do Notion - Resumo CSS Avançado Parte 3 - Grid")

2. __Vídeos complementares no YouTube, que procurei para reforçar minha habilidade no uso de Grid Layout.__  
[Link para a Página do Notion onde consta os Vídeos  Complementares Assistidos e as Anotações sobre eles](https://gigantic-chef-a6f.notion.site/Conte-do-Extra-Aprimorando-meu-conhecimento-em-Grid-151cd10b93ab80b290a1c54463fa57d6/ "Página do Notion - Conteúdo Extra: Aprimorando meu conhecimento em Grid")

3. __ChatGPT, utilizado para esclarecer dúvidas e explorar abordagens alternativas para resolver desafios.__ 


## 🎉 Conclusão
Agradeço por dedicar seu tempo para acompanhar este projeto e explorar meu diário técnico. Este desafio representou um marco importante na minha jornada de aprendizado, permitindo-me consolidar conhecimentos e adquirir novas habilidades, especialmente no uso do CSS Grid. Ainda há muito a explorar e aprimorar, mas cada passo me aproxima mais da excelência. 🙌

  <div style="margin-bottom: 20px;">
    <a style="padding-right: 3px;" href="https://www.linkedin.com/in/mariomigueldealmeida/" target="_blank"><img
        src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white"
        target="_blank"></a>
    <a href="mailto:mariomigueldealmeida@gmail.com"><img
        src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white"
        target="_blank"></a>
  </div>

<div>
  <img src="https://i.imgur.com/kwfpJJn.gif" alt="Gif do resultado final da página" width="100%">
</div>