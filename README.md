# Pyhton_Skills_BST
Checks if a given binary search tree contains a given value.
It is a simple code to show how to run code by itselft to search.     

# Question
Binary search tree (BST) is a binary tree where the value of each node is larger or equal to the values in all the nodes in that node's left subtree and is smaller than the values in all the nodes in that node's right subtree.    
Write a function that, efficiently with respect to time used, checks if a given binary search tree contains a given value. For example, for the following tree:     
    n1 (Value: 1, Left: null, Right: null)     
    n2 (Value: 2, Left: n1, Right: n3)     
    n3 (Value: 3, Left: null, Right: null)      
Call to contains(n2, 3), it should return True since a tree with root at n2 contains number 3.      

# The core code
```
    if root is None:
        return False
    elif root.value == value:
        return True
    elif root.value >= value:
        return contains(root.left, value)
    else:
        return contains(root.right, value)
 ```
