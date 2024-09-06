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

A simple implementation of Rock Paper Scissors created with Java Swing. This was created as an example of a GUI in Java that I could quickly refer to when students would seek tutoring with me for this specific assignment.

Here is some code that illustrates how I display the user's choice, the computer's choice, as well as increment the game stats.

```java
public void userChose(String option) {
  userPick.setText(option);
  getCompChoice();
}

public void getCompChoice() {
  Random rand = new Random();
  int compChoice = rand.nextInt(3);

  compPick.setText(choices[compChoice]);
  incrementStats(compPick.getText());
}

public void incrementStats(String comp) {
  this.count++;

  userStats.setText("Games Played: " + this.count);
  String result = determineWinner(userPick.getText(), comp);

  if (result.equals(TIE)) {
    this.ties++;
  } else if (result.equals(USER)) {
    this.wins++;
  } else {
    this.losses++;
  }

  userTies.setText("Ties: " + ties);
  userWins.setText("Wins: " + wins);
  userLosses.setText("Losses: " + losses);
}
```
