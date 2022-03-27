# Sets
### Unique Data Structure
Sets are a programming data structure that enables programmers to store varying datatypes within a single variable. Unique to sets, datatypes do not have to be similar, nor are the values within the collection ordered or index accessible. Sets 

### Common Operations
Python operations that deal with sets are as follows:

* Set Creation
    * Create an empty set
        * `empty_set = set()`
    * Create a set from a list
        * `myset = set((1, 2, 3, 4))` (notice the doubled brackets)


* Set Manipulation
    * Assume a set:
        * `myset = {1, 2, 3, 4}`
    * Add a value to the set:
        * `myset.add(5)`
        * `>>> myset = {1, 2, 3, 4, 5}`
    * Remove a value from the set:
        * `myset.remove(1)`
        * `>>> myset = {2, 3, 4, 5}`
    * Check if a specific value is in the set:
        * `if 3 in myset:`
        * `>>> True`
    * Find the number of items in the set:
        * `length = len(myset)`
        * `>>> 4`

* Multi-Set Manipulation

    Assume two sets: 

    `set1 = {10, 20, 30, 40, 50}` AND `set2 = {40, 50, 60, 70, 80}`    

    * Union
        * `set3 = intersection(set1, set2)`
        
        OR
        
        * `set3 = set1 & set2`
        * `>>> set3 = {40, 50}`
    * Intersection
        * `set4 = union(set1, set2)`

        OR 

        * `set4 = set1 | set2`
        * `>>> set4 = {10, 20, 30, 40, 50, 60, 70, 80}`


