# Energy-Consumption-Forecasting
*A project to support the pursuit of Net Zero. Collab between myself (Nissan) and Newcastle University.*

## Introduction
With the recent introduction of data visualisation software at Nissan, awareness of energy consumption is being observed on a wider scale than ever before. Coupled with exponentially increasing energy costs across the UK, awareness of company spending on energy is also higher than ever. Advancement within the company to install measuring infrastructure has made it possible to now collect, analyse and present data rapidly, in ways that were previously impossible. This report aims to support Nissan in the next stage of their digital intelligence development journey to look at future forecasting methods that can make predictions for energy consumption, allowing the company to make more proactive decisions. 

## Purpose
The purpose of this project was to build and train a machine learning model that could accurately predict future energy consumption within the Nissan Paintshop, based on previous data gathered across the site over a 15 month period.

## Method
In this work, three different machine learning algorithms were modelled to develop a time-series power forecast. The proposed models were Long Short-Term Memory (LSTM), the Gated Recurrent Unit (GRU) and the Recurrant Neural Network (RNN). These models were selected because they are traditionally suited to this type of sequence-dependent, time-series analysis. 
Prior to the models being applied, the data was amalgamated from various sources into a single file using Python within a Jupyter notebook (Appendix A). This was then cleaned and pre-processed using cyclical encoding and normalization methods (Appendix B) so that it could be further explored. The data was segregated into training, validation and test sets, which provided the opportunity for an unseen data set to be used when gathering results to ensure an unbiased experiment. 

## Result
The initial results were recorded and improved further by adjusting hyperparameters, namely the learning rate and number of epochs. The final results showed an improvement by increasing the number of epochs (from 15 to 50) and maintaining the same learning rate (0.001). Mean squared error was used to compare the success of the three models. The GRU model performed the best, as expected, as this model is well suited to smaller time-series datasets such as this. 
Nissan has never previously collected data of this volume or carried out data analysis on such a large scale. Whilst the company have previously carried out some machine learning activities for action recognition and categorisation (for identifying defects within vehicles in real-time), forecasting is a novel concept for the company. It is proposed that the activity is rolled out across the wider plant in the near future, as the raw energy data already exists for the other shops. 
