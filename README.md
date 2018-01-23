# Javascript

**Manipulando Strings** 

_Propriedades_

Propriedade | Descrição
--- | --- 
**length** | retorna o tamanho da string.

_Funções_

Função | Descrição
--- | --- 
**charAt** | retorna o caractere de uma data posição da string.
**charCodeAt** | retorna o código do caractere de uma data posição da string.
**indexOf** | retorna a primeira posição de uma substring.
**lastIndexOf** | retorna a última posição de uma substring.
**startsWith** | verifica se uma string começa com uma substring.
**endsWith** | verifica se uma string termina com uma substring.
**includes** | verifica se uma string inclui uma substring.
**split** | separa/quebra uma string em um array.
**slice** | extrai uma parte de uma string.
**substring ou substr** | retorna uma parte de uma string a partir de uma posição inicial.
**match** | verifica se uma string atende a uma expressão regular.
**toLowerCase** | retorna uma nova string com os caracteres em minúsculo.
**toUpperCase** | retorna uma nova string com os caracteres em maiúsculo.
**normalize** | retorna a forma normalizada unicode da string.
**repeat** | retorna uma string contendo os elementos do objeto repetidos pela quantidade de vezes dada.
**trim** | retira espaços em branco no começo e no final da string.

> Todas as operações (funções) sobre uma string retornam outra string.

**Manipulando Arrays** 

_Propriedades_

Propriedade | Descrição
--- | --- 
**length** | retorna o número de elementos de um array.

_Funções_

Função | Descrição
--- | --- 
**push(elemento1, ...)** | adiciona um ou mais elementos ao final do array e retorna o novo tamanho. 
**unshift(elemento1, ...)** | insere um ou mais elementos no ínicio do array e retorna o novo tamanho.
**pop()** | retira o último elemento do array.
**shift()** | retira o primeiro elemento do array.
**reverse()** | inverte o array.
**join(delimitador = ",")** | gera uma string dos elementos delimitados pelo delimitador informado.
**slice(posi_ini, posi_fim)** | extrai elementos de um array.
**splice(posi, qtde, elemento1, elemento2, ...)** | remove elementos de um array e (opcionalmente) substitui.
**sort()** | ordenação.
**concat()** | concatena dois arrays e gera um novo.

**Explorando Funções** 

> Toda função em JavaScript é um objeto do tipo **Function**. Portanto possui propriedades e funções.

_Propriedades_

Propriedade | Descrição
--- | --- 
**Function.arguments** | retorna um array dos argumentos de uma função quando estamos dentro da função.
**Function.length** | retorna o número de argumentos de uma função quando estamos dentro da função.
**Function.caller** | retorna a função chamadora da função chamada quando estamos dentro da função chamada.
**Function.name** | retorna o nome de uma função quando estamos dentro da função. 
**Function.displayName** | retorna o nome de exibição de uma função quando estamos dentro da função.
**Function.prototype.constructor** | função base criadora de outras funções.

_Funções_

Função | Descrição
--- | --- 
**Function.prototype.apply()** | chama uma função e aplica um objeto (substitui _this_ pelo objeto passado) e retorna um novo objeto Function. 
**Function.prototype.bind()** | cria uma nova função "cópia/clone".
**Function.prototype.call()** | chama uma função. 
**Function.prototype.toString()** | retorna o código fonte de uma função. 

**Objeto global _document_**

_Propriedades_  

Propriedade | Descrição
--- | --- 
**document.activeElement** | retorna o elemento que possui o foco.
**document.title** | título da página corrente
**document.location** | URI da página corrente
**document.URL** | URI somente leitura da página corrente
**document.cookie** | retorna uma string com os cookies relacionados ao domínio

_Funções_  

Função | Descrição
--- | --- 
**document.getElementById("id")** | retorna um elemento ativo HTML
**document.getElementsByTagName(tagName)** | retorna uma lista ativa de elementos HTML
**document.getElementsByTagNameNS(namespace, tagName)** | retorna uma lista ativa de elementos HTML
**document.getElementsByClassName(className)** | retorna uma lista ativa de elementos HTML
**document.querySelector("lista de seletores")** | retorna o primeiro nodo DOM a partir de document (raiz) ou de uma subárvore **elemento.querySelector("lista de seletores")**
**document.querySelectorAll("lista de seletores")** | retorna um array de nodos DOM (NodeList) a partir de document (raiz) ou de uma sobárvore **elemento.querySelectorAll("lista de seletores")**
**document.hasFocus()** | retorna **true** se algum elemento do documento atual possui o foco.

**Objeto global _window_**

_Propriedades_  

