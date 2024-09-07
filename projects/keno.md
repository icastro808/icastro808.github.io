---
layout: project
type: project
image: img/keno_title_page.png
title: "Keno"
date: 2023
published: true
labels:
  - Java
  - Swing
  - Game
  - Class Project
summary: "A Java implementation of the casino game Keno that I developed for my ICS 211 class."
---

<div class="text-center p-4">
  <img width="500px" src="../img/Keno.png" class="img-thumbnail" >
</div>

Keno is a lottery-style gambling game. In most versions of Keno, you are able to choose 20 numbers out of 80. The winning numbers are drawn randomly, and the payout depends on how many of your selected numbers were drawn.

My version of Keno has shortened this to choose 10 numbers out of 40 for the sake of simplicity (and size of the window).

This program was created using Java Swing and AWT. I utilized JPanels to separate the frame into sections: the payout/hit table, game board, and stats table. JOptionPanes were used to provide the user with information regarding how to play the game, and worked alongside JButtons to provide a functioning GUI with real time changes. Arrays were used to keep track of which buttons the user chose, as well as the randomly generated numbers for the drawing.

Here is some code that illustrates how I handled the functionality of the game buttons.

```java
for (JButton button : BUTTON_ARR) {
  if (button.isSelected() && e.getSource() == button) {
    if (count == MAX) {
      PLAY_BUTTON.setEnabled(false);
    }

  button.setSelected(false);
  setColor(button, colorArr[0]);

  count--;
  updateStats();
  SELECTED_BUTTONS.remove(button);
  }
  else if (!button.isSelected() && e.getSource() == button) {
    if (count == MAX) {
      JOptionPane.showMessageDialog(new JFrame(), "\nYou may only have 10 selected buttons." +
                                "\n\nClick on a highlighted button to deselect before choosing another.");
      break;
    }
...
...
...
```
