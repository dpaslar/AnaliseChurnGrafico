# Analise Churn Grafico
Análise de Churn de Clientes com Machine Learning
Objetivo
Este projeto tem como foco prever a evasão de clientes (churn) em uma empresa de telecomunicações, utilizando técnicas de Machine Learning supervisionado. A previsão de churn é essencial para identificar clientes em risco e reduzir perdas financeiras.

Técnicas Utilizadas
Pré-processamento de dados

Tratamento de valores ausentes

Codificação de variáveis categóricas

Normalização dos dados

Balanceamento da base

Utilização de SMOTE para lidar com o desbalanceamento da variável alvo (Churn)

Modelos aplicados

Regressão Logística

Random Forest

Avaliação de desempenho

Acurácia, Precision, Recall, F1-Score

Matriz de confusão

ncipais Insights (baseados nos gráficos)
Distribuição da variável Churn

Cerca de 26% dos clientes abandonaram a empresa.

Base desbalanceada → justificativa para uso de SMOTE.

Correlação de churn com contrato mensal

Clientes com contrato mensal apresentaram taxas significativamente maiores de churn.

Já contratos anuais ou bianuais retêm mais clientes.

Serviços extras e churn

Clientes sem serviços adicionais (como segurança online ou backup) apresentaram maior probabilidade de saída.

Isso sugere que quanto mais serviços o cliente assina, menor a chance de churn (efeito lock-in).

Total de gastos (TotalCharges)

Clientes que gastam menos tendem a sair mais.

Pode indicar que novos clientes (baixo histórico de pagamento) têm maior risco.

Internet e churn

Clientes sem internet ou com conexão DSL saem mais.

Fibra ótica, apesar de ser melhor, também tem alta taxa de churn — pode estar relacionada a preço.

Modelos de ML

Random Forest teve melhor desempenho geral, principalmente no recall (essencial para churn).

A Regressão Logística também performou bem e é mais interpretável.

Resultados
Modelo	Acurácia	Precision	Recall	F1-Score	ROC AUC
Regressão Logística	~0.81	~0.71	~0.66	~0.68	~0.85
Random Forest	~0.85	~0.78	~0.73	~0.75	~0.88
