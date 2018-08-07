# Seletores

[<-- Voltar](../README.md)

[Ex.: Html](../src/home.html)

[Ex.: Css](../src/home.css)

## Lista

- tag `<element>`
- id `#`
- classe `.`
- ancestral ` ` descendente
- irmão `~` irmão
  - Selecionar elementos depois de outros elementos.
- irmão `+` irmão seguinte
  - seleciona apenas o elemento imediatamente depois
- pai `>` filho
  -  Indica que queremos aplicar a propriedade apenas no primeiro grau da hierarquia.

## Pseudoclasses

São classes que o navegador coloca naturalmente, mais rápidos que os seletores. São chamadas com os `":"` (dois pontos):

### Estruturais

#### first-child

Seleciona o primeiro filho do elemento

#### last-child

Seleciona o último filho do elemento

#### nth-child

Pode reber os parâmetros `odd` e `even` ou numéricos

- `:nth-child(odd)` - linhas ímpares;
- `:nth-child(even)` - linhas pares;
- `:nth-child(3)` - terceira linha;

```css
:nth-child(xn + c)
```
- x é a periodicidade, de quantos em quantos elementos será aplicado o estilo;
- c é o ponto de partida;
- n é a variável, que começa em 0 (zero).

Ex.:

```css
:nth-child(7n+3)
```

```css
tr:nth-child(odd)
```
ou
```css
table:nth-child(odd)
```

Neste caso as _tags_ `tr` e `table` foram utilizadas para especificar o seletor na tabela, só aplicando nas linhas ímpares.

#### nth-of-type

Somente os tipos especificados

```css
blockquote:nth-of-type(even)
```

Ex.:
```html
  <p>
  <p>
  <h2>
1 <blockquote>
  <p>
  <p>
  <h2>
2 <blockquote>
  <p>
  <p>
  <h2>
3 <blockquote>
```

### Dinâmicas

#### hover

Aplica um novo estilo dinâmicamente pelo navegador

```html
<a href="..." class="botao hover">
```

```css
.botao{
  border: 8px solid purple;
}

.botao:hover{
  background-color: purple;
}
```

#### focus

Quando o teclado está com foco em algum elemento

#### active

Quando o há um clique em um elemento

#### checked

...
