# Transform

[<-- Voltar](../README.md)

Rotacionar textos ou elementos, alterar forma geométrica de elementos e até mesmo utilizar propriedades 3d.

[Exemplo](../src/transform.html)

Ex.:
```css
div {
  transform: ...
}
```

## Propriedades

### Rotate
Rotaciona o elemento informando o valor em `deg` (degress)

```css
div {
  transform: rotate(30deg);
}
```

### Scale
Aumenta ou diminui o tamanho do elemento informando o valor `numerico` de 0 a n

```css
div {
  transform: scale(1.5);
}
```

### Skew

"Entorta" o elemento informando o valor em `deg` (degress)

```css
div {
  transform: skew(20deg);
}
```

### Translate

Deslocar o elemento de um ponto a outro `horizontal`, `vertical`

```css
div {
  transform: translate(10px, 50px);
}
```

## Combinar todas as propriedades

> Quando colocamos mais de uma transformação, a ordem entre elas importa, já que o navegador as aplica *da direita para a esquerda*.

```css
div {
  transform: skew(20deg) rotate(30deg) scale(1.2);
}
```

> A declaração `transform-style: preserve-3d` deve ser usada para os elementos de dentro de um container numa cena 3D também entrarem no cálculo da perspectiva.
