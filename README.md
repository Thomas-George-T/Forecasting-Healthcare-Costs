# Linear Regression on Personal Health Data

## Motivation
Hi all, This is my first notebook. I am trying to perform Exploratory Data Analysis (EDA) and linear regression on personal health data set end to end. Any feedback and constuctive feedback is appreciated hosted on Kaggle. Link to the Dataset: https://www.kaggle.com/mirichoi0218/insurance

# Steps

## 1. Import Data

Once we import the Data using `read_csv`, we then use `head()` to sample the data . We try to identify numerical and categorical data.

![sample-data](assets/sample-data.JPG)

## 2. Preprocessing

We proceed to collect basic descriptive stats using `describe()`. 

```python
data.describe()
```

We then split the data into numerical and categorical data.

![preprocessing](assets/preprocessing.JPG)

We proceed to convert categorical data into numerical data. We use One hot encoding technique for this.

One hot encoding is a technique where we replace the categorical data with binary digits. The categorical column is split into same number of columns as the values. The respective column is then given a '1' or a '0' corresponding to the values.

we use one hot encoding by using `get_dummies()`

![one hot encoding](assets/one-hot-encoding.JPG)

## 3. Exploratory Data Processing (EDA)

We try to then find the correlation between features.

![eda](assets/eda.JPG)

Using a heat map to explore the trends.

![heatmap](assets/corr-heatmap.JPG)
