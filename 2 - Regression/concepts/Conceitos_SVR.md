# 🧠 Conceitos: Support Vector Regression (SVR)

Este arquivo contém um resumo teórico sobre o algoritmo Support Vector Regression (SVR).

## 🎯 O que é?

A SVR é a versão de regressão do famoso algoritmo de classificação **Support Vector Machine (SVM)**. A principal ideia da SVR é diferente da regressão linear tradicional.

Em vez de tentar minimizar o erro entre a previsão e todos os pontos de dados, a SVR tenta ajustar a melhor linha (ou hiperplano) que se encaixa no **maior número de pontos de dados possível DENTRO de uma margem de erro definida**.

Imagine a linha de regressão como uma "rua". A SVR não se importa com os pontos que estão dentro da rua, apenas com os que estão fora. Os pontos que definem os limites dessa rua são chamados de **vetores de suporte**.

## 🤔 A Margem de Erro (Epsilon - ε)

A SVR tem um hiperparâmetro crucial chamado **epsilon (ε)**, que define a largura da "rua".
- O modelo só penaliza os erros para os pontos que caem **fora** dessa margem.
- Isso torna a SVR muito robusta a **outliers**, pois se um outlier estiver dentro da margem, ele será ignorado.


## ✅ Quando usar?

- Funciona bem em datasets com muitas features (alta dimensionalidade).
- É muito eficaz quando o número de features é maior que o número de amostras.
- É robusto a outliers, graças ao conceito da margem de erro.