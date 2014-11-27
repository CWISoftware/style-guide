
# CWI Software JavaScript Style Guide() {

### ..Espaçamento

* Indente o código com **2 espaços**:
```javascript
function errado() {
....var name;
}

function correto() {
..var name;
}
```
*  Use espaço antes das chaves de abertura de uma função `{`:
```javascript
function errado(){
}

function correto() {
}
```

* Não utilize espaço ao invocar ou definir uma função/método:
```javascript
function (errado) {
}

function(correto) {
}
```
### convencoesDeNomes

* Use camelCase para nomear objetos, funções e instâncias:
```javascript
var umObjeto = {};
var umaFuncao = function umaFuncao() { };
var umaInstancia = new Person();
```

* Mantenha em maiúsculo a PrimeiraLetra quando criar construtores/classes:
```javascript
// errado
function produtoEstoque(nome) {
  this.nome = nome;
}
// correto
function ProdutoEstoque(nome) {
  this.nome = nome;
}
```

*  Nomeie as constantes `DESTA_FORMA_AQUI`
*  Dê nomes para todas as funções, inclusive quando estas são atribuídas para variáveis. Isto ajuda na leitura dos stacktraces. 
```javascript
var errado = function() {
};

var correto = function correto() {
};
```
* Prefixe com `$` o nome das variáveis que armazenam objetos do jQuery:
```javascript
var parent = $('#parent'); // errado 
var $parent = $('#parent'); // correto
```

### 'Strings'

* Use aspas simples `'` para criar strings
  
 `var errado = "aspas duplas"`; 
 `var correto = 'aspas simples';`

* Utilize `+` para concatenar as strings (no fim da linha)

### Chaves `{   }`

* Use. A única exceção é quando a instrução inteira couber na mesma linha.
```javascript
if (condicao) 
  errado = true;
  
if (condicao) {
  correto = true;
}

if (condicao) correto = true; // Correto caso a instrução esteja na mesma linha!
```

### Vírgulas`,`

* Não coloque no ínicio da linha
```javascript
var nao
 , faça
 , isso;
 
var prefira,
  fazer, 
  isso;
```
* Não coloque vírgulas "extras" no fim. Isto causa bugs no IE.
```javascript
var errado = [
  feijao,
  arroz, 
  abacate, // não coloque a vírgula extra aqui!
];
 
var correto = [
  feijao, 
  arroz,
  abacate
];
```

### Ponto e vírgula`;`

* Use. Não colocar pode causar bugs bizarros. 
```javascript
var errado = true
var correto = true;

var errado = function errado() {}
var correto = function correto() {};

function errado() {
}; // aqui realmente não vai!

function correto() {
}
```

### `var`iáveis

* Declare as variáveis com `var`. Não utilizar `var` faz com que as variáveis apareçam no escopo global.
```javascript
errado = true; 
var correto = true;
```
* Declare as variáveis no topo do seu escopo. A única exceção é as variáveis utilizadas como índices em loop, que podem ser declaradas no momento que serão utilizadas.
* Use somente uma declaração para definir mais de uma variável.
```javascript
// errado
var x = 0;
var y = 0;
var z = 0;

// correto
var x = 0,
  y = 0,
  z = 0;
```

### Propriedades

* Defina propriedades sem usar aspas. Embora qualquer string possa ser um nome de propriedade, use sempre nomes que permitam o seu uso sem aspas, não iniciando o nome com números ou usando hífens no nome.
```javascript
obj.nome_propriedade = 1; // correto
obj.nomePropriedade = 2; // correto
obj['nome-propriedade'] = 3; // errado
```
* Use `.` para acessar as propriedades sempre que o nome da propriedade for conhecido
```javascript
obj.correto;
obj['errado'];
```
* Use `[]` para acessar as propriedades quando o nome da propriedade for desconhecido/parametrizável
```javascript
// correto
function get(atributo) {
  return obj[atributo];
}
```

### `this` is not `that`

* Se você precisar criar uma variável para passar adiante a referênca do objeto atual (bastante comum com KnockoutJS), chame-a sempre de `self`
```javascript
function ViewModelWrong() {
  var that = this; // errado
}

function ViewModelRight() {
  var self = this; // certo
}
```

### Módulos

* Sempre declare ` 'use strict'; ` no topo do módulo.
```javascript
;(function(w, d){
  'use strict';

  function () {
  
  }

})(window, document);
```


# };
