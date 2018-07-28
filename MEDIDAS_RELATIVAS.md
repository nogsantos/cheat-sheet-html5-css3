# Html 5 and Css 3 Advanced tips

## Medidas Relativas

- px: É sempre um px
- %: Dependendo do contexto, pode ser à largura, à altura ou ao tamanho de fonte do elemento anterior (pai)
- rem: É baseada no tamanho padrão da fonte do navegador ou baseado no tamanho da fonte definida no html
- em: É baseada no tamanho da fonte do elemento que foi usada
- ch: A largura do caractere 0 (zero)
-- Vale notar que existem algumas fontes em que todos os caracteres têm a mesma largura, que são fontes conhecidas como monoespaçadas.

### Exemplificação das medidas `em` e `rem`

#### em

```css
p {
    font-size: 20px;
    margin: 1em;
}
```
nesse caso, os parágrafos terão uma margem de 20 pixels.

#### rem

```css
html{
    font-size: 25px;
}

p {
    margin: 1rem;
}
```
nesse caso todos os parágrafos terão 25 pixels de margem.