Propriedade | Descrição
--- | --- 
**window.document** | referência para o objeto global document.
**window.innerHeight** | altura da janela interna incluindo a scrollbar.
**window.innerWidth** | largura da janela interna incluindo a scrollbar.
**window.outerHeight** | altura da janela toda do navegador.
**window.outerWidth** | largura da janela toda do navegador.
**window.localStorage** | referência para acesso ao armazenamento local.
**window.sessionStorage** | referência para acesso ao armazenamento local de sessão.
**window.scrollX** | posição horizontal da scrollbar.
**window.scrollY** | posição vertical da scrollbar.
**window.screen** | referência para acesso a propriedades e métodos do objeto screen.
**window.status** | conteúdo da status bar.

_Funções_  

Função | Descrição
--- | --- 
**window.alert("texto")** | exibe um diálogo de alerta.
**window.confirm("texto")** | exibe um diálogo de confirmação.
**window.print()** | imprime o documento atual.
**window.scroll()** | muda a posição da janela.
**window.scrollBy()** | muda a posição do documento.
**window.scrollTo()** | muda para uma a posição do documento.
**window.focus()** | solicita o foco para a janela em questão.
**window.getAttention()** | altera a aparência da janela para chamar a atenção do usuário.
**window.setCursor()** | muda o cursor da janela corrente.
**window.open()** | abre uma nova janela.
**window.openDialog()** | abre uma nova janela do tipo diálogo.
**window.close()** | fecha a janela atual.
**window.postMessage()** | envia mensagens de forma segura para uma outra janela.
**window.setInterval()** | chama uma função de tempo em tempo.
**window.setTimeout()** | chama uma função depois de um tempo.
**window.clearInterval()** | cancela a execução de setInterval.
**window.clearTimeout()** | cancela a execução de setTimeout.
**window.addEventListener()** | registra um _event handler_.
**window.dispatchEvent()** | dispara um _event_.

--- 

**Criando Objetos**

Partindo de um objeto literal "vazio".
```javascript 
var objeto1 = {};
objeto1.propriedade1 = "...";
objeto1.funcao1 = function() { 
    //...
};
```

Partindo de um "super" objeto literal. 
```javascript 
var objeto1 = {
    propriedade1 : "...",
    funcao1 : function() { 
        //...
    }
};
```

Utilizando uma função construtora/modelo com o operador **new**.
```javascript 
var ClasseX = function(p1) {
    this.propriedade1 = p1;
    this.funcao1 = function(x) { 
        return this.propriedade1 + x;
    };
};
var objeto1 = new ClasseX("a");
var objeto2 = new ClasseX("b");
```

> Sempre que utilizar o **new** temos que usar **this** dentro da função. Na prática a engine javascript aplica (apply) o modelo a uma instância gerada pela engine.

Utilizando uma função construtora.
```javascript
var objeto1 = (function() {
    var funcao_interna = function(x) {
        //...
    };

    return {
        propriedade1 : "...",
        funcao1 : function(b) {
            return funcao_interna(b);
        }
    }
})();
```

--- 

**Fases de um evento DOM**

Segundo o padrão DOM, cada evento possui três fases:
- Captura 
- No alvo
- Borbulhamento: quando o usuário, por exemplo, clica sobre um botão/link o evento de clique é acionado no alvo, depois ele "borbulha" para o elemento pai logo acima na árvore DOM e vai "borbulhando" até atingir a raiz de tudo. Esse processo de borbulhamento pode ser cancelado no alvo.

> O IE não implementa a fase de captura.

**Temporizadores** 

- window.setInterval(): executa continuadamente uma rotina/função dentro de um intervalo de tempo.
- window.setTimeout(): agenda a execução de uma rotina/função para um dado intervalo de tempo.

**Web Workers**

