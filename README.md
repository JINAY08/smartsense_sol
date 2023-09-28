# smartsense_sol

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
![Count of each cuisine type](https://github.com/JINAY08/smartsense_sol/blob/main/images/Screenshot%202023-09-28%20135822.png)

## Approach


