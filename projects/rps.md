---
layout: project
type: project
image: img/rps/rps_title_page.png
title: "Rock Paper Scissors"
date: 2023
published: true
labels:
  - Java
  - Game
summary: "Rock Paper Scissors game developed in Java, from the ICS 211 curriculum."
---

<div class="text-center p-4">
  <img width="200px" src="../img/rps/rps.png" class="img-thumbnail" >
</div>

A simple game of Rock Paper Scissors vs. your computer. This was my attempt at the ICS 211 GUI RPS project. This was mainly done to be an example I could refer to when students would seek tutoring with me for this specific assignment. 

Here is some code that illustrates how I generated the computer's response.

```java
public void getCompChoice() {
  // array of possible choices
  String[] choices = {"ROCK", "PAPER", "SCISSORS"};

  // generate a random number between 0-2
  Random rand = new Random();
  int compChoice = rand.nextInt(3);

  // set text to computer's choice
  compPick.setText(choices[compChoice]);

  // increment and update game values
  incrementStats(compPick.getText());
}
```
