# User Behavior Analysis & Funnel Optimization 

## Overview

This project was developed as part of the TripleTen Data Analytics Program and focuses on **user behavior analysis and conversion funnel optimization** for an e-commerce startup in the food industry.

The main objective was to understand the customer journey, identify drop-off points within the conversion funnel, and evaluate the impact of a design experiment (A/A/B test) on user behavior.

---

## Business Context

The startup aims to improve its overall conversion rate and user engagement within the application.

To achieve this, event logs were analyzed to reconstruct the user journey and build a conversion funnel, allowing identification of where users drop off during the process.

In addition, an A/A/B experiment was conducted to test a new app font design, comparing two control groups (A/A) against a test group (B), ensuring statistical reliability before any product decision.

---

## Technologies & Tools

* Python 3.x
* Pandas — data cleaning, transformation, and event aggregation
* Plotly — interactive funnel visualization and exploratory analysis
* SciPy (stats) — statistical hypothesis testing (Z-test for proportions)

---

## Technical Challenges Overcome

### Event Data Processing

* Handled raw event logs with inconsistent data types and timestamps.
* Extracted and standardized date-time features for time-based analysis.
* Filtered incomplete or unstable data to ensure analytical reliability.

### Conversion Funnel Analysis

* Reconstructed the user journey using event sequence:
  * `MainScreenAppear`
  * `OffersScreenAppear`
  * `CartScreenAppear`
  * `PaymentScreenSuccessful`
* Calculated conversion rates between each stage of the funnel.
* Identified the main drop-off point between the main screen and the offers screen.

### A/A/B Experiment Analysis

* Validated A/A groups to ensure statistical equivalence before testing.
* Compared control groups individually and combined against the test group.
* Applied **Bonferroni correction** to adjust for multiple hypothesis testing and reduce the risk of false positives.

---

## Key Insights

* Only 47% of users who reached the main screen proceeded to the offers screen, indicating a significant drop-off at the top of the funnel.
* Once users reached the payment stage, the conversion rate exceeded 95%, showing strong final-stage efficiency.
* The A/A/B experiment showed no statistically significant difference in user behavior, indicating that the font change did not impact conversion or engagement.

---

## Business Recommendations

* Focus optimization efforts on the transition between the main screen and offers screen, where the highest user loss occurs.
* Maintain a streamlined checkout experience, as the payment stage already shows strong performance.
* The proposed font change can be implemented safely, as it does not negatively impact user behavior.
* Prioritize further experiments targeting early-stage funnel engagement.

---

## Repository Structure

* `notebook.ipynb` — full analysis including data preprocessing, funnel analysis, and statistical testing
* `README.md` — project documentation

---
# Análise de Comportamento do Usuário e Otimização de Funil 

## Visão Geral

Este projeto foi desenvolvido como parte do programa de Análise de Dados da TripleTen e tem como foco a **análise de comportamento do usuário e otimização do funil de conversão** para uma startup do setor de alimentos.

O objetivo principal foi entender a jornada do usuário dentro do aplicativo, identificar pontos de abandono no funil de conversão e avaliar o impacto de um experimento de design (Teste A/A/B) no comportamento dos usuários.

---

## Contexto de Negócio

A startup busca aumentar sua taxa de conversão e melhorar a experiência do usuário dentro do aplicativo.

Para isso, foram analisados logs de eventos para reconstrução da jornada do usuário e construção de um funil de conversão, permitindo identificar em quais etapas ocorre maior perda de usuários.

Além disso, foi realizado um experimento A/A/B para testar uma nova fonte de design no aplicativo, comparando dois grupos de controle (A/A) com um grupo de teste (B), garantindo validade estatística antes de qualquer decisão de produto.

---

## Tecnologias e Ferramentas

* Python 3.x
* Pandas — limpeza, transformação e agregação de dados de eventos
* Plotly — visualização interativa do funil e análise exploratória
* SciPy (stats) — testes estatísticos de hipótese (Z-test para proporções)

---

## Desafios Técnicos Superados

### Processamento de Dados de Eventos

* Tratamento de logs brutos com inconsistências de tipos e timestamps.
* Extração e padronização de variáveis de data e hora para análise temporal.
* Filtragem de dados incompletos para garantir consistência e confiabilidade analítica.

### Análise do Funil de Conversão

* Reconstrução da jornada do usuário com base na sequência de eventos:
  * MainScreenAppear
  * OffersScreenAppear
  * CartScreenAppear
  * PaymentScreenSuccessful
* Cálculo das taxas de conversão entre cada etapa do funil.
* Identificação do principal ponto de abandono entre a tela principal e a tela de ofertas.

### Análise do Experimento A/A/B

* Validação dos grupos A/A para garantir equivalência estatística antes da comparação.
* Comparação dos grupos de controle individualmente e combinados com o grupo de teste.
* Aplicação da **correção de Bonferroni** para ajuste de múltiplas hipóteses e redução de falsos positivos.

---

## Principais Insights

* Apenas 47% dos usuários que acessam a tela principal avançam para a tela de ofertas, indicando um forte ponto de abandono no topo do funil.
* Após a etapa de pagamento, a taxa de conversão é superior a 95%, demonstrando alta eficiência na etapa final do processo.
* O experimento A/A/B indicou que a mudança de fonte não gerou impacto estatisticamente significativo no comportamento dos usuários.

---

## Recomendações de Negócio

* Focar otimizações na transição entre a tela principal e a tela de ofertas, onde ocorre a maior perda de usuários.
* Manter o fluxo de pagamento atual, já que apresenta alta taxa de conversão.
* A mudança de fonte pode ser implementada com segurança, pois não impacta negativamente o comportamento do usuário.
* Priorizar novos testes voltados para melhorias nas etapas iniciais do funil.

---

## Estrutura do Repositório

* `notebook.ipynb` — análise completa incluindo processamento de dados, construção do funil e testes estatísticos
* `README.md` — documentação do projeto

---
