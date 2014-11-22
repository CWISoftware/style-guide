
# CWI Software JavaScript Style Guide() {

### ..Espaçamento

1. Indente o código com **2 espaços** [exemplo]
1. Use espaço antes das chaves de abertura de uma função `{` [exemplo]

### convencoesDeNomes

1. Use camelCase para nomear objetos, funções e classes [exemplo]
1. Mantenha a primeira letra em maiúsculo quando criar construtores/classes [exemplo]
1. Dê nomes para todas as funções, inclusive quando estas são atribuídas para variáveis. Isto ajuda na leitura dos stacktraces. [exemplo]

### 'Strings'

1. Use aspas simples `'` para criar strings [exemplo](#chapter-1)
1. Utilize `+` para concatenar as strings (no fim da linha)

### Chaves `{   }`

1. Use. A única exceção é quando a instrução inteira couber na mesma linha.

### Vírgulas`,`

1. Não coloque no ínicio da linha
1. Não coloque vírgulas "extras" no fim. Isto causa bugs no IE.

### Ponto e vírgula`;`

1. Use. Não colocar pode causar bugs bizarros.

### `var`iáveis

1. Declare as variáveis com `var` 
1. Declare as variáveis no topo do seu escopo. A única exceção é as variáveis utilizadas como índices em loop, que podem ser declaradas no momento que serão utilizadas.

### Propriedades

1. Use `.` para acessar as propriedades sempre que o nome da propriedade for conhecido
1. Use `[]` para acessar as propriedades quando o nome da propriedade for desconhecido/parametrizável



# Exemplos

### Strings <a id="chapter-1"></a>

# };
