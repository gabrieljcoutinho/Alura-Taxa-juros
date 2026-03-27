# Projeto: Cálculo de Juros Compostos em JavaScript

## Descrição
Este projeto implementa uma função que calcula o valor final de um investimento ou dívida com base em **juros compostos**.

A fórmula utilizada é:

- M = C × (1 + i)^t

Onde:
- M = montante final
- C = capital inicial (valor)
- i = taxa de juros (em decimal)
- t = tempo

---

## Código

```javascript
const calculaJuros = (valor, juros, tempo) => {
    let taxaJuros = (juros / 100) + 1;
    return valor * Math.pow(taxaJuros, tempo);
}

console.log(calculaJuros(1000, 5, 2));
