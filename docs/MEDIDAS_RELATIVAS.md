# Medidas Relativas

[<-- Voltar](../README.md)

#### Comprimentos Absoluto

As unidades de comprimento absoluto são fixas e, qualquer uma dessas medidas quando utilizadas, aparecerá exatamente como seus tamanhos definidos.

- `px`: É sempre um *px*
- `cm`: Centimetros
- `mm`: milimetros
- `in`: inches *(1in = 96px = 2.54cm)*
- `pt`: points *(1pt = 1/72 of 1in)*
- `pc`: picas *(1pc = 12 pt)*

#### Comprimentos Relativos

Unidades de comprimento relativo especificam um comprimento em relação a outra propriedade de comprimento e escalonam melhor entre diferentes meios de renderização.

- `rem`: É baseada no tamanho padrão da fonte do navegador ou baseado no tamanho da fonte definida no html
- `em`: É baseada no tamanho da fonte do elemento que foi usada
- `ch`: A largura do caractere *0 (zero)*
  - Vale notar que existem algumas fontes em que todos os caracteres têm a mesma largura, que são fontes conhecidas como monoespaçadas.
- `%`: Dependendo do contexto, pode ser à largura, à altura ou ao tamanho de fonte do elemento anterior (pai)
- `vw`: Relativo a *1%* da **largura** da *janela de exibição*\* do navegador
- `vh`: Relativo a *1%* da **altura** da *janela de exibição*\* do navegador
- `vmin`: Relativo a *1%* da *janela de exibição*\*, menor dimensão
- `vmax`: Relativo a *1%* da *janela de exibição*\*, maior dimensão

> * janela de exibição = Tamanho da janela do navegador. Se a janela de visualização tiver *50cm* de largura, *1vw* = *0,5cm*.

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
