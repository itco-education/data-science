**Getting a bit more advanced**

Time to step it up a bit, and perform some more advanced queries!

In the previous step, we discovered the most common pet name is Bella! Cute! Let's now find out where all those Bellas are coming from!

What we want to do here is find each row where the animals name is Bella. We can do this in the following way:

```python
pets[pets.Animal_Name == "BELLA"]
```

Let's break this down a bit. We are performing a *query* here, asking for the pets data *where* the pet's name is Bella. This will filter all the rows where the pets name is Bella, and show them to us!

We can assign that to a new DataTable, called `bellas`!

```python
bellas = pets[pets.Animal_Name == "BELLA"]
```

This is pretty powerful, because now we can perfom the same queries before, on an already filtered table! So, we're still trying to find out where the Bellas are... How about we count the suburbs of the Bellas?

```python
bellas.Suburb.value_counts()
```

This shows us that 46 Bellas live in homes from Torquay! That's a lot of Bellas!

### Final Code:

```python
bellas = pets[pets.Animal_Name == "BELLA"]
bellas.Suburb.value_counts()
```

### Your task

Do you have a pet? Why don't you find how many pets in the dataset share your furry one's name! (You can just make one up if you don't have a pet!).