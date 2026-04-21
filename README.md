# BST File System

## Scenario
In a computer system, files need to be stored and accessed efficiently. Instead of searching through all files every time, the system organizes file sizes (or IDs) using a Binary Search Tree (BST). 

In this structure:
- Smaller values are stored in the left subtree
- Larger values are stored in the right subtree

This arrangement helps in maintaining the data in a sorted manner and improves performance.

---

## Justification
Binary Search Tree is used because it provides:
- Faster insertion compared to linear structures like arrays
- Efficient searching of elements
- Automatic sorting of data using traversal techniques

Thus, BST reduces time complexity and improves overall system efficiency.

---

## Algorithm

### Insertion Algorithm
1. Start from the root node
2. If the tree is empty, create a new node as root
3. If the value is less than the current node, move to the left child
4. If the value is greater than the current node, move to the right child
5. Repeat until the correct position is found and insert the node

### Inorder Traversal Algorithm
1. Traverse the left subtree
2. Visit the root node
3. Traverse the right subtree

This traversal prints the elements in sorted order.

---

## Time Complexity
- Insertion:
  - Best/Average Case: O(log n)
  - Worst Case: O(n) (when tree becomes skewed)
  
- Traversal:
  - O(n), as all nodes are visited once

---

## Output
After inserting the file sizes into the Binary Search Tree and performing inorder traversal, the output will display all file sizes in sorted order.

For the given input:
Input: 50, 30, 70, 20, 40, 60, 80  

Output:
20 30 40 50 60 70 80
