# Stacks
### Last In, First Out
Last in First out is the principle of Stacks, not dissimilar from the idea of a "stack" of any physically and vertically stackable objects (ex: books, pancakes, etc). Consequently, the first item to picked up from the pile/stack would have been the last one added. Stacks are inherently useful to developers who need an easy way to work with history-based data. 

---

### Big O Efficiency
Due to their nature of primarily using only the "top" element of the data structure, the Big O notation for insertion and deletion are O(1) (aka, the best). Access and searching within the rest of the pile is average efficiency (O(n)) since you are reverting back to an unordered list approach. 

---

### Common Operations

Considering the format of the stack structure, the built-in Python list operations "Push" and "Pop" are used to add and remove data from the list, respectively. 

| Common Stack Operations | Description | Python Code | Performance |
| ---- | ---- | ---- | --- |
| push(_value_) | Adds "value" to the back of the stack. | `my_stack.append(value)` | O(1) - Performance of adding to the end of a dynamic array
| pop() | Removes and returns the item from the back of the stack | `value = my_stack.pop()` | O(1) - Performance of removing from the end of a dynamic array
| size() | Return the size of the stack. | `length = len(my_stack)` | O(1) - Performance of returning the size of the dynamic array
| empty() | Returns true if the length of the stack is zero. | `if len(my_stack) == 0:` | O(1) - Performance of checking the size of the dynamic array

## For Example:

>![Control Z](/Images/download.jpeg)
>
>*A common keyboard usage is Control + Z*

Assume you are working on a paper for school and you type it up yourself. When something inevitably goes wrong with your typing, you instinctively hit the CTRL + Z combo you've seemingly known forever and you go on with your project. This functionality is a stack. 

Now lets say that for every new thing you do to the document is associated with a number. Opening a file, adding a new page, inserting a picture, or just general typing all qualify. As you go along, that stack might look something like this:

```python
stack = []

stack.append(1) # New action
stack.append(2) # New action
stack.append(3) # New action
stack.append(4) # New action
stack.append(5) # New action


print(stack)
```
`>>> [1, 2, 3, 4, 5]`

Then at action 5 you realize you have misspelled your word in your document. Now what? 

_CTRL + Z_

```python
stack.pop() # CTRL + Z
stack.pop() # CTRL + Z
stack.pop() # CTRL + Z

print(stack)
```

`>>> [1, 2]`

---

For the stacks coding exercise, click [here](/Stacks/stackexercise.md)
