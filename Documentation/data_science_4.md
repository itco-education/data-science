**Now that we have access to our dataset in Python, let's explore!**

We now have 6842 rows of pet data loaded, that's a lot! It's definitely too much to go through yourself! So let's explore some of the techniques we can use to understand this data.

Before we dive into the code iteself, let's understand how to use the tools at our disposal. We now have a DataTable loaded which represents the data. The name of our table is *pets*. Just like any other tables, we have a few columns which we can use to query information. We can use the `.columns` attribute to find out the names of the columns:

```python
pets.columns
```

This shows us:

* 'Suburb'
* 'Breed'
* 'Animal_Type_Name'
* 'Colour'
* 'Animal_Name'
* 'Registered'

So if we want to list only the breeds, we can use:

```python
pets.Breed
```

![Pets Breed](https://raw.githubusercontent.com/itco-education/data-science/master/Documentation/Images/petsbreed.png)

That's cool, but it shows us every single row, still too much data... let's get summarising! How about counting the number of rows each breed?

```python
pets.Breed.value_counts()
```

![Pets Breed](https://raw.githubusercontent.com/itco-education/data-science/master/Documentation/Images/petsbreedcount.png)

`value_counts()` will *count* the number of *values* in each row! By default, it is sorted by the count, so the most common value will be shown first.

### Your Task!

Can you tell us the most popular name of pet?