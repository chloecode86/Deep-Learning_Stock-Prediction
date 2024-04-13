# Classification Project
>### AML Prediction <br />
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/META.jpeg" width="600" height="280"> <br /> 
<br /> 

#### Business Objective
To predict the movement of the FB stock price based on previous 21 days of trading of three stocks: META, AMZN and INTC.
<br /> 

#### Data Collection
The dataset is obtained from yahooFinance. <br /> 
<br />

#### Exploratory Data Analysis
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Stocks_Adj_Closing.png" width="650" height="380"> <br /> 
<br />
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Stocks_Volume.png" width="400" height="300"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Regression.png" width="600" height="530"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Heatmap.png" width="600" height="530"> <br /> 
<br /> 
#### Models Building
#####LSTM Architecture <br />

Activation function: ReLu and Sigmoid <br />

Cross-validation: Random Search is used to find the best model. <br />

search_space = {"lstm_size":     np.linspace(50, 200, 5, dtype = int), <br />
                "dropout":       np.linspace(0, 0.4, 2), <br />
                "learning_rate": np.linspace(0.004, 0.01, 4)} <br />

- LSTM size refers to the number of units in the layer that has a memory state and a gate mechanism that controls the flow of information <br />
- Dropout refers to the nodes that are dropped by a probability to prevent overfitting <br />
- Learning rate refers to the magnitude of weight updates for minimising the network's loss function <br />

#### Models Evaluation
Best model: <br /> 

<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Model_Architecture.png" width="600" height="530"> <br /> 
<br /> 

Evaluation: <br />
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Classification_report.png" width="600" height="530"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Deep-Learning_Stock-Prediction/blob/main/image/Confusion_matrix.png" width="600" height="530"> <br /> 
<br /> 
4. SVC <br />
   - Recall : 0.97 <br />
<img src="https://github.com/chloecode86/Classification-AML/blob/main/image/Confusion_matrix_SVC.png" width="300" height="250"> <br /> 
<br /> 
Since the cost of not detecting true money laundering cases (false negatives) is high, Recall (also known as Sensitivity or True Positive Rate) is the most important metric for evaluation. SVC model has given the best result.
