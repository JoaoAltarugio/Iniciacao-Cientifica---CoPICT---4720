# Aprendizado Profundo para Previsão em Séries Temporais: Um Estudo Comparativo entre Modelos de Redes Neurais

Este repositório contém o código-fonte do projeto de Iniciação Científica e Tecnológica (ICTSR) **"Aprendizado Profundo para Previsão em Séries Temporais: Um Estudo Comparativo entre Modelos de Redes Neurais"**, desenvolvido por João Eduardo Batelochi Altarugio, sob orientação do Prof. Dr. Alexandre Luis Magalhaes Levada na Universidade Federal de São Carlos (UFSCar). O projeto foi fomentado pela Coordenadoria dos Programas de Iniciação Científica e Tecnológica.

---

## Resumo do Projeto

A análise de séries temporais financeiras é crucial para a compreensão e previsão do comportamento do mercado, auxiliando a tomada de decisões estratégicas. Neste contexto, técnicas de aprendizado profundo (deep learning) se mostram promissoras devido à sua capacidade de capturar padrões complexos e não lineares nos dados.

O estudo explora dois cenários de aprendizado profundo para a previsão em séries temporais:

- **Cenário (i):** Modelos univariados baseados em Redes Neurais Convolucionais (CNNs) e Redes de Memória de Longo Prazo (LSTMs). Estes modelos usam uma janela de 5 dias para prever os 5 dias seguintes.

- **Cenário (ii):** Um modelo multivariado LSTM, que incorpora variáveis qualitativas de análise de sentimento de notícias macroeconômicas. Para isso, utiliza o modelo de linguagem FinBERT-pt-Br em notícias da base de dados GDELT. Este modelo usa uma janela de 8 dias para prever o dia seguinte.

Os experimentos foram realizados com dados do ETF BOVA11, coletados via Yahoo Finance, e mais de 300 mil notícias macroeconômicas. Os resultados indicaram que os modelos CNN e LSTM superaram a linha de base (que simplesmente repetia a janela de entrada). Além disso, a adição da análise de sentimentos melhorou a capacidade preditiva do modelo multivariado.

---

## Conteúdo do Repositório

- **Coleta e Pré-processamento de Dados:** Scripts para coleta de dados financeiros do ETF Ibovespa usando a API do Yahoo Finance e coleta de notícias macroeconômicas do projeto GDELT via Google Cloud BigQuery.

- **Anotação de Sentimento:** Código para análise de sentimento das notícias utilizando o modelo de linguagem FinBERT-pt-Br.

- **Arquiteturas de Modelos:** Implementações das arquiteturas de redes neurais univariadas e multivariadas, incluindo CNN e LSTM, prontas para uso.

---

## Observação sobre os dados

Embora os códigos de coleta de dados e as arquiteturas dos modelos estejam disponíveis, a base de dados completa de notícias macroeconômicas não pôde ser hospedada neste repositório do GitHub devido ao seu grande volume. No entanto, os scripts de coleta permitem que a base de dados seja replicada para reprodução dos experimentos.