A partir da especificação HTML5 (http://www.w3.org/TR/workers) é possível executar código fora da thread UI e isso pode contribuir muito para melhorar o desempenho de aplicações dinâmicas. Antes da inclusão deste recurso tinhamos que usar os temporizadores. Vale ressaltar que não é possível manipular o DOM de dentro de um web worker. Se for necessário manipular o DOM temos que usar os temporizadores.

> O uso de web workers é mais indicado para _serviços_. Ex: obter conteúdos de uma api. Essa operação não precisa ficar presa ao código que manipula o DOM, ela pode perfeitamente ficar em um arquivo externo e ser acionada sempre que necessário.

**Boas Práticas** 

- Posicionar os scripts no final do documento, antes de **\</body>**.
- Definir variáveis locais para acessar objetos globais (this, document, window e outros). Essa prática deve ser usada principalmente em laços de repetição.
- Evitar o acessos ou alterações repetidas ao DOM (xml). Essa prática deve ser usada principalmente em laços de repetição.
```javascript
//desempenho ruim - acessa e modifica toda hora o DOM
function renderizarTabela(itens) {
    document.getElementById("#main").innerHtml = 
        "<table>"+
            "<tr>"+
                "<th>Código</th>"+
                "<th>Nome</th>"+
                "<th>Preço</th>"+
            "</tr>";
    for (var i=0; i<itens.length; i++) {
        document.getElementById("#main").innerHtml += 
        "<tr>"+
            "<td>"+itens[i].codigo+"</td>"+
            "<td>"+itens[i].nome+"</td>"+
            "<td>"+itens[i].preco+"</td>"+
        "</tr>";
    }
    document.getElementById("#main").innerHtml += "</table>";
}

//desempenho melhor - acessa e modifica o DOM uma única vez no final
function renderizarTabela(itens) {
    var tabela = 
        "<table><tr><th>Código</th><th>Nome</th><th>Preço</th></tr>";
    for (var i=0; i<itens.length; i++) {
        tabela += 
        "<tr><td>"+itens[i].codigo+"</td><td>"+itens[i].nome+"</td><td>"+itens[i].preco+"</td></tr>";
    }
    tabela += "</table>";
    document.getElementById("#main").innerHtml = tabela;
}
```
- A realização de loops em um array é mais rápido do que loops em uma coleção **{ var colecao = document.getElementsByTagName("input"); }**, de modo que se primeiro copiarmos a coleção para um array, o acesso das propriedades dos elementos em array será mais rápido e eficiente.
- Ao realizar um loop em uma coleção, a primeira otimização que podemos fazer é armazenar a coleção em uma variável local e armazenar **length** fora do loop, seguido pelo uso de uma variável local para elementos que são acessados repetidamente.
- Verifique se de fato é necessário usar **document.getElementsByTagName()**, pois esta função retorna uma **coleção ativa** de elementos HTML. Utilize a API de seletores **document.querySelectorAll()**, pois esta nova função retorna um **array**. É claro que tem ocasiões em que se deseja atuar sobre elementos ativos, nestes casos não tem o que fazer, temos que usar **coleções ativas**.
```javascript
//retorna um NodeList = um objeto do tipo array
var arrayDeLinks = document.querySelectorAll("#menu a");

//retorna uma coleção ativa de elementos HTML
var colecaoAtivaDeLinks = document.getElementById("menu").getElementsByTagName("a");
```
- Evite **reflow** e **repaint** sempre que possível. Se que possível dê preferência para repaint, pois reflow é uma operação computacional custosa. Se for necessário reflow gere reflows em lote (para evitar recálculos e modificações consecutivas no mesmo elemento - isso é custoso). Vale ressaltar que navegadores modernos enfileiram alterações em fluxo para evitar reflows individuais, mas mesmo assim é importante tomar cuidado.
```javascript
//gera reflows consecutivos sobre o mesmo elemento => mais custoso e menos eficiente
var btn = document.getElementById("btnSalvar");
btn.style.borderLeft = "1px";
btn.style.borderRight = "2px";
btn.style.padding = "5px";

//gera reflow em lote sobre o mesmo elemento => menos custoso e mais eficiente
var btn = document.getElementById("btnSalvar");
btn.style.cssText= "border-left: 1px; border-right: 2px; padding: 5px;";

//outra forma de gerar reflow em lote => menos custoso e mais eficiente
var btn = document.getElementById("btnSalvar");
btn.className = "novo-estilo";
```
- Sempre que possível cancele o borbulhamento de eventos.
- Sempre que possível utilize Web Workers para processamentos em paralelo à thread UI em substituição aos temporizadores. Vale ressaltar que não é possível manipular o DOM de dentro dos web workers, sendo neste caso que o mais indicado é continuar usando os temporizadores.
- Dê preferência para utilizar métodos e APIs nativas. Um exemplo é a classe **Math** que oferece uma série de propriedades e métodos matemáticos prontos e de auto desempenho. 

**Javascript na Web** 

A manipulação de Javascript na web é feita através de um navegador. Geralmente os navegadores possuem duas implementações importantes, uma biblioteca/dll que interpreta o nosso código Javascript e outra biblioteca/dll que manipula o DOM (xml) e cuida da renderização.

Toda vez que o navegador se depara com um código Javascript, este precisa ser interpretado para que a execução ocorra devidamente. De acordo com o código definido, uma ou várias chamadas à biblioteca/dll DOM devem ser realizadas, e é aí que temos um cenário que pode gerar gargalos, pois acessar o DOM sempre exige chamadas externas.

Por isso que é uma boa prática evitar acessos e alterações repetidas no DOM.

**Navegadores** 

Nome | DOM e Renderização | Engine Javascript 
--- | --- | --- 
Internet Explorer | Trident (mshtml.dll) | JScript (jscript.dll)
Safari | WebCore/WebKit | SquirrelFish 
Google Chrome | WebCore/WebKit | V8 
Firefox | Gecko | SpiderMonkey ou TraceMonkey

--- 

**Fontes** 

- Livro Javascript de Alto Desempenho - novatec
- https://www.youtube.com/user/rodrigobranas
- https://www.w3schools.com/js
- https://www.caelum.com.br/curso-html-css-javascript
- https://www.caelum.com.br/apostila-html-css-javascript
- https://jquery.com