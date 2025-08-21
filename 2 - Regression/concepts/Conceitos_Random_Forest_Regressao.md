# 🧠 Conceitos: Regressão com Random Forest

Este arquivo contém um resumo teórico sobre o algoritmo de Regressão com Random Forest.

## 🎯 O que é?

Random Forest é um algoritmo de **ensemble learning**, o que significa que ele combina múltiplos modelos para obter uma previsão melhor e mais estável. Especificamente, ele constrói **muitas Árvores de Decisão** durante o treinamento.

Para fazer uma previsão de regressão, cada árvore na floresta faz sua própria previsão individual. A previsão final do Random Forest é a **média das previsões de todas as árvores**.

## 🤔 A "Mágica" da Aleatoriedade

O nome "Random Forest" vem de duas fontes de aleatoriedade que o algoritmo usa para evitar o overfitting das árvores individuais:

1.  **Amostragem Aleatória de Dados (Bootstrap):** Cada árvore é treinada em uma amostra aleatória (com reposição) do conjunto de dados original. Isso significa que cada árvore vê uma versão ligeiramente diferente dos dados.
2.  **Seleção Aleatória de Features:** Em cada nó da árvore, em vez de verificar todas as features para encontrar a melhor divisão, o algoritmo seleciona apenas um subconjunto aleatório de features.

Essa dupla aleatoriedade garante que as árvores na floresta sejam bem diferentes umas das outras.

## ✅ Por que usar?

- **Alta Precisão:** Geralmente fornece resultados muito precisos e é um dos algoritmos mais populares.
- **Robusto a Overfitting:** Ao tirar a média de muitas árvores, ele corrige o principal problema de uma única árvore de decisão.
- **Importância das Features:** Ele consegue nos dizer quais features foram mais importantes para a previsão.