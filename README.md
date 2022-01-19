# projeto-musicdot
Projeto em HTML CSS e Javascript da Apostila Caelum


HTML: Linguagem de Marcação de Hipertexto

Sintaxe: estrutura/forma das expressões, instruções e unidades

Tags: marcação de conteúdo
    Sintaxe: <nomedatag>
    Ex: <h1>

Atributo: parâmetros para tags
    Sintaxe: atributo="valor"
    Exemplo: <img src="/endereço/img.jpg">

Tags q carregam conteúdo externo não precisam de fechamento
    Ex: img

Título
    H1 só pode usar uma vez por página

Parágrafo: <p></p>

Ênfase:
    <strong>: texto mais forte (negrito <b>)
    <em>: mais forte (itálico <i>)
    <small>: texto mais fraco
Imagem:
    <img src (local) alt (nome da imagem)>

Legenda imagem:
    <figure>
    <img src="img/matriz-musicdot.png" alt="Foto da matriz da musicdot">
    <figcaption>Matriz da MusicDot</figcaption>
    </figure>

Estrutura
    <!DOCTYPE>
        (versão do HTML mais atual)
      <html> <!-- mãe -->
        <head></head> <!-- filha -->
            (head: informações de interesse do navegador)
        <body></body> <!-- filha -->
            (obrigatório no mínimo 1 elemento filho)
      </html>

Codificação/Título
    <head>
      <meta charset="utf-8">
      <title>MusicDot</title>
    </head>

Desenvolvimento do HTML mantido pelo W3C (World Wide Web Consortium) https://www.w3.org/ https://github.com/whatwg/html


CSS: Cascading Style Sheet ou folha de estilos em cascata (outra linguagem, para estilização)
    Sintaxe: 
        propriedade:valores;
    Ex: color: blue;
        background-color: yellow;

Seletor CSS: elementos aos quais serão aplicados os estilos
    Sintaxe:
        seletor{
            propriedade: valor;
        }
    Sintaxe Subpropriedade:
        seletor {
            propriedade-SUBPROPRIEDADE: valor;
        }
    Ex: text-align: center;
        text-decoration: underline;
Ligação com arquivo .css:
    <link rel="stylesheet" href="estilos.css">

Fontes
    font-family
    Serif: "Times" e "Times New Roman"
    Sans-serif: "Arial" e "Helvetica"
    Monospace(letras do mesmo tamanho): "Courier"

    Ex: 
        h1 {
        font-family: serif;
        }

        h2 {
        font-family: sans-serif;
        }

        p {
        font-family: monospace;
        }
    Ex:
        font-family: "Helvetica", "Lucida Grande", sans-serif;
        (verifica a primeira, a segunda, e se não tiver, qualquer uma sans-serif)

    Font-style: normal; (ou: italic, oblique)
        (itálico muda alguns desenhos/detalhes das letras, oblíquo só inclina sem mudar nada)
    
    Outras propriedades: 
     text-aling: right /*alinhamento do texto/* (ou: center, left, justify)

     line-height: 3px; /* tamanho da altura de cada linha */

     letter-spacing: 3px; /* tamanho do espaço entre cada letra */

     word-spacing: 5px; /* tamanho do espaço entre cada palavra */

     text-indent: 30px; /* tamanho da margem da primeira linha do texto */

Imagem de fundo: background-image: url(sobre-background.jpg);

Bordas: 
    border-color: red;
    border-style: solid;
    border-width: 1px;
  ou
    border: 1px solid red;
    (para o color funcionar, o style deve ter alguma valor diferente de none)

  Lado da borda:
    border-top: 1px solid red; /* borda vermelha em cima */
    border-right: 1px solid red; /* borda vermelha à direita */
    border-bottom: 1px solid red; /* borda vermelha embaixo */
    border-left: 1px solid red; /* borda vermelha à esquerda */

Comentários: /*comentário*/

Cores
  nome:
    color: red
  rgb (0 a 255):
    color: rgb(255, 255, 0) */amarelo*/
    color: rgb(255, 200, 0) */laranja*/
  hexadecimal (MAIS COMUM e com aceitação universal nos navegadores):
    color: #ffffff 
    (caracteres: 123456789ABCDEF
    #+XX+XX+XX: XX=red, XX= green, XX=blue)
  
  
INSPEROR DE ELEMENTOS
    botão direito do mouse, inspetor, setinha no canto superior esquerdo

ESPAÇAMENTO
    padding (espaçamento interno)
    margin (espaçamento externo)

    width: largura
    height: altura

    Ex:
        p {
        background-color: red;
        height: 300px;
        width: 300px;
        }   

    SUBPROPRIEDADES:
        padding-top
        padding-right
        padding-bottom
        padding-left

shorthand property (encurtamento)
   
    padding: 10px; (top, right, bottom, left)
    padding: 10px 20px 15px 5px; (top, right, bottom, left)
    padding: 10px 15px; (top, bottom - right, left)
    padding: 10px 20px 15px; (top - right, left - bottom)
    
    se encurtar: sentido anti-horário, começando a partir do left

    auto: (margem automática conforme espaço disponível na tela)
    Ex:
        margin: 0 auto;

Listas
    unordered list: <
    ></ul>
    ordered list: <ol></ol>
    list item: <li></li>

        Ex:
        <ul>
        <li>Primeiro item da lista</li>
        <li>
            Segundo item da lista:
            <ul>
            <li>Primeiro item da lista aninhada</li>
            <li>Segundo item da lista aninhada</li>
            </ul>
        </li>
        <li>Terceiro item da lista</li>
        </ul>

    definition list (glossário):    <dl></dl>
        Ex:
        <dl>
            <dt>HTML</dt>
            <dd>
                HTML é a linguagem de marcação de textos utilizada
                para exibir textos como páginas na Internet.
            </dd>
            <dt>Navegador</dt>
            <dd>
                Navegador é o software que requisita um documento HTML
                através do protocolo HTTP e exibe seu conteúdo em uma
                janela.
            </dd>
        </dl>

    list-style-type: circle;
    list-style-type: upper-alpha; /*sequência alfabética*/

        Ex:
            ul {
                list-style-type: circle;
            }
            ol {
                list-style-type: upper-alpha;
            }

    shorthand property:
        list-style: circle

LINKS
    tag de âncora: <a>

    links (externos): 
        Visite o site da <a href="https://www.caelum.com.br">Caelum</a>.

    abrir em outra aba:
        <a href="https://www.caelum.com.br" target="_blank"> 

    bookmark (demarcação) - link para um trecho da mesma página:
        <h2 id="info">Mais informações sobre o assunto:</h2>
    
    chamar bookmark/marcação:
        <p>Mais informações <a href="#info">aqui</a>.</p>

    bookmark em outra página:
        <a href="http://www.caelum.com.br/curso/wd43/#contato">
    
    Outra página do próprio site:
        <p>Acesse <a href="index.html">nossa loja</a>.</p>



SELETORES
    Seletores mais específicos:
            tag-pai tag-filha
            class=""
            id=""
        
        tag-pai tag-filha
        Ex:
            figure img{
                width: 300px;
            }

        class=""
        Ex:
            HTML:
            <img class="figura1">
            
            CSS:
            .figura1 {
                width: 300px;
            }
        (feito pra CSS e JavaScript)
        
        id=""
        Ex:
            HTML:
            <img id="figura1">
            
            CSS:
            #figura1 {
                width: 300px;
            }
        (para estilização, usar class e não id)

    Prioridade dos seletores:
        tag: 1
        class: 10
        id: 100
    Ex:
        p { 
            color: blue;
        }
        .paragrafo { 
            color: red;
        }
        #paragrafo-rosa { 
        color: pink;
        }
        - No exemplo acima (tag, class, id), a cor prioritária é pink (id = 100)

    - dois seletores somam valor
    Ex:
        body p {
            color: pink;
        }
        - tag+tag = 1+1 = 2

    - em seletores iguais o último tem prioridade

    - trabalhar sempre com baixa escificidade (prioridade), para q não seja impossível sobrescrever valores

HERANÇA
    Elemento filho herdar característia de estilo de elemento superior. Características podem ou não passar aos descendentes

    Ex:
        HTML:
        <body>
            <p>
            <figcaption>
        CSS:
        body {
            font-family: sans-serif;
        }
        - font aplicada à body, p e figcaption

ELEMENTO SEMÂNTICO:
    Tags: 
        h1, p, figure, 
        section, article, addres
        para representar com precisão os elementos

    passam informação com significado específico para o conteúdo interpretado pelo navegador
        Ex:
            <section>, <article>, <address>
    -úteis para leitores não visuais (acessibilidade/Google)
    -sites mais semânticos e estruturados ganham prioridade nas respostas de buscas
    
    Servem para representar e não para "exibir" (não visual)
    Exceção:
        -tags para facilitar estilização: 
        <div>(divisão em blocos), 
        <span>(texto sem quebrar linha)
        <dl> = Definition List
        <dd> = Detalhes da Descrição


