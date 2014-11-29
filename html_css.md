# `<CWI Software HTML/CSS Style Guide>`

### ..Espaçamento

* Indente o código com **2 espaços**
* No CSS, deixe **1 espaço** entre o seletor e a chave (`{`) e antes do valor da propriedade
```html
<ul>
..<li>Correto</li>
</ul>
```

```css
.main {
..color: red;
} 
```

### capitalização

* Todo código deve ser **lowercase**. Não utilizar *camel-case* nas classes CSS, mas sim separar palavras por hífen
```html
<A HREF="/">Errado</A>
<a href="/">Correto</a>
```

```css
.wrongClass {
  color: #D3D3D3;
}
.right-class { 
  color: #d3d3d3;
  font-family: "Times New Roman"; /* dentro da String é permitido maiúscula */
}
```

### ~~Atributo `type`~~

* Omitir o atributo `type` das tags `<link>` e `<script>`
```html
<link rel="stylesheet" href="//errado.css" type="text/css">
<link rel="stylesheet" href="//correto.css">

<script src="//errado.js" type="text/javascript"></script>
<script src="//correto.js"></script>
```

### "'Aspas'"

* Use `"` para valores de atributos no HTML
```html
<a class='errado'>Login</a>
<a class="correto">Login</a>
```

* Use `'` para valores de propriedades no CSS
```css
.wrong {
  font-family: "open sans"; /* errado */
}
.right {
  font-family: 'open sans'; /* correto */
}
```

# `</CWI Software HTML/CSS Style Guide>`
