---
layout: project
type: project
image: img/bst/tree.png
title: "Binary Search Tree Visualization"
date: 2023
published: true
labels:
  - Java
  - Swing
  - AWT
  - Trees
summary: "A visualization of binary search trees, and its preorder, inorder, and postorder."
---

<div class="text-center p-4">
  <img width="500px" src="../img/bst/bst.png" class="img-thumbnail" >
</div>

My first personal project in Java outside of classwork. While the BST section is complete, the Max Heap and AVL Tree sections are largely a work in progress. The entire program may be reworked entirely eventually as I was very much a beginner when I created this.

Created with Java Swing and AWT to guide ICS students through learning and understanding binary search trees and the traversals. Swing and AWT were utilized for the graphics. The program also features a working login system, where users are able to create accounts and sign in to see their saved binary search trees for future reference.

How the program works:
Once the user logs in or makes an account, they are able to choose between a Binary Search Tree, Max Heap, or AVL Tree. The user can specify how many nodes are in the tree, enter the numbers, and watch as the program automatically creates the tree for them. The program also provides the preorder, inorder, and postorder traversals.

Here is some example code that illustrates how I implemented the binary search tree.

```java
public void bsTree() {
	if (circle != null) {
		box.remove(circle);
	}

	bstree = new BSTree();
	circle = new Circle(treeNum.length, treeNum, bstree.getSides());
		
	for (int num : treeNum) {
		bstree.addNode(num);
	}
		
	box.setVisible(true);
	box.add(circle);

	circle.repaint();
	preOrder.setEnabled(true);
	inOrder.setEnabled(true);
	postOrder.setEnabled(true);
}
```
