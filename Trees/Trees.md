# Trees
### Searching...
BST's (Binary Search Trees) are one of the most intriguing data structures that code development has to offer. Often, within our scope of learning the basics of code, the scale of data that we experiment with is understandably small. But once we enter the realm of large-scale data, being aware of efficiency begins to pay large dividends. Binary Search Trees help us accomplish this with searchable data, primarily structured around the ability to compare values against their neighbors with _less than_ or _greater than_ logic. Specific to _Binary_ Search Trees, as the name would have it, is the structure where each node has at most two children.

A successful way of thinking about the layout and more specifically, the insertion logic of a binary search tree, would be a triangular plinko board. With values added to the plinko board, each value will end up taking a path contrived of right and left variations with a destination unique to itself as the tree fills up. In our digital version, as the value is place into the top, our program dictates where the value will end up based on repeated logic instead of leaving it up to the whims of gravity. 

>![Plinko Board](/Images/plinko.webp)
>*Homemade plinko board*

With common search tree structures in mind, a visual representation of a BST could look something like this:

>![Example BST with random integers](/Images/BST.jpg)
>*Example BST layout with random integers*


Each one of the numbers seen in this diagram represents a "_node_", or a data element that holds the value. The uppermost node (in this case, the number 8) is our "_root_". As a number is inserted into the tree, the value is compared to the node (our proverbial plinko peg, as it were) and then send down and to the left if it is less than the current node, or down and to the right if it is greater than the current node. 

Assuming that you were to insert the number 9 into the structure pictured above, where would it end up?

---

### Recursion 
Recursion is a key part of BST's, since unlike our previous example, we can be given values that need more steps to accomplish. The basic rule to note about this structure is the fact that navigating a BST is a repeated question of "_Left or Right?_" By using recursion appropriately, we can stop at a node, run a function to know whether to go left or right, and when/if we get to the next node, run that same function again, all within a singular action: Inserting, Searching, Deleting, etc.

---

