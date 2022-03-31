# Sets
### Unique Data Structure

Sets are a programming data structure that enables programmers to store varying datatypes within a single variable. Unique to sets, datatypes do not have to be similar, nor are the values within the collection ordered or index accessible. Right now that probably sounds bad, but as you learn more about sets and what they are, this will not be such a bad thing. 

---

### Big 0 Efficiency

Because of the nature of sets, duplicate values are eliminated from the data set, which makes adding, removing, and finding values from a set almost always an O(1) efficiency. This is possible because when a value is assessed by the built-in Python logic, a *hash value* is assigned to that piece of data. You can think of this as a serial number on a reproducible product. Yes, the items are the same kind of thing, but they are not the *exact* same thing. Consequently, when we search for a specific value within a set, this distinguishing identity of our desired value helps us find the item we are looking for very efficiently. 


>![Fleet of Cars](/Images/Car%20Fleet.jpeg)
>*A fleet of mixed up cars*


As a practical example, let's say you work for a rental car company. The cars are not parked in any particular order, but as the cars are moved around, the VIN numbers of each car is dutifully recorded and placed in a database with the assigned parking space. Without this aspect of the business, if a customer wanted a specific car, your only option would be to go out and look for the car that visually matches the discription of the desired vehicle. How many black sedans can you see? Probably enough to make you question if there's a better way.
Luckily, when a specific car is needed, you are provided the VIN number and in return are given the exact parking spot for the car you need. There is only one car that could possibly match your requirements, and you can quickly find out if that car is available or not. 

---

### Common Operations
Python operations that deal with sets are as follows:

* __Set Creation__
    * Create an empty set
        > `empty_set = set()`
           
        (**NOTE**: *Creating an empty set via empty "{}" brackets will result in Python assuming you are initializing an empty dictionary.*)
    * Create a set from a list
        > `myset = set((1, 2, 3, 4))` 
        
        (notice the doubled brackets)
---

* __Singular Set Manipulation__
    * Assume a set:
        > `myset = {1, 2, 3, 4}`
    * Add a value to the set:
        > `myset.add(5)`
        >
        > `>>> myset = {1, 2, 3, 4, 5}`
    * Use update to add values with other datatypes to your set:
        > `myset.update([3, 4, 5, 6])`
        >
        > `>>> myset = {1, 2, 3, 4, 5, 6}`     
    * Remove an existing value from the set:
        > `myset.remove(1)`
        >
        > `>>> myset = {2, 3, 4, 5, 6}`
    * Remove a value that does not exist without a Traceback Error:
        > `myset.discard(91)`
        >
        > `>>> myset = {2, 3, 4, 5, 6}`
    * Check if a specific value is in the set:
        > `if 3 in myset:`
        >
        > `>>> True`
    * Find the number of items in the set:
        > `length = len(myset)`
        >
        > `>>> 5`
---
* __Multi-Set Manipulation__

    Assume two sets: 

    >`set1 = {10, 20, 30, 40, 50}` 
    >
    >AND 
    >
    >`set2 = {40, 50, 60, 70, 80}`    

    * Union
        > `set3 = intersection(set1, set2)`
        >
        >OR
        >
        > `set3 = set1 & set2`
        >
        > `>>> set3 = {40, 50}`
    * Intersection
        > `set4 = union(set1, set2)`
        >
        >OR 
        >
        > `set4 = set1 | set2`
        >
        > `>>> set4 = {10, 20, 30, 40, 50, 60, 70, 80}`

For additional insights into set methods, visit [this page](https://www.programiz.com/python-programming/set#:~:text=other%20python%20set%20methods) for a complete list. 

For the sets coding exercise, click [here.](/Sets/setsexercise.md)

