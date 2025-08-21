# 🧠 Conceitos: Regressão Polinomial

Este arquivo contém um resumo teórico sobre o algoritmo de Regressão Polinomial.

## 🎯 O que é?

A Regressão Polinomial é um tipo de regressão linear que modela a relação entre a variável de entrada `x` e a saída `y` como um **polinômio de n-ésimo grau**. Ela é usada quando a relação entre os dados não é uma linha reta, mas sim uma **curva**.

Apesar do nome, ela é considerada um caso especial de regressão linear, pois ainda estamos criando uma equação linear, mas as *features* (variáveis de entrada) são potências da variável original (`x`, `x²`, `x³`, etc.).

A fórmula matemática é:

`y = b₀ + b₁*x + b₂*x² + ... + bₙ*xⁿ`

Onde:
- **`n`** é o **grau do polinômio**. Um grau 2 cria uma parábola, um grau 3 uma curva cúbica, e assim por diante.

## 🤔 Overfitting (Sobreajuste)

O maior desafio da Regressão Polinomial é escolher o grau certo.
- **Grau baixo (ex: 1):** O modelo pode ser simples demais e não capturar a tendência dos dados (**underfitting**).
- **Grau muito alto:** O modelo pode se ajustar perfeitamente aos dados de treino, mas falhar em generalizar para novos dados, pois ele "decorou" o ruído em vez de aprender a tendência (**overfitting**).

![Imagem de Overfitting](https://i.imgur.com/38b9Aop.png)
*A linha verde (grau alto) se ajusta perfeitamente aos pontos de treino, mas provavelmente fará previsões ruins para novos pontos.*

## ✅ Quando usar?

- Quando um gráfico de dispersão mostra claramente que a relação entre as variáveis segue uma curva.
- Para capturar relações mais complexas que a regressão linear simples não consegue modelar.