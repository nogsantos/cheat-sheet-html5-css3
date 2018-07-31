# Sombra e opacidade

[<-- Voltar](../README.md)

Sombra e opacidade destacam os elementos ou dão efeito de iluminação e tridimensionalidade. Para adicionar sobra a algum elemento da tela (textos, divs, etc...), podemos utilizar as propriedades `text-shadow` e `box-sadow`.

[Exemplo](../src/box-shadow.html)

## Sombra

A propriedade `text-shadow` recebe algumas configurações para dar impressão de tridimensionalidade, perspectiva, difusão de luz, além da cor da sombra.

`text-shadow: [horizontal[obrigatorio]] [vertical[obrigatorio]] [blur-radius[opcional]] [cor[opcional]];`

### Textos

```css
h1 {
  text-shadow: 5px 5px #000;
}
```

### Div's

```css
div {
  box-shadow: 5px 5px #000;
}

Dentro do elemento:

div {
  box-shadow: 5px 5px #000, inset 0 0 .5em #999;
}
```

## Opacidade


A escala da opacidade vai de 0 a 1, onde, 0 = totalmente invisível e 1 = totalmente visível.

### Textos

```css
h1 {
  opacity: .5;
}
```

Quando aplicado a propriedade `opacity` em um elemento que contenha filhos, todos eles herdarão essa característca, por exemplo, se uma div possuir texto, ele também receberá essa opcidade definida em seu pai.

Para evitar que os filhos herdem a opcidade do elemento pai, pode-se modificar a opacidade apenas do fundo do elemento, escolhendo uma cor semitransparente na escala RGB.

```css
div {
  background-color: rgba(0 ,0, 0, .3);
}
```

Valor	| Descrição
------|----------
red	| Define a intensidade da cor `vermelha` que pode ser passada como um valor inteiro entre *0* e *255*, ou como porcentagem do entre *0%* e *100%*
green | Define a intensidade da cor `verde` que pode ser passada como um valor inteiro entre *0* e *255*, ou como porcentagem do entre *0%* e *100%*
blue |	Define a intensidade da cor `azul` que pode ser passada como um valor inteiro entre *0* e *255*, ou como porcentagem do entre *0%* e *100%*
alpha | Define a opacidade como um numeral entre *0.0* _(completamente transparente)_	e *1.0* _(totalmente opaco)_
