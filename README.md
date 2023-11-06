# EX-7-Implementation-of-BTree-Indexing

## DATE : 14/09/23

## AIM :

To implement B-tree indexing and to search an element in the B-tree using python.

## ALGORITHM :

<div align="justify">
1. Starting from the root node, compare k with the first key of the node.<br>
2. If k = the first key of the node, return the node and the index.<br>
3. If k.leaf = true, return NULL (i.e. not found).<br>
If k < the first key of the root node, search the left child of this key recursively.<br>
4. If there is more than one key in the current node and k > the first key, compare k with the next key in the node.
If k < next key, search the left child of this key (ie. k lies in between the first and the second keys).
Else, search the right child of the key.<br>
5. Repeat steps 1 to 4 until the leaf is reached.<br>
</div>
  
## PROGRAM :

```python
Searching a key on a B-tree in Python
Create a node

  ```python
# Searching a key on a B-tree in Python
# Create a node
class BTreeNode:
  def __init__(self, leaf=False):
    self.leaf = leaf
@@ -119,4 +120,9 @@ def main():
if __name__ == '__main__':
  main()
```
## OUTPUT :

![image](https://github.com/dineshgl/EX-7-Implementation-of-BTree-Indexing/assets/143793356/a0988958-d08d-4bf3-a518-f46af62ca388)

## RESULT :

Thus the python program for the implementation of B-Tree Indexing has been executed successfully.
