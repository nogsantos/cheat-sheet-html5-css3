# Posição

[<-- Voltar](../README.md)

## Absolute

O position absolute, só é relativo a página `<body>` quando nenhum nó pai possuir uma posição definida.

```html
<html>
  <body> <!-- [position: relative/absolute/fixed (referencia)] -->
    <div> <!-- [position absolute] -->
      ...
```

Caso o nó pai, do elemento em que será atribuída a posição absolute, possuir um definição de posicionamento, esse elemento terá posição `absolute` em relação a ele.

> O valor `static` é o padrão para a propriedade `position`, dessa forma, mesmo se definida em um nó pai, o comportamente de seus nós filhos não será afetado
