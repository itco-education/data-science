**Let's get visualising!**

So far we have been extracting and learning information from the dataset, but some data is best understood visually. When visualising data, it is important to use appropriate charts for appropriate datasets.

### Dog person, or a cat person?

Let's try understand the percentage breakdown of the type of pet in the dataset!

To do this, we will need the count of the type of animal. If you can recal, we did something similar earlier!

```python
pets.Animal_Type_Name.value_counts()
```

This will count the animal types in the dataset! But instead of just printing the numbers, let's chart it! To do this is pretty simple, first let's store the count into a new variable, and the plot it!:

```python
animal_type_count = pets.Animal_Type_Name.value_counts()
animal_type_count.plot(kind='pie')
```

![Pet Type](https://raw.githubusercontent.com/itco-education/data-science/master/Documentation/Images/pet_type.png)

### Your task!

Try and plot a bar chart, of the most common pet breeds!

*HINT*: We can *limit* the number of results by using `.head(10)`, this would only keep the top 10 values. For example: `pets.head(10)` will only list the first 10 pet rows.