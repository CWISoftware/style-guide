# public class CSharpStyleGuide {

### Boas Práticas Gerais
* Use as configurações default da IDE

### Comentários
* Espaço após as barras duplas (//)

```cs
// comentário aqui
```

### Indentação

* Indente o código com quatro espaços (configuração padrão do VS) ao invés de tabs:
```
public void certo() {
....Console.WriteLine("Certo");
}

public void errado() {
____Console.WriteLine("Errado");
}

```
### Classes
* O Nome de classes é PascalCase:
```
public class CálculoAritimético {

}
```
### Métodos
* O Nome de métodos é camelCase:
```
public class CalculoAritimetico {
	public double calcularMedia() {
	// ...
	}
}
```

### Namespaces

* O nome dos namespaces é PascalCase, com palavras consecutivas simplesmente concatenadas, sem usar underscore
* Quando a codificação é em português, pode-se usar acentuação no nome de namespace
```
// correto
namespace NomeCliente.CamadaServiço.Usuário {

}

// errado
namespace nomeCliente.camadaserviço.usuário {

}
```

# }
