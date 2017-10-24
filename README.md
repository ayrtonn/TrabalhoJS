"# TrabalhoJS" 

1- O que é JavaScript?

  O JavaScript é uma linguagem de programação client-side, ou seja, é processada pelo próprio navegador. Com o JavaScript podemos criar efeitos especiais para nossas páginas na Web, além de podermos proporcionar uma maior interatividade com nossos usuários. O JavaScript é uma linguagem dinâmica e orientada a objetos, ou seja, ela trata todos os elementos da página como objetos distintos, facilitando a tarefa da programação.
  Visando o potencial da Internet para o público geral e a necessidade de haver uma interação maior do usuário com as páginas, ela foi desenvolvida em 1995 por Brendan Eich na Netscape Communications, foi originalmente chamado LiveScript mas foi renomeado para JavaScript, devido à relação de amizade do Netscape com Sun Microsystems na época. A norma que descreve o funcionamento do JavaScript é o ECMAScript
  O JavaScript, como o próprio nome sugere, é uma linguagem de scripting. Uma linguagem de scripting é comumente definida como uma linguagem de programação que permite ao programador controlar uma ou mais aplicações de terceiros. No caso do JavaScript, podemos controlar alguns comportamentos dos navegadores através de trechos de código que são enviados na página HTML. O JavaScript é a terceira camada de desenvolvimento por que ele manipula as duas primeiras camadas, isto é: HTML e CSS.
  
2- O que é Closure?

Um closure é uma função interior que tem acesso a variáveis de uma função exterior. O closure tem três cadeias de escopo:

O seu próprio escopo;
O escopo externo, tendo acesso as variáveis da função exterior;
E o acesso as variáveis globais.
A função interior tem acesso não somente as variáveis da função exterior, mas também aos parâmetros dela.

3- O que é Hoisting?

Elevação é nada mais, nada menos do que trazer para o início do escopo a declaração de variáveis e funções.

4- ES6/ES7 features

ES6, ECMAScript 6 ou ES2015, é uma versão do JavaScript. JavaScript é como nós chamamos a linguagem, só que esse nome é um trademark da Oracle (que veio após a compra da Sun). O nome oficial da linguagem é ECMAScript. E ES é simplesmente uma abreviação do mesmo. O TC39 focou em alguns objetivos no desenvolvimento do ES6:
- Ser uma linguagem melhor para construir aplicações complexas
- Resolver problemas antigos do JavaScript
- Facilidade no desenvolvimento de libraries

Declaração de variáveis:

var x let


// escopo de função com var
function doSomething() {
  var a = 1;
  if (true) {
    var b = 2; // b é declarado dentro do if mas é visível fora
  }
  var c = a + b; // 3
}

//escopo de bloco com let
function doSomethingElse() {
  let a = 1
  if (true) {
    let b = 2 // b é declarado dentro do if e não é visível fora
  }
  let c = a + b // Uncaught ReferenceError: b is not defined
}

A diferença principal entre o var e o let é que enquanto o primeiro tem escopo de função, o segundo possui escopo de bloco. Em resumo, let conserta o antigo problema causado pelo hoisting fazendo com que a declaração de variáveis funcione da forma esperada pela maioria dos desenvolvedores.

let x const

let a = 1
a = 2

const b = 1
b = 2 // Uncaught SyntaxError "b" is read-only

const funciona de forma semelhante. A única diferença é que as variáveis criadas não podem ser reatribuídas.

ES7:

Adesão ou possibilidade de utilizar funções assíncronas. As comunicações Síncrona e Assíncrona são dois métodos distintos de sincronização de transmissão, cada uma tem suas vantagens e desvantagens.

Analogia

Imaginemos que um emissor está a enviar uma mensagem de texto através de um tubo e que a mensagem é enviada recorrendo a bolas, cada bola com uma letra. Quando as bolas chegam ao receptor, a mensagem tem que ser remontada, ou seja, têm que se colocar as bolas pela ordem correta, para se voltar a ter a mensagem.

Em comunicação Assíncrona, cada bola tem um número de sequência, que permite que seja colocada na sua posição. Isto permite que as bolas sejam enviadas e recebidas por qualquer ordem, uma vez que esse número de sequência identifica a posição de cada bola (letra) na mensagem.
Em comunicação síncrona, as bolas têm que ser enviadas e recebidas de forma sincronizada, mantendo uma ordem bem definida: a primeira bola (letra) a ser enviada, tem que ser a primeira a ser recebida e assim sucessivamente.


REFERÊNCIAS:

https://developer.mozilla.org/pt-PT/docs/Web/JavaScript/O_que_%C3%A9_o_JavaScript

http://tableless.github.io/iniciantes/manual/obasico/o-que-front-back.html

https://www.significados.com.br/javascript/

https://pt.stackoverflow.com/tags/javascript/info

https://www.caelum.com.br/apostila-html-css-javascript/javascript-e-interatividade-na-web/#11-19-para-saber-mais-varios-callbacks-no-mesmo-elemento

http://tableless.github.io/iniciantes/manual/js/

https://imasters.com.br/desenvolvimento/apresentando-o-conceito-de-closures/?trace=1519021197&source=single

https://developer.mozilla.org/pt-BR/docs/Glossario/Hoisting

https://tableless.com.br/elevacao-ou-javascript-hoisting/

https://tableless.com.br/elevacao-ou-javascript-hoisting/

https://medium.com/@matheusml/o-guia-do-es6-tudo-que-voc%C3%AA-precisa-saber-8c287876325f

https://pt.stackoverflow.com/questions/51268/qual-a-diferen%C3%A7a-entre-comunica%C3%A7%C3%A3o-ass%C3%ADncrona-e-s%C3%ADncrona

https://code.tutsplus.com/pt/tutorials/a-primer-on-es7-async-functions--cms-22367