INHERIT
    valor "inherit" indica ao elemento q deve usar o msm valor do elemento pai
    Ex:
        HTML
        <div>
            <img>
        </div>
        CSS
        div {
            width: 30px;
            height: 30px;
        }
        img {
            width: inherit;
            height: inherit;
        }
    -usar inherit quando a propriedade não são aplicadas em cascata (herança)

DESACOPLAMENTO COM CLASSES
    tag+class
    Ex:
        <h3 class="subtitulo">TITULO H3</h3>
        .subtitulo {
            blablabla
        }

PADRÕES CSS (BEMCSS)
    Padronização da nomenclatura de CSS
    BEMCSS:
        bloco__elemento--modificador
        bloco = representa uma divisão de conteúdo cuja sua existência já tenha um sentido por si só
        elemento = representa uma parte semântica do bloco 
        modificador = uma sinalização de comportamento ou estilização
    DIVISÕES:    
        double snake__case
        double kebab--case
    Kebab-case para HTML e CSS 
    camelCase para JavaScript.
    display: 
        display: block (embaixo)
            não permite elemento ao lado, mesmo com width
        display: inline (ao lado)
            permite elemento ao lado
            não recebe width e height
        display: inline-block
            permite elemento ao lado
            recebe propriedades de tamanho (width, height)
    Ex:
        HTML:
        <p>Um parágrafo que é block</p>
        <a>Um link que é inline</a>
        CSS:
        p {background-color: blue;}
        a {background-color: red;}

EM REM
    medidas baseadas em tamanho de fonte. 
    PX: tamanho fixo
    EM: tamanho depende da fonte do elemento pai 
        HTML font-size: 10px
            BODY font-size: 1.4em (=14px)
                DIV font-size: 1.2em (=16.8)
    REM: tamanho da fonte do <html> (body). /* facilmente escalável em responsividade */
        HTML font-size: 10px
                BODY font-size: 1.4em (=14px)
                    DIV font-size: 1.2em (=12px)
    Ex.:
        HTML: <img src="img/foto" alt="Uma foto">
        CSS:
            html {font-size: 10px;}
            div {font-size: 20px;}
            img {
                height: 10rem; /* A altura será de 100px (10x10) */
                width: 10em; /* A largura será de 200px (10x20) */
                }
        
    medida relativa: %
    Ex.:
        HTML: <div><img src="img/flor.png" alt="Foto de uma flor"></div>
        CSS:    
            div {width: 400px;} 
            img {width: 100%;}

    "Estas unidades de medida são ideais para quando o site precisa ser exibido em diferentes tamanhos de telas, onde em cada tamanho de tela a fonte deve ser exibida em escalas de tamanhos diferentes e proporcionais entre si."

RESPONSIVIDADE (Web Design Responsivo)
    Fazer a experiência do usuário em diversos dispositivos mais atraente (usando @media)
    Web única (One Web)
    -CSS3
    -Detectar se é dispositivo móvel através do User-Agent do navegador       
    -Boa prática: incluir link da versão normal do site (função visualizar como desktop)
    -Media types: diferenciar suporte de regras de layout
    CSS2
        Declarados ao invocar arquivo CSS:
            HTML:
            <link rel="stylesheet" href="site.css" media="screen">
            <link rel="stylesheet" href="print.css" media="print">
            <link rel="stylesheet" href="handheld.css" media="handheld">
        Declarados no CSS:
            CSS:
            @media screen {
                body {
                    background-color: blue;
                    color: white;
                }
            }
            @media print {
                body {
                    background-color: white;
                    color: black;
                }
            }
        Media types:
            screen: visualização normal (Desktop)
            print: regras de impressão
            handheld: para dispositivos móveis
                modelo antigo, não mais usado
            os celulares modernos tbm usam media type screen
    CSS3
    regras do CSS vinculadas a propriedades do dispositivo: 
        -Tamanho da tela, 
        -orientação (landscape ou portrait) e 
        -resolução em dpi
    Ex.:
        HTML:     
        <link rel="stylesheet" href="base.css" media="screen">
        <link rel="stylesheet" href="mobile.css" media="(max-width: 480px)">
        CSS:
        @media screen {
            body {
                font-size: 16px;
            }
        }
        @media (max-width: 480px) {
            body {
                font-size: 12px;
            }
        }
    Problemática: celulares com telas maiores q a escolhida
    device-width: representa um número em pixels que o fabricante do aparelho considera como mais próximo da sensação que o usuário tem ao visualizar a tela
    Ex.:
        iPhones: device-width 370px
    Viewport: tamanho da tela visível
    Solução: 
        <meta name="viewport" content="width=370">
        <meta name="viewport" content="width=device-width">
    Requisitos do design responsivo:
        -layout fluído usando medidas flexíveis, como porcentagens;
        -media queries para ajustes de design;
        -uso de imagens flexíveis.
    mobile-first: mais recomendado
        usando media queries min-width
        abordagem mais simples e evolutiva, devido a área limitada
        mudar p/ desktop: readaptar layout
    desktop-first: começa pelo ambiente mais livre e vai tentando cortar coisas quando chega no mobile
    
