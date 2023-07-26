# Trees

## Introduction:
In our exploration of trees, we've encountered Binary Trees, Binary Search Trees, and K-ary Trees. Now, let's embark on a new adventure and learn about different ways to traverse these trees efficiently. Traversals allow us to visit each node in the tree exactly once, uncovering the hidden treasures they hold. We'll delve into two common traversal techniques: Depth-First and Breadth-First Traversals.

---

## Common Terminology
1. Node - A Tree node is a component which may contain its own values, and references to other nodes
2. Root - The root is the node at the beginning of the tree
3. K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
4. Left - A reference to one child node, in a binary tree
5. Right - A reference to the other child node, in a binary tree
6. Edge - The edge in a tree is the link between a parent and child node
7. Leaf - A leaf is a node that does not have any children
8. Height - The height of a tree is the number of edges from the root to the furthest leaf

---

I. Depth-First Traversal:
Imagine you are exploring a maze, and your goal is to reach the end while taking the deepest path possible at each junction. That's precisely what Depth-First Traversal is all about!

1. Preorder Traversal:
In Preorder traversal, we start at the root and follow the order: Root - Left Child - Right Child.

    Example (Binary Search Tree):

```shell 
   5
  / \
 2   7
/ \   \
1  3   8


Inorder: 1 - 2 - 3 - 5 - 7 - 8
```

2. Inorder Traversal:
In Inorder traversal, we start at the leftmost node, traverse the left subtree, visit the root, and then traverse the right subtree.

    Example (Binary Search Tree):

```shell
   5
  / \
 2   7
/ \   \
1  3   8

Inorder: 1 - 2 - 3 - 5 - 7 - 8
```

3. Postorder Traversal:
In Postorder traversal, we start at the leftmost node, traverse the left subtree, then the right subtree, and finally visit the root.

    Example (Binary Tree):

```shell
   1
  / \
 2   3
/ \   \
4  5   6

Postorder: 4 - 5 - 2 - 6 - 3 - 1
```

II. Breadth-First Traversal (Level Order):
Imagine you are exploring the tree level by level, like reading pages of a book from left to right.

Breadth-First Traversal follows this approach, visiting all nodes at the same level before moving to the next level.

Example (Binary Tree):

```shell
   1
  / \
 2   3
/ \   \
4  5   6

Breadth-First: 1 - 2 - 3 - 4 - 5 - 6
```
---

## Quiz:

1. What is the order of traversal in Preorder Traversal for a Binary Tree?
2. Which traversal is commonly used to print the contents of a Binary Search Tree in ascending order?
3. How does Breadth-First Traversal explore the tree?

## Review of a Classmate's Learning:

Classmate's Topic: Big O of Searching a BST
Review: Your explanation of the Big O of searching a Binary Search Tree was clear and concise. It's essential to understand that in the average case, the time complexity for searching a BST is O(log n), where n is the number of nodes in the tree. However, in the worst case (unbalanced tree), the search time can be O(n), where the tree resembles a linked list. Keep up the good work in your learning journey!

