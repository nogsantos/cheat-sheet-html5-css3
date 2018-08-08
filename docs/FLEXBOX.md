# Flexbox

[<-- Voltar](../README.md)

O `flexbox` é uma dentre várias outras especificações que estão surgindo no CSS para facilitar nosso trabalho com layout e deixar o código mais simples, a qual permite termos esse controle a partir de um elemento pai.

[Exemplo 1](../src/flexbox.html)

[Exemplo 2](../src/flexbox/)

- `display: flex`: ativa o flexbox no elemento;
- `align-items`: distribui verticalmente os elementos dentro de um container flex;
- `justify-content`: distribuir os elementos espaçadamente dentro do container;
- `flex-direction`: permite inverter o align-items;
- `order`: muda a ordem dos elementos;
- `flex`: indica a proporção do tamanho dos elementos. Ele é um atalho para mais três propriedades:
    - `flex-grow`: determina quanto o elemento deve crescer;
    - `flex-shrink`: determina quanto o elemento deve diminuir;
    - `flex-basis`: determina o tamanho mínimo do elemento.
