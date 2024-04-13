# Neural Network LSTM Project
>### META Stock Prediction <br />
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/META.jpeg" width="600" height="280"> <br /> 
<br /> 

#### Business Objective
To predict the movement of the FB stock price based on previous 21 days of trading of three stocks: META, AMZN and INTC. <br /> 
<br /> 

#### Data Collection
The dataset is obtained from yahooFinance. <br /> 
<br />

#### Exploratory Data Analysis
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Stocks_Adj_Closing.png" width="600" height="420"> <br /> 
<br />
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Stocks_Volume.png" width="600" height="420"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Regression.png" width="500" height="430"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Heatmap.png" width="400" height="320"> <br /> 
<br /> 
#### Models Building
LSTM Architecture <br />

1. Activation function: ReLu and Sigmoid <br />

2. Cross-validation: Random Search is used to find the best model. <br />

  search_space = {"lstm_size":     np.linspace(50, 200, 5, dtype = int), <br />
                "dropout":       np.linspace(0, 0.4, 2), <br />
                "learning_rate": np.linspace(0.004, 0.01, 4)} <br />

- LSTM size refers to the number of units in the layer that has a memory state and a gate mechanism that controls the flow of information <br />
- Dropout refers to the nodes that are dropped by a probability to prevent overfitting <br />
- Learning rate refers to the magnitude of weight updates for minimising the network's loss function <br />

#### Models Evaluation
Best model: <br /> 

<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Model_Architecture.png" width="500" height="300"> <br /> 
<br /> 

Evaluation: <br />
<br />
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Classification_report.png" width="400" height="300"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Confusion_matrix.png" width="300" height="250"> <br /> 
<br /> 
