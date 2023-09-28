# SmartSense Assessment-1

The repository consists of a Python Notebook that contains the entire code for the solution.

The comments have been made in the Notebook explaining the data pre-processing and the subsequent steps to train the model. For the purpose of this problem statement, I have used Logistic Regression for identifying the cuisine type and ratings.
## Organisation of the Repository

- The zipfile containing the data is provided in the ['data/](./data) folder. You can use the following simple command to extract the data and unzip it:
```
!wget https://github.com/JINAY08/smartsense_sol/blob/main/EPI_batch.zip
!unzip -q EPI_batch.zip -d "content/"
```

- The source code is under the ['src/'](./src) directory. You could find the Google colab notebook there and could easily run it from the Github interface!
- The requirements for running the code are in the ['requirements.txt'](requirements.txt) file. You could easily install them by running the following command:
```
pip install -r requirements.txt
```

## Logistic Regression

Logistic Regression is used for a dataset of independent variables. Logistic regression is also called logits model, the main idea behind which is to output the probabilities for the independent variables.

## Data Preprocessing

Data pre-processing is a very important step before starting to train any ML model. For the purpose of data pre-processing in this problem statement, I first downloaded the given dataset, and visualised the data using pandas and Dataframes. Next, I observed that there were some columns of the dataframe that was of minimal use for the purpose of this problem statement. In the initial parts of the code I tried removing these columns and just using the important columns after merging the dataframes.
Given below is one of the plots showing the frequency of each of the occurring Cuisine type:

![Screenshot 2023-09-28 135822](https://github.com/JINAY08/smartsense_sol/blob/main/images/Screenshot%202023-09-28%20135822.png)

As could be observed the data is quite biased towards one or two cuisines.
## Approach and Results

So after performing the pre-processing, I identified the important columns (ratings and type of cuisine) and trained a Logistic Regression model on the data. I used the in-built sklearn's Logistic Regression model. Firstly, I split the data into training and test sets (75/25 ratio); learned the model on the training set, and used cross-validation accuracy as the metric to judge the performance of the model.

The mean cross-validation accuracy came out to be nearly 63 %. The drop in the accuracy could be attributed to the initial bias present in the dataset with one or two classes dominating the others!

As it turns out, the model is fairly accurate while predicting the type of cuisine based on the ingredients and average ratings received by the cuisine!

