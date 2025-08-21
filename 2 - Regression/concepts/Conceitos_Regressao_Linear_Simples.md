# 🧠 Conceitos: Regressão Linear Simples

Este arquivo contém um resumo teórico sobre o algoritmo de Regressão Linear Simples, abordado na seção 2 do curso.

## 🎯 O que é?

A Regressão Linear Simples é um algoritmo de aprendizado supervisionado usado para **prever um valor numérico contínuo**. O objetivo é encontrar a melhor **linha reta** que descreve a relação entre uma única variável de entrada (independente, `X`) e uma variável de saída (dependente, `y`).

A fórmula matemática que descreve essa linha é:

`y = b₀ + b₁ * x`

Onde:
- **`y`**: O valor que queremos prever.
- **`x`**: O valor da nossa variável de entrada.
- **`b₁`**: O **coeficiente** (ou peso), que representa a inclinação da linha. Ele nos diz o quanto `y` muda para cada unidade de mudança em `x`.
- **`b₀`**: O **intercepto**, que representa o valor de `y` quando `x` é igual a zero.

## 🤔 Como o modelo "aprende"?

O treinamento do modelo consiste em encontrar os melhores valores para `b₀` e `b₁` que minimizem a distância entre a linha de regressão e os pontos de dados reais. O método mais comum para fazer isso é o **Método dos Mínimos Quadrados** (Ordinary Least Squares - OLS), que busca minimizar a soma dos erros ao quadrado.

![Imagem de Regressão Linear](https://i.imgur.com/yUgk3D8.png)
*Nesta imagem, a linha azul é o nosso modelo, e as linhas vermelhas representam o erro (a distância) entre a previsão e o valor real para cada ponto.*

## ✅ Quando usar?

- Para prever valores contínuos (ex: prever o salário de uma pessoa com base nos anos de experiência, prever o preço de uma casa com base no seu tamanho).
- Quando há uma suspeita de que a relação entre as duas variáveis é linear (pode ser verificada com um gráfico de dispersão).

## ⚠️ Limitações

- Funciona bem apenas com **relações lineares**. Se a relação for curva, o modelo não terá um bom desempenho.
- É sensível a **outliers** (valores muito discrepantes), que podem "puxar" a linha de regressão para longe do ideal.
- Só consegue analisar a relação entre **duas variáveis** (uma de entrada e uma de saída). Para mais variáveis de entrada, usamos a Regressão Linear Múltipla.