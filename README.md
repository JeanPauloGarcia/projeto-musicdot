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
    unordered list: <ul></ul>
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

    bookmark (demarcação):
        <p>Mais informações <a href="#info">aqui</a>.</p>
        <h2 id="info">Mais informações sobre o assunto:</h2>

    bookmark em outra página:
        <a href="http://www.caelum.com.br/curso/wd43/#contato">
    
    Outra página do próprio site:
        <p>Acesse <a href="index.html">nossa loja</a>.</p>