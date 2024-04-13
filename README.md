# Neutral Network Project
>### Stock Prediction <br />
<img src="https://github.com/chloecode86/Classification-AML/blob/main/image/AML_image.jpeg" width="600" height="280"> <br /> 
<br /> 

#### Business Objective
To detect money laundering based on various features.
<br /> 

#### Data Collection
The dataset is obtained from Kaggle. <br /> 
<br />
• Time and Date <br />
• Sender and Receiver Account Details <br />
• Amount <br />
• Payment Type (eg. credit card, debit card, cash, ACH transfers, cross-border, and cheque) <br />
• Sender and Receiver Bank Location <br />
• Payment and Receiver Currency <br />
• 'Is Suspicious' Feature (Binary indicator) <br />
• Type (Classifies typologies) <br />
<br />
#### Exploratory Data Analysis
<img src="https://github.com/chloecode86/Classification-AML/blob/main/image/Laundering_type.png" width="650" height="380"> <br /> 
<br />
<img src="https://github.com/chloecode86/Classification-AML/blob/main/image/Payment_type.png" width="400" height="300"> <br /> 
<br /> 
<img src="https://github.com/chloecode86/Classification-AML/blob/main/image/Correlation_matrix.png" width="600" height="530"> <br /> 
<br /> 
#### Models Evaluation
1. Naive Bayes <br />
   - Recall : 0.47 <br />
2. Logistic Regression <br />
   - Recall : 0.56 <br />
3. KNN <br />
   - Recall : 0.96 <br />
4. SVC <br />
   - Recall : 0.97 <br />
<img src="https://github.com/chloecode86/Classification-AML/blob/main/image/Confusion_matrix_SVC.png" width="300" height="250"> <br /> 
<br /> 
Since the cost of not detecting true money laundering cases (false negatives) is high, Recall (also known as Sensitivity or True Positive Rate) is the most important metric for evaluation. SVC model has given the best result.
