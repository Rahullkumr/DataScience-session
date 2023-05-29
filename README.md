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

google cloud inut tools try (search in google)

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


