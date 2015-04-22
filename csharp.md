# public class CSharpStyleGuide {

### Boas Práticas Gerais
* Use as configurações default da IDE

### Comentários
* Espaço após as barras duplas (//)

```csharp
// comentário aqui
```

### Indentação

* Indente o código com quatro espaços (configuração padrão do VS) ao invés de tabs:
```csharp
public void Certo() {
....Console.WriteLine("Certo");
}

public void Errado() {
____Console.WriteLine("Errado");
}

```
### Classes
* O Nome de classes é PascalCase:
```csharp
public class CálculoAritmético {

}
```
### Métodos
* O Nome de métodos **privados** é **camelCase**:
```csharp
public class CalculoAritmetico {
	private double calcularMedia() {
		// ...
	}
}
```
* O Nome de métodos **públicos** é **PascalCase**:
```csharp
public class CalculoAritmetico {
	public double CalcularMedia() {
		// ...
	}
}
```

### Namespaces

* O nome dos namespaces é PascalCase, com palavras consecutivas simplesmente concatenadas, sem usar underscore
* Quando a codificação é em português, pode-se usar acentuação no nome de namespace
```csharp
// correto
namespace NomeCliente.CamadaServiço.Usuário {

}

// errado
namespace nomeCliente.camadaserviço.usuário {

}
```

# }
