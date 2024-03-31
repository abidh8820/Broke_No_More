# Broke No More: Deep Learning for Financial Forecasting

This project aims to predict stock prices in the Dhaka Stock Exchange (DSE) using Long Short-Term Memory (LSTM) models, a type of recurrent neural network. The goal is to develop an accurate predictive model that can assist investors in making informed investment decisions.

## Table of Contents

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Data](#data)
- [Preprocessing](#preprocessing)
- [Model](#model)
- [Experimental Setup](#experimental-setup)
- [Results](#results)
- [Conclusion and Future Work](#conclusion-and-future-work)
- [References](#references)

## Introduction

Accurately predicting stock prices is a challenging task in the field of finance. This project leverages the capabilities of recurrent neural networks (RNNs) and Long Short-Term Memory (LSTM) models to forecast stock market prices in the Dhaka Stock Exchange (DSE). By capturing temporal dependencies and patterns in historical stock data, the LSTM model aims to provide valuable insights for investment decisions.

## Methodology

The methodology employed in this project encompasses the following steps:

1. Data Acquisition
2. Data Preprocessing
3. Proposed RNN-LSTM Forecasting Model

## Data

The project utilizes historical price and volume data from companies listed on the Dhaka Stock Exchange (DSE). The data was obtained by scraping the official DSE website and covers the period from January 2008 to December 2022.

## Preprocessing

The acquired dataset underwent several preprocessing steps to ensure its suitability for training LSTM models. These steps included:

- Handling missing values (imputation or removal)
- Scaling numerical features (min-max scaling or standardization)
- Encoding categorical variables (one-hot encoding or label encoding)
- Creating relational features (e.g., yesterday's closing price)

## Model

The proposed method employs Long Short-Term Memory (LSTM) models, a specialized variant of Recurrent Neural Networks (RNNs), to forecast stock prices. LSTM models are well-suited for time series forecasting tasks due to their ability to capture and utilize temporal dependencies within sequential data.

The LSTM model was trained on input-output pairs created from the preprocessed data. The input consisted of sliding windows of past stock price observations, and the target output was the subsequent stock price value. The model was iteratively refined using a validation set, and its performance was evaluated on a separate testing set (December 2022 data).

## Experimental Setup

The experimental setup involved the following steps:

1. Data preparation (preprocessing)
2. LSTM model training and validation
3. Performance evaluation using metrics like Mean Squared Error (MSE), R-squared, and buy/sell recommendation accuracy

## Results

The results of the LSTM model's performance are presented in the report, including visualizations and analyses. While some companies in the DSE showed accuracy in the range of 60%, others demonstrated lower accuracy levels.

## Conclusion and Future Work

Although the LSTM-based approach did not achieve the desired accuracy levels, the report suggests exploring alternative techniques like transformer models and time encoding techniques (e.g., time2vec) for future work. These advancements may lead to more accurate and reliable stock price forecasting in the context of the Dhaka Stock Exchange and other financial markets.

## References

The references cited in the report are listed here:

1. Code for Data Scraping, GitHub Repository: https://github.com/diptomondal007/bdstockexchange
2. D. M. Q. Nelson, A. C. M. Pereira, and R. A. de Oliveira, "Stock market's price movement prediction with LSTM neural networks," 2017 International Joint Conference on Neural Networks (IJCNN), 2017.
3. Abdul Quadir Md, Sanjit Kapoor, Chris Junni A.V., Arun Kumar Sivaraman, Kong Fah Tee, Sabireen H., Janakiraman N., "Novel optimization approach for stock price forecasting using multi-layered sequential LSTM," Applied Soft Computing, Volume 134, 2023.
4. Chaojie Wang, Yuanyuan Chen, Shuqi Zhang, and Qiuhui Zhang, "Stock market index prediction using deep Transformer model," Expert Systems with Applications, Volume 208, 2022.
5. Project Google Colab Link: https://colab.research.google.com/drive/1kK0-O8nxK0aRfnfKoo8B-j_FxfmpgJ51?ts=648ed2b2

Please note that this readme provides an overview of the project and its components. For more detailed information, refer to the project report.
