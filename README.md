# analysis-of-mental-health

Olá! Neste projeto, analisei um conjunto de dados sobre saúde mental no ambiente de trabalho, com o objetivo de prever a probabilidade de uma pessoa buscar tratamento para questões de saúde mental, com base em características pessoais e profissionais presentes no dataset.

# 1. Análise Exploratória de Dados (EDA): 🔍
Realizei uma análise cuidadosa das variáveis, identificando e corrigindo erros nos dados, como outliers e valores nulos. Percebi que, em alguns casos, remover valores ausentes automaticamente pode não ser o ideal, pois a ausência em si pode carregar informações relevantes para o modelo.

Apliquei One-Hot-Encoding nas variáveis qualitativas nominais e Ordinal Encoding nas qualitativas ordinais.

# 2. Modelagem Preditiva: 🤖
Como a variável-alvo era binária, utilizei regressão logística (pela biblioteca statsmodels). Também me atentei às suposições estatísticas da regressão logística.

# 3. Teste de Significância (aplicado aos coeficientes estimados pelo modelo): 📈
Hipótese nula (H₀): O coeficiente é igual a zero.
Hipótese alternativa (H₁): O coeficiente é diferente de zero.

Esse teste de hipótese ajuda a verificar se as variáveis preditoras são estatisticamente significativas (coeficientes ≠ 0) para a variável-alvo.

# 4. Seleção de Variáveis: ✂️
Eliminei as variáveis com p-value > 0.05. O modelo final utilizou apenas 6 variáveis preditoras, extraídas de um conjunto inicial de 35, e obteve uma acurácia de 82%. 🔥

# Resultados:
Os principais fatores que afetaram a decisão de buscar tratamento para questões de saúde mental foram:
- Interferência negativa no trabalho;🧠
- Histórico familiar de doenças mentais;🧬
- Gênero (ser homem diminui a probabilidade de buscar tratamento);👨‍⚕️
- A empresa oferece benefícios de saúde mental e o indivíduo conhece esses benefícios;🏥
- O indivíduo está disposto a discutir problemas de saúde mental com os colegas de trabalho.💬

Esses fatores fazem total sentido quando refletimos sobre a realidade do ambiente de trabalho e as dificuldades enfrentadas por quem lida com questões de saúde mental.
