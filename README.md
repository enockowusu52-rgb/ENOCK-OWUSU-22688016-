# Project Title
Regression and Classification with Multi-Architecture (Deep) Neural Networks 

## Description
This project investigates and compares the performance of multiple deep learning architectures—Deep Neural Networks (DNN), Convolutional Neural Networks (CNN), Long Short-Term Memory networks (LSTM), and a custom CNN–LSTM hybrid—on two different tasks:

1. **Jena Climate Dataset (Regression & Classification)**  
   - Regression: Predict temperature 24 hours ahead using a 120-hour lookback window.  
   - Classification: Categorise future temperature into four classes (Cold, Cool, Mild, Warm).

2. **MNIST Dataset (Classification)**  
   - Classify handwritten digits (0–9) using DNN, CNN, and LSTM-based approaches.

The project begins with data preprocessing and exploratory analysis, followed by the design and training of baseline models (DNN), advanced models (CNN, LSTM), and a hybrid architecture. Performance is evaluated using metrics such as MAE, RMSE, R² (for regression), and accuracy and macro-F1 (for classification). Additional analyses include hyperparameter sensitivity, visualization of predictions, and statistical comparison using the Diebold–Mariano test.

Key findings highlight the importance of **inductive bias** and **task-architecture alignment**:
- CNNs perform best for image data due to spatial feature extraction.
- LSTMs perform well for sequential data due to long-term dependency modelling.
- The CNN–LSTM hybrid effectively captures both local and global temporal patterns in climate data.

## How to run
1. Install required packages (see Requirements section).
2. Open the `.qmd` (Quarto) or `.Rmd` (R Markdown) file in RStudio.
3. Ensure the dataset paths are correct (Jena dataset and MNIST via Keras).
4. Click **Render** to compile the full report (HTML/PDF).
5. All results, tables, and plots will be generated automatically.

## Requirements
**R version:** R 4.5.3
**Packages used:**
  - `keras`
  - `tensorflow`
  - `tidyverse`
  - `ggplot2`
  - `dplyr`
  - `tidyr`
  - `lubridate`
  - `forecast`
  - `reticulate`

> Note: TensorFlow backend was properly installed via: 
install.packages("keras3")
library(keras3)
install_keras()

## Author
Enock Owusu (Mr.)
