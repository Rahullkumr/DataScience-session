# DataScience with Python session

## Day1: 29/05/2023

What is required?

same type of data(homogeneous and contiguous data) is stored in python using "Numerical Python(NumPy)" package.
Array
series
Data frame

install Jupyter Notebook(Anaconda)

create new file
rename untitled to Day-1B
------

first program
print('Hello world')
run ==> shift + enter
the file is auto Saved

select mode and edit mode

in select mode, 

shift+enter ==> new input below current field

a ==> input field above the current input field

b ==> below

x ==> delete the selected input

### Array Operation ==> m (to make it heading)

Anaconda contains numpy by default
--------

int(python) ==> any length of data can be stored, no limit

num.shape ==>>> kitna dimension ka hai wo btata hai

num = np.array([56,12,34,87,19,52,63,27])

num.shape ===> (8,)

ascii(1 byte for each) is limited so they invented uni-code (2 byte for each symbol)

character in c ==> 1 byte

char in java ==> 2 byte

because java supports UNICODE but c supports ascii

google cloud input tools try (search in google)

list * 2 ==> list extends and appends the same list again

array * 2 ==> multiplies each element with two

list.range(10) ==> list create krega
np.arange(10) ==> array create krega

np.arange(1, 10, 0.25) ==> 1 to 10 incrementing 0.25

np.ones(13) ==> creates array of 1s, with 13 elements

num.argmax() ==> index of maximum element

np.linspace(1,10,11) ==> PATA KRO KYA HAI

scalar[1], vector[1,2,4], matrix[][], tensor[][]

matrix is a collection of vectors of equal length

vectorwa.flatten() ==> any dimensional array convert into 1D 

-------------------------------------------------
PANDAS STARTS HERE

dataFrame(2D) = collection of series(1D)

Series k contents mutable hote hn

Dataframe operations
df.ndim ==> n dimensions
df.shape==> (rows, columns)

df.T ==> Transpose(convert rows to columns & columns to rows)
help(object ka naam)
eg: help(df) ==> each function of dataframe will be shown

https://mathsisfun.com/

Data mining: converting data into meaningful information

Types of Data analytics
1. Descriptive analytics (what has happened) vvi
2. Predictive analytics (what will happen) vvi
3. Diafnostic analytics
4. Prescriptive analytics

median is more important than mean because it tells where the crowd is going
<img src="dynamic_hr.gif">

## Day2: 30/05/2023

mode = most frequent value in an array <br>
list from 1 to 90 will have same mean and median

Dispersion Types
-----------------
1. Absolute Deviation from Mean
2. Variance
3. a
4. a
5. a

Mean Absolute Deviation

variance
is a measure of how far indivdual(numeric) values in a dataset are from the mean or average value.
used to quantify spread or dispersion.

Three steps of building a Dataset
1. Collection
2. PreProcessing
3. Annotation

Data Set resources
1. https://data.gov.in/
2. https://archive.ics.uci.edu/ml/index.php
3. https://datasetsearch.research.google.com/

Structured dataset best file format ==> what and why?<br>
```diff
+ csv

+ It is a simple and universal format that can be easily read and written by many programs and tools, such as Python, R, SQL, and even text editors. 
+ CSV files are also lightweight and compact, which means they take up less space and can be transferred faster than Excel files.
+ CSV files are plain text, which means they are less prone to corruption and can be easily inspected and modified.
```

let's collect data : https://mitu.co.in/survey

df.iloc[2:9, 3:8]
display rows 2 to 8 and columns 3 to 7

df.iloc[:9, 3:8]
display rows 0 to 8 and columns 3 to 7

df.iloc[:9, 3:]
display rows 0 to 8 and columns 3 to last

df.iloc[2:9, 2]
display rows 2 to 8 and 2 columns only

df.iloc[5, :]
display 5 rows and all columns

df.iloc[5, :] vs df.loc[:, ['name', 'gender', 'sgpa']]

df.drop(4) ==> skips row 4
df.drop([3,5,7,8,9]) ==> 3,5,7,8,9 rows are skipped

df.drop('टाइमस्टँप', axis=1, inplace=True)
==> drops 'टाइमस्टँप' column and inplace changes the content

df['name'].str.title() ==> changes first letter to capital

df.isnull().sum() ==> gives how many rows have null values

df['age'] = df['age'].fillna(df['age'].median())
==> used to fill null values

x.to_csv('output.csv', index=False) ==> export to csv file in the current working directory
<img src="dynamic_hr.gif">
## Day3: 31/05/2023

### Visualization of Data
Descriptive analysis(only analysis)

import matplotlib.pyplot as plt
import numpy as np
........
plt.plot(x, y)

plt.xticks(range(0,81,10))
==> range of x axis starts from 0 to 100 with difference 10

aspect ratio of pc = 16:9

Types of plot
1. Scatter plot (only dots visible)
2. Bar (vertical line)
3. Barh (Horizontal bars)
4. Pie (Pie chart) = when share of a whole is required
5. Histogram
6. Boxplot

------------

Data Science life cycle
1. business understanding
2. data mining
3. data cleaning
4. Data exploration
5. Feature Engineering 
6. Predictive modeling
7. Data visualization

Artificial Intelligence:
through which machines can mimic human behaviour
computer can see ==> copmuter vision
computer can understand ==> NLP

who is the father of computer? what he created(mechanical computer) and when?
Alan Turing movie: The Imitation Game
father of modern computing(AI) = Alan Turing


compute vs calculate?
both are synonym
```diff
+ Compute: 
+ Calculate: 
```
statical modeling in old days and these days it's called Machine learning:
Explain ML.
```diff
ML is to identify pattern and use it
```
Halley's comet => seen at 76 years interval

Applications of ML
1. predict the outcomes of elections
2. identify and filter spam messages from email
3. foresee criminal activity
4. targeted advertising
5. auto pilot

Practical implementation of ML
x = 2, y = 1, z = ?
==> 2x + y

Types of ML
1. Supervised: require input and output (1 classification and 2 Regression)
2. Unsupervised: only require input(1 cluster and 2 anomaly ----)
3. Reinforcement Learning (advanced ML)


Quote: A breakthrough in ML would be worth ten microsofts(Bill Gates)

Linear Regression
<img src="dynamic_hr.gif">
## Day4: 1/06/2023

Multi variant Regression
Multiple linear Regression
co-relation

df.corrwith(df['mpg']) ==> co-relation against mpg i.e millage/gallon

classification starts here
eg - mail is spam or not

Types of classification
1. Binary classification
2. Multi class classification
3. Decission tree classification
4. Probability based classification

Decision tree (simplest algorithm)
eg - hollywood movie prediction whether it's going to be hit or not

when co-relation is not found then we can use decision tree

[scikit-learn.org ](https://scikit-learn.org/stable/)==> sir learnt from this website 

Probabilistic model
Probability ==> Theoritical(eg coin toss) and Practical(eg ipl match) probability

Real life implementation of BAYE'S THEOREM(used for conditional probability)

P(defective|mach2) = [p(mach2|defect) * p(defect)] / p(mach2)

Public Review: 
https://mitu.co.in/review

Private Feedback:
https://mitu.co.in/feedback

<img src="dynamic_hr.gif">
