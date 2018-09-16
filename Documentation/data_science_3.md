**Now that we have everything set up, let's start writing some Python code to access our dataset!**

In the first cell, type the following code:
```python
import csv
import pandas as pd
```

To actually run this code, simply click the *play* button on the left of the cell. Alternatively you can make sure you have the correct cell selected, and hit *shift+enter* on the keyboard.

## How it works
We will need to use a few *libraries* to help up access and understand the dataset we are using. Libraries are used in almost every programming project, and they contain more specialised code to help us do what we need to do! In this case, we are using:
  * `CSV` to read our CSV file
  * `pandas` is a `Python Data Analysis Library`. (The library’s name derives from **pan**el **da**ta, a common term for multidimensional data sets encountered in statistics and econometrics).

---

Now let's load our CSV file into Pandas. In a new cell write the following code:

```python
pets = pd.read_csv('surfcoastshireregisteredanimals.csv', sep=',',header=0)
```

## How it works
we are using Pandas to read a csv file, with the name of the CSV file we uploaded. We are then giving Pandas some extra information so it knows how the file is formatted: `sep=',', header=0`.

To check that it is all working, underneath the line we just added, simply type `pets`:
```python
pets = pd.read_csv('surfcoastshireregisteredanimals.csv', sep=',',header=0)
pets
```

This will print the data loaded in pets. You should see the Pandas table with the information from the CSV! If you come across an error, don't worry! Make sure you have run all of the previous cells in sequence by clicking the *play* button. Make sure you do see the data before proceeding to the next step.