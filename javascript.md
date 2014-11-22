
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

### convencoesDeNomes

* Use camelCase para nomear objetos, funções e instâncias:
```javascript
var umObjeto = {};
var umaFuncao = function umaFuncao() { };
var umaInstancia = new Person();
```

* Mantenha em maiúsculo a PrimeiraLetra quando criar construtores/classes:
```javascript
//errado
function user(nome) {
  this.nome = nome;
}
//correto
function User(nome) {
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

### 'Strings'

* Use aspas simples `'` para criar strings [exemplo](#chapter-1)
  
 `var errado = "aspas duplas"`; 
 `var correto = 'aspas simples';`

* Utilize `+` para concatenar as strings (no fim da linha)

### Chaves `{   }`

* Use. A única exceção é quando a instrução inteira couber na mesma linha.

### Vírgulas`,`

* Não coloque no ínicio da linha
* Não coloque vírgulas "extras" no fim. Isto causa bugs no IE.

### Ponto e vírgula`;`

* Use. Não colocar pode causar bugs bizarros.

### `var`iáveis

* Declare as variáveis com `var` 
```javascript
errado = true;
var correto = true;
```
* Declare as variáveis no topo do seu escopo. A única exceção é as variáveis utilizadas como índices em loop, que podem ser declaradas no momento que serão utilizadas.

### Propriedades

* Use `.` para acessar as propriedades sempre que o nome da propriedade for conhecido
```javascript
obj.correto;
obj['errado'];
```
* Use `[]` para acessar as propriedades quando o nome da propriedade for desconhecido/parametrizável
```javascript`
// correto
function get(atributo) {
  return obj[atributo];
}
```

# };
