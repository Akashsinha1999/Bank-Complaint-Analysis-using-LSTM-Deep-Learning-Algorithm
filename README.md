
# Bank Complaint Analysis Using Deep Learning LSTM

This project aims to automate the analysis of a large dataset of more than 10 lakh text complaints submitted to a bank. Analyzing such a vast volume of complaints manually is impractical. To address this challenge, we employed a deep learning algorithm based on Long Short-Term Memory (LSTM) neural networks for sentiment analysis and classification.

## Screenshots

[Complaint analysis](https://drive.google.com/file/d/10egNGxW2IJiZPqAYjym_rsRfxQFxkDKO/view?usp=drive_link)


## Problem Statement

The primary goal of this project is to determine the department or category to which each complaint is relevant. The following departments were considered for categorization:

Credit reporting, credit repair services, or other personal 

consumer reports

Debt collection

Mortgage

Bank account or service

Credit card

Credit card or prepaid card

Student loan

Checking or savings account

Consumer Loan

Vehicle loan or lease

Money transfer, virtual currency, or money service

Payday loan, title loan, or personal loan

Payday loan

Money transfers

Prepaid card

Other financial service

Virtual currency

I convert these 18 department into 7 most import department 
to know that you can click the screenshot link https://drive.google.com/file/d/1cx5fkLrPO9UmfPgIWhy1lhQeocyCH4D8/view?usp=drive_link


## Techniques/Methods used
We utilized a deep learning model, specifically an LSTM (Long Short-Term Memory) neural network, to perform sentiment analysis on the text complaints.

Also i have used libraries like Numpy, pandas for data manipulation ,I imported Matplotlib, seaborn to visualize how many complaints registered for which department but i didnt used because methamtically i got the answer.

Imported warnings warnings.filterwarnings("ignore"), imported re (regex) , imported BeautifulSoupas , as i have used WordNetLametizer to perform lemmatization on text complaints.

I have also used train_test_split to split data into train and test set , then i have used Tokenizer which convert text into tokens (means assigning number according to the frequesncy of the number like word with highest frequency will be assigned as 1 ).

I have used pad_sequence as well ,as it stacks a list of tokens along a new dimension, and pads them to equal lenth 

Then i imported Dense , Input , LSTM , Embedding, Activation from keras.layers , i also imported Model, sequential from keras , then i imported initializers, regularizers, constraints, optimizers,layers from keras to execute the model and then i compiled the model  to predict the output.

This model can understand the sentiment expressed in each complaint and categorize it into one of the relevant departments.
## Data
This dataset consists of more than 10 lakh text complaints, which were collected from customers. The complaints are diverse and contain varying degrees of sentiment, making it challenging for manual analysis.

dataset link -  https://drive.google.com/file/d/1mVeJmR-hJVP2xlu8b4me2b3W9RQKL76K/view?usp=drive_link
## Result
The LSTM deep learning model successfully analyzed and categorized the complaints into the respective departments with 84% of accuracy. This automation has significantly reduced the manual workload and improved the efficiency of addressing customer complaints
## Usage 
To use this project, you can follow the instructions provided in the codebase to train the LSTM model on your own dataset of bank complaints. The trained model can then be used to automatically categorize complaints into their relevant departments.
## Conclusion
Automating the analysis of a vast number of bank complaints using the LSTM deep learning algorithm not only saves time and resources but also enhances the efficiency of the complaint handling process. This approach can be applied to similar text classification tasks in various domains, providing valuable insights and automation capabilities.





