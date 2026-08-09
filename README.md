# Previsão de Risco Financeiro: VaR e Expected Shortfall (ES)

Este repositório contém uma implementação robusta em R para a estimativa de medidas de risco financeiro — **Value at Risk (VaR)** e **Expected Shortfall (ES)**. 

O script utiliza uma abordagem de janela móvel para realizar previsões um passo à frente aplicando diversas modelagens econométricas e estatísticas a séries temporais financeiras.

## Modelos Implementados

O código realiza previsões empíricas, paramétricas e baseadas em Simulação Histórica Filtrada (FHS) utilizando os seguintes modelos:

*   **Simulação Histórica:** Tradicional e Filtrada (FHS).
*   **Modelos Paramétricos:** Distribuições Normal e t-Student.
*   **Família GARCH:** sGARCH, eGARCH, iGARCH, fiGARCH e NAGARCH (distribuições Normal e t-Student).
*   **CAViaR (Conditional Autoregressive Value at Risk):** Abordagens Assimétrica (Asymmetric Slope) e Simétrica (Symmetric Absolute Value).
*   **Teoria dos Valores Extremos (EVT):** Abordagem Peaks Over Threshold (POT) com a Distribuição Generalizada de Pareto (GPD).
*   **Modelos GAS (Generalized Autoregressive Score):** Distribuições Normal e t-Student.
*   **Modelos MSGARCH (Markov-Switching GARCH):** Mudança de regime para distribuições Normal e t-Student.

## Pré-requisitos

Para executar este código, você precisará do `R` instalado e dos seguintes pacotes:

```R
install.packages(c("tidyverse", "readxl", "quantmod", "stringr", "MASS", "ggplot2", "rugarch", "eva", "MSGARCH", "GAS"))
