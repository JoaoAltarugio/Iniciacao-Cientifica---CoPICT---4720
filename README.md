# Iniciacao-Cientifica---CoPICT---4720

Previsão de Séries Temporais Financeiras com Deep Learning

Este repositório contém a implementação de modelos de deep learning para previsão de séries temporais financeiras, com foco no ETF BOVA11. O projeto utiliza arquiteturas de redes neurais como LSTM, CNN e, em breve, Transformers, para prever os preços futuros do ativo com base em dados históricos. O código foi desenvolvido em Python utilizando os frameworks Keras e PyTorch.

Descrição do Projeto
O objetivo deste projeto é comparar diferentes arquiteturas de redes neurais para prever a tendência de preços do ETF BOVA11. Modelos como Redes Neurais Recorrentes (RNN), LSTMs, CNNs e modelos baseados em Transformers serão comparados em termos de desempenho, com foco na acurácia das previsões de preços futuros.

Dados Utilizados
Os dados utilizados para treinamento e teste do modelo foram extraídos da API do Yahoo Finance, cobrindo mais de 17 anos de históricos diários de preços do ETF BOVA11. O conjunto de dados contém 6360 amostras de valores de pregão, e foi enriquecido com métricas adicionais, como:

MA7 (Média Móvel de 7 dias)

EMA (Média Exponencialmente Ponderada)

FFT_10 (Transformada Rápida de Fourier de 10 períodos)

ARIMA_Pred (Previsões ARIMA)

Arquiteturas de Redes Neurais
LSTM (Long Short-Term Memory): Escolhida pela sua capacidade de capturar dependências de longo prazo em séries temporais.

CNN (Redes Neurais Convolucionais): Adaptada para prever padrões temporais, capturando variações locais e rápidas.

Transformer (em progresso): Planeja-se a implementação e comparação de redes baseadas em Transformer como BERT e GPT para a previsão de séries temporais financeiras.
