# Insurance Forecasting
Multiple Linear Regression Model

### Action

1. Dataset
2. Aim
3. Approach
4. Expolratory Data Analysis
5. Feature Engineering
6. Modelling
 * Independent and Dependent variables
 * Test Train Split
 * Multiple Linear Regression Model
7. Evaluation
8. Conclusion

### About Dataset

Link: https://www.kaggle.com/datasets/mirichoi0218/insurance

The dataset has been taken from _kaggle_ from the source link mentioned above. The _csv_ file contains the details in the following columns.

**Columns:**

1. _age:_ age of primary beneficiary
1. _sex:_ insurance contractor gender, female, male
1. _bmi:_ Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight ($kg/m^2$) using the ratio of height to weight, ideally 18.5 to 24.9
1. _children:_ Number of children covered by health insurance / Number of dependents
1. _smoker:_ Smoking
1. _region:_ the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.
1. _charges:_ Individual medical costs billed by health insurance

### Aim:

To accurately predict insurance costs.

### Insight:

If we observe the columns, it is clear that age, sex, bmi, children, smoker and region columns form the features of our dataset and charges column is our target variable.

The key observations that can be made from the dataset above:
* We have 4 numerical and 3 categorical variables.
* We have $1338$ rows of data.
* Another important thing to be noticed here is that there are no null values in our dataset (Hence, no cleaning is required).

We then move to feature engineering and subsequently modelling of out dataset.

We have 3 categorical variables, namely, **sex**, **smoker** and **region**. The first two have binary values and hence label enconding can be used for them. For **region**, we will be using one-hot encoding. From here on I will be using a new copy of dataset, thereby retaining the original one.

We split our data into test and train and deploy our **Multiple Linear Regression model**.

### Result

The accuracy of our model comes out to be about 77%.
