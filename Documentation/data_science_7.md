**We've gone through a number of interesting techniques so far, let's try and tie it all together with a number of challenges! Keep in mind that you are *not* expected to know or remember all the different commands at your disposal, rather, look at what we've covered in earlier tasks and ask us for hints and help!

1. What is the most common pet colour?
2. Which suburb has the most pets?
3. Draw an appropriate graph which represents the number of registered/unregistered pets.
4. Which suburb has the most Golden Retrievers?
5. How many unique pet names in BARRABOOL are there? there?
6. What other interesting information can you find out? If you don't know how to find it out, ask one of the presenters and we can try together!

---

The following is a list of helpful commands which can be used:

* `.value_counts()` lists the count of the different values. (can only be used in a single column dataframe).
* `.count()` counts the number of rows returned
* `pets[pets.Animal_Name == "BELLA"]` lists all the rows where the animal's name is "BELLA"
* `.groupby(<FIELD>)` groups rows by one of the fields provided. The result must be described using `desribe()`, for example: `pets.groupby('Suburb').describe()`.
* `.plot(kind='pie')` plots the returned rows as a pie chart.
* `.nunique()` returns the number of unique rows.