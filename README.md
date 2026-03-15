# Fraud Detection in Financial Transactions using Logistic Regression
This project focuses on detecting fraudulent financial transactions using the PaySim synthetic dataset, which simulates real-world mobile money transfer behavior. The project works with unbalanced data (only 0.2% flagged as Fraud) and samples 10,000 entries from the dataset-- which originally contains over a million entries. 
<br>
Dataset used: https://www.kaggle.com/datasets/ealaxi/paysim1
<br>

### Exploratory data analysis (EDA)
<ul>
  <li>Transaction types generally and ones used in fraudulent transactions.</li> 
  <ul><li>Found that fraud rates are generally only under transfers and cash outs.</li>
  <li>Checked fraud distribution over the both types.</li></ul>
  <li>Plotted a correlation matrix over the main features.</li>
  <li>Plotted transactions over a histogram.</li>
  <ul><li>Peaks around medium to high amount transactions.</li></ul>
  <li>Box Plot to show that fraudulent transactions generally are of higher amounts.</li>
</ul>

### Methodology 
<ul>
  <li>Divided the sampled dataset into 70-30 (70% for training and 30% for testing).</li>
  <li>Scaled numeric features using a Standard Scaler and classified categorical features into binary values using OneHotEncoding.</li>
  <li>Made use of Logistic regression to predict target (fraud)</li>
  <li>Evaluated the model using confusion matrix and classification report</li>
</ul>
<br>
The model reached around 85% accuracy. Currently, the model prioritizes recall over precision- can help minimize financial loss from missed frauds (Recall is 95%). However still needs improvements over precision. 
<br>

#### Future improvements: 
<ul>
  <li>Increase the precision.</li>
  <li>Implementing other models (XGBoost / Random Forest).</li>
  <li>Implement SMOTE.</li>
  <li>Add other features.</li>
</ul>
