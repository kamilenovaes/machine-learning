# 🧠 Conceitos: Regressão Linear Múltipla

Este arquivo contém um resumo teórico sobre o algoritmo de Regressão Linear Múltipla.

## 🎯 O que é?

A Regressão Linear Múltipla é uma extensão da Regressão Linear Simples. Em vez de usar apenas uma variável de entrada para fazer uma previsão, ela utiliza **múltiplas variáveis de entrada** (features) para prever um resultado numérico contínuo.

A fórmula matemática se expande para incluir os novos coeficientes:

`y = b₀ + b₁*x₁ + b₂*x₂ + ... + bₙ*xₙ`

Onde:
- **`y`**: O valor que queremos prever.
- **`x₁, x₂, ..., xₙ`**: Os valores das nossas múltiplas variáveis de entrada.
- **`b₁, b₂, ..., bₙ`**: Os coeficientes para cada variável de entrada. Cada `b` representa o impacto daquela variável `x` na previsão `y`, mantendo todas as outras variáveis constantes.
- **`b₀`**: O intercepto, que representa o valor de `y` quando todas as variáveis de entrada são zero.

## 🤔 Desafios e Suposições

Para que o modelo funcione bem, ele assume algumas condições:
1.  **Linearidade:** A relação entre cada variável de entrada e a saída é linear.
2.  **Independência:** As variáveis de entrada não devem ser altamente correlacionadas entre si (isso é chamado de **multicolinearidade** e pode confundir o modelo sobre qual variável é realmente importante).
3.  **Homocedasticidade:** A variância dos erros deve ser constante.
4.  **Normalidade dos Resíduos:** Os erros do modelo devem seguir uma distribuição normal.

## ✅ Quando usar?

- Quando você acredita que **múltiplos fatores** influenciam o resultado que você quer prever.
- **Exemplo:** Prever o preço de uma casa (`y`) usando o tamanho (`x₁`), o número de quartos (`x₂`), e a idade da casa (`x₃`).