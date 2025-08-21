# 🧠 Conceitos: Regressão com Árvore de Decisão

Este arquivo contém um resumo teórico sobre o algoritmo de Regressão com Árvore de Decisão.

## 🎯 O que é?

A Árvore de Decisão para regressão é um modelo que prevê um valor contínuo dividindo o conjunto de dados em subconjuntos menores e mais homogêneos. O modelo aprende uma série de "perguntas" (regras de decisão) baseadas nas features, criando uma estrutura de árvore.

Para fazer uma previsão, uma nova amostra percorre a árvore de cima para baixo. Em cada "nó" da árvore, uma pergunta é feita sobre uma de suas features. Dependendo da resposta, ela segue por um galho até chegar a uma "folha".

A previsão final é a **média de todos os valores de treino** que terminaram naquela folha.

## 🤔 Como funciona?

- O algoritmo divide o dataset em cada feature, buscando o ponto de corte que mais reduz a variância (ou o erro quadrático médio) dos dados.
- Ele repete esse processo de forma recursiva para cada novo subconjunto, criando os galhos e nós da árvore.
- O processo para quando um critério de parada é atingido (ex: profundidade máxima da árvore, número mínimo de amostras em uma folha).


## ✅ Vantagens e Desvantagens

- **Vantagens:** Fácil de interpretar e visualizar. Não exige escalonamento de features.
- **Desvantagens:** Propenso a **overfitting** (uma única árvore pode crescer demais e decorar os dados). Pequenas variações nos dados podem gerar uma árvore completamente diferente.