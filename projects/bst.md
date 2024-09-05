---
layout: project
type: project
image: img/bst/tree.png
title: "Binary Search Tree Visualization"
date: 2023
published: true
labels:
  - Java
summary: "A visualization of binary search trees, and its preorder, inorder, and postorder."
---

<div class="text-center p-4">
  <img width="200px" src="../img/bst/BST.png" class="img-thumbnail" >
</div>

Created to help ICS students understand binary search trees. Users are able to specify how many nodes are in the tree, and the program will draw the BST. The program also provides the preorder, inorder, and postorder of the tree.

This is the first GUI project I'd ever created, and it is full of inefficient code, as I was still very much a beginner. It was a big project for me, especially figuring out how to manipulate the graphics.

Here is some example code that illustrates how I developed the graphics.

```java
for (int j = 0; j < tokens.length; j++) {
  tempX = x;
  tempY = y;

  if (tokens[j].equals("left") || tokens[j].equals("left!")) {
    // manipulate x and y values
    // get width of node (visual)
		      		
    if (((x - textWidth) + 28) >= 320) {
      // manipulate x value
    }

    if (tokens[j].contains("!")) {	   	
      // draw oval
      // draw line connecting
    }
  }
```
