# Previsão de Default de Cartão de Crédito usando Regressão Logística

Este repositório contém uma análise detalhada do dataset de default em pagamentos de cartão de crédito por clientes de Taiwan, em 2005, disponível no [Kaggle](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata). O objetivo principal do projeto é realizar uma análise exploratória dos dados e construir um modelo de aprendizado de máquina para prever a probabilidade de default (inadimplência) de pagamento, utilizando o método de Regressão Logística.

## 📁 Sobre o Dataset

O dataset foi obtido no Kaggle e contém informações sobre o histórico de pagamentos de clientes de cartões de crédito em Taiwan. As variáveis incluem:

* Dados demográficos: sexo, idade, estado civil, nível educacional.
* Limite de crédito: limite total do cartão de crédito.
* Histórico de pagamento: status de pagamento dos últimos seis meses.
* Montante das faturas: valores das faturas de cada mês.
* Pagamentos realizados: valores dos pagamentos efetuados nos últimos meses.
* A variável alvo é **`ira_dar_calote`**

`1` indica que o cliente não efetuou o pagamento do cartão (inadimplente),
`0` indica que o cliente está adimplente.

## 🛠️ Estrutura do Projeto

1. **Importação e Preparação dos Dados**: 
   - Carregamento dos dados e verificação de tipos, valores ausentes e estatísticas iniciais.
   - Pré-processamento para padronização e limpeza dos dados, garantindo a qualidade para análise e modelagem.

2. **Análise Exploratória dos Dados (EDA)**:
   - Visualizações para entender a distribuição das variáveis numéricas e categóricas.
   - Análise de correlações entre variáveis, incluindo gráficos como heatmaps, boxplots e count plots.
   - Insights sobre padrões de pagamento e perfil de clientes inadimplentes versus adimplentes.

3. **Modelagem com Regressão Logística**:
   - Implementação de um modelo de Regressão Logística para prever o *default* no pagamento.
   - Avaliação do modelo com métricas como Acurácia, Precisão e *Recall*.
   - Interpretação dos resultados e ajuste de hiperparâmetros para melhorar a performance.

## 📊 Principais Análises

- **Distribuição de Limite de Crédito**: Exploramos a distribuição de limite de crédito entre clientes e identificamos que limites mais altos geralmente estão associados a clientes com melhor histórico de pagamento.
- **Padrões de Pagamento**: Analisamos o status de pagamento mensal e a frequência de inadimplência, indicando que clientes com histórico recente de atraso têm maior probabilidade de *default*.
- **Fatores Demográficos**: Variáveis como educação e estado civil foram analisadas em relação ao *default*, revelando tendências interessantes que podem influenciar na concessão de crédito.

## 📈 Resultados do Modelo

O modelo de Regressão Logística conseguiu prever a inadimplência com uma boa taxa de acerto, destacando-se como uma abordagem eficaz para este tipo de problema de classificação binária. Foram utilizadas métricas como *accuracy*, *precision* e *recall* para avaliar o desempenho do modelo, que apresentou resultados satisfatórios na maioria das métricas.

## 📂 Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/leovnoliveira/ML-logistic-regression-credit-card-default.git

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt

3. Execute o notebook ou script principal para visualizar a análise completa e os resultados.

 ## 🔍 Conclusão
Este projeto demonstrou o uso de uma abordagem de análise exploratória e modelagem com Regressão Logística para prever o default de clientes de cartão de crédito. Através das visualizações e do modelo preditivo, conseguimos obter insights valiosos sobre o perfil de clientes com maior risco de inadimplência, oferecendo uma base para decisões de crédito mais informadas.