LIVROS PAGOS
    https://www.casadocodigo.com.br/

PROCESSO DE DESENVOLVIMENTO
    Passar info doprojeto
    analisar e validar info
    publico alvo
        tom linguistico
        visual
        intensidade e tipo de inovações
    1ª etapa (análise):
        -UX Design (Experiência do usuário)
            Cursos de Design de Interação, Experiência do Usuário e Usabilidade
        -Designer
        -Conteúder
        Levantamento das informações:
            -quantidade
            -conteúdo
            -localização
            -estilização
    
    Resultado (definições sobre):
        -Navegação (mapa do site)
        -Esboço das visões (layout)
        -Visões parciais (diálogos de alerta e confirmações da aplicação)
        -Estilo fica genérico (fontes, cores e imagens neutras)
        -Informações escritas
        esboços = wireframes 
    2ª etapa (á partir dos wireframes)
        Adicionar:
            -cores
            -fontes
            -fundos
            -bordas
            -características visuais
        Mesma equipe mas sem a pessoa de conte´udo
        Ferramentas:
            -Photoshop
            -Illustrator
            -Figma
            ...
    Resultado:    
        Layout = imagens estáticas com visual pronto
    3ª etapa (front-end):
        Objetivo: telas visíveis e utilizáveis por navegador
        Tecnologia: HTML, CSS, JavaScript
        Análise do layout
            Definir:
                Áreas de página
                    cabeçalho
                    rodapé
                    conteúdo principal
                HTML
                    header
                    main
                    footer
            Planejamento de fora para dentro
                1º ver header, main, footer
                Apronfudar em 1
                    header
                        logo
                        3 links
                Aprofundar nas outras
                ...
ESTRUTURA
    PRINCIPAL
        html
        header
        main
        footer
    CABEÇALHO
        nav
        ul
        li

CSS RESET   
    definição de valores básicos no CSS para sobrescrever o estilo padrão do navegador
    ESTILOS:
        HTML5 Boilerplate
            Um pouco complexo
            https://html5boilerplate.com/
        YUI3 CSS Reset
            Reset: Muda tudo para valores padrão
            Base: margens e dimensões de elementos padronizados
            Font: tipologia com visual consistente, incluindo dispositivos móveis
        Eric Meyer CSS Reset  
            http://meyerweb.com/eric/tools/css/reset/
        Existem outros
    FONTES EXTERNAS
        Google Fonts
            https://fonts.google.com/
            link
            Ex.: 
                <link href="https://fonts.googleapis.com/css?family=Roboto&display=swap" rel="stylesheet">
        @import
            direto no CSS:
            @import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');
            body {font-family: 'Roboto', sans-serif;}
        @font-face
            @font-face {
            font-family: minhaFonte;
            src: url(fonts/minha-fonte-customizada.woff);
            }
            body {font-family: 'minhaFonte', sans-serif;}
        Verificar direitos de uso
MODULARIZAR COMPONENTES
    Usar um estilo de CSS para todas as páginas
            (tipos
            cor
            tamanho
            componentes)
        seções repetidas ou não em outras páginas do site
        Vantagens:
            poder escrever HTML com as classes
            importação de só um arquivo CSS padrão
        Desvantagem:
            Arquivo CSS grande causa efeito na performance
            Difícil encontrar o seletor
    Usar um estilo para cada componente
        Vantagens:
            Só importa os componentes necessários para cada página
        Desvantagens:
            Importar um CSS diferente para cada componente
FRAMEWORK       
    Facilitador

ENHANCEMENT (melhoria/aprimoramento)
    Condições, opções, limitações e restrições
        Tela
        Mouse, teclado   
        Navegador
        Velocidades de Conexões 
        Pessoas com Deficiências (cegueira, miopia, visão embaçada; incapacidade de usar um mouse, controle motor com limitações; audição: surdez)
        Ônibus/Escritório
    Testar em todas as condições
    Usar fluxo de desenvolvimento que inclua a maior parte das situações:
        Usar analogia da caixa de fósforo/Caixa de sapato
        Conteúdo
            Qual tipo
            Onde
            Quanto em cada lugar
            Como será agrupado
        TESTE
            -revisão de conteúdo, ortografia, etc
        SEMÂNTICA com HTML
            melhoria em cima do conteúdo sem nenhuma marcação
                Ex.: tag footer
                leitores de tela
                    se movimenta pelas tags
                Ex.: lê diretamente o footer
        TESTE
            -definir casos de uso
                caso de uso: descrição de uma funcionalidade “especificação do comportamento da funcionalidade”
            -testar site conforme cada leitor
            -programas q exibem árvore de assebilidade (Ex: Dev Tools do Firefox)
        CSS
            3º passo (depois de conteúdo e semântica)
            Começar pela caixa de fósforo (limitando largura e altura do viewport)
        USER AGENT
            identificação do tipo de dispositivo do navegador q está acessando o site
        tags novas em navegadores desatualizadas viram <div>
        propriedades e valores novos de CSS em navegadores desatualizados são desconsiderados
    P.E. (Progressive Enhancement)
        - Escolher marcação semântica
        - Testar semântica em leitores de tela (NVDA) ou em ferramentas de acessibilidade (Dev Tolls do Firefox)
        - Desenvolver com device-mode aberto no mobile
        - Mobile-first
        - Testar touch no device-mode

        Device-mode:
            aumentar área clicável

        Verificar suporte do padrão de cores: https://caniuse.com/?search=rrggbbaa
DISPLAY FLEX
    manipular posição de elementos
        display:
            inline, block, inline-block
        margin
        text-align
    display: flex; (flexível)
        elemento torna-se flex container
        Flex Container
            permite manipular elementos filhos
            todos filhos de elemento flex automaticamente ficam lado a lado como se fosse display inline
    JUSTIFY-CONTENT (propriedade)
        ajusta HORIZONTALMENTE os filhos do flex container:
        flex-start (valor)
            valor padrão, lado a lado à esquerda
        flex-end
            lado a lado à direita
        center
            lado a lado no meio
        space-between
            1º à esquerda e último á direita, o restante distribuídos
        space-around
            distribuído com espaço em volta (o espaço de elementos próximos é somado, portanto o 1º e o último tem menos espaçamento nas suas laterais)
        space-evenly
            corrige o problema acima, espaçamento igual em ambos os lados
    ALIGN-ITEMS
        ajusta VERTICALMENTE os elementos filhos:
        stretch
            valor padrão, se esticam proporcionalmente na vertical
        flex-start
            alinhados no topo do flex container
        flex-end
            alinhados com a base
        center
            alinhados com o meio
        baseline
            alinhados com a base do conteúdo textual de cada um deles
    FLEX-WRAP (propriedade)
        "quebra de linha" dos elementos em linha (inline)
        nowrap (valor)
            valor padrão, elementos lado a lado, msm q não haja espaço horizontal
        wrap
            elemento q não cabem na lateral vão para a linha debaixo
        wrap-reverse
            elemento q não cabem na lateral vão para a linha de cima
FLEXBOX B
    layouts mais declarativos com flexbox
    
RESPONSIVIDADE E FALLBACK
    Browsers desatualizados
    https://caniuse.com/
        mostra compatibilidade de navegadores com propriedesdes CSS

    Section: função semântica
    Div: função visual

FORMULÁRIO
    Semântica: deve haver um rótulo/texto explicativo para o campo de email
    Propriedade overflow: Especifica quando o conteúdo de um elemento de nível de bloco deve ser cortado, exibido com barras de rolagem ou se transborda do elemento.
        visible | hidden | scroll |
        visible: conteúdo não é cortado e pode ser renderizado para fora da caixa de conteúdo.
        hidden: conteúdo é cortado e nenhuma barra de rolagem é exibida.
        scroll: conteúdo com barras de rolagem que são exibidas SEMPRE. Impressoras podem imprimir o conteúdo vazado.

EXERCÍCIO: EMBARALHANDO OS ITENS DO RODAPÉ EM TELAS MAIORES COM FLEXBOX

COMPONENTE/BLOCO: CONTAINER
    estilo repetido
    colocar estilo dentro de um container no css para não repetir código, chamar o container no html

DISPLAY: grid
    "Display: flex": bom p/ distribuição igual em direção bem definidad
    forma bidimensional