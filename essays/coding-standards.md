---
layout: essay
type: essay
title: "Coding Standards: Necessary or Not?"
# All dates must be YYYY-MM-DD format!
date: 2024-09-26
published: true
labels:
  - Software Engineering
  - Coding Standards
  - Education
---

<img width="200px" class="rounded float-start pe-4" src="../img/essays/standard.png">


My first introduction to the computer science world and programming was an Intro to Java course at Leeward Community College. On the first day of instruction, the professor provided a document of coding standards for the class—things that were, at the time, foreign and intimidating for me. Things like camelCase, consistent indentation, where it’s okay to place spaces and where it isn’t, as well as the placement of curly braces. For many, learning coding standards can be tedious, and some may even choose to ignore them entirely to do their own thing. After all, the code still works even when these standards aren’t followed, right? When working in Java, I could place curly braces wherever I want, on the same line or on a new line. I could name my variables using lowercase, PascalCase, or other naming conventions. I could place spaces between the function name and the arguments. I could separate each line of code using as many blank lines as I want, creating an endless abyss of whitespace. If it doesn’t affect functionality, why, some may ask, is there a need to follow coding standards at all?

## The Importance of Consistency
When working with a team, you may realize the way you approach problems and resolve them is different from your teammates. This can make it difficult to fully understand what’s happening in their code compared to yours, as you may have not thought of the solution they did. To make matters even worse, imagine you and your teammates all have vastly different personal coding standards, making their code completely unreadable to you. This would pose a significant challenge to whoever is tasked with reviewing or maintaining the team’s final, combined code. To prevent these issues, one solution could be to establish a guideline for the team that everyone can follow to improve the readability and consistency of the codebase. In other words, establishing a coding standard.

Returning to my experience in the Intro to Java course, I followed my professor’s coding standards to a tee. In doing so, I created a consistent structure throughout my programs, and whenever I turned to Google for help with a problem, the way the solutions were presented on the tutorial and forum sites were already familiar to me. Moreover, when I moved onto Python, I was already used to indentation and limiting whitespace, so the stricter syntax was not a problem for me and I was able to familiarize myself with the programming language much faster than if I had to learn the coding standards for the first time.

## Enforcing Coding Standards
Some IDEs (integrated development environment) and downloadable tools enforce coding standards, regardless of their necessity for the functionality of the program. In my ICS 314 class, I was introduced to ESLint; a tool that helps to identify and fix JavaScript and TypeScript code. When you deviate from the coding standard, ESLint alerts you to the problems and gives you suggestions on how to fix it. At first, ESLint alerted me to a few errors I didn’t even realize I was making—such as unnecessary trailing whitespace or a missing new line at the bottom of the file. Though it was initially frustrating to be nitpicked and corrected so thoroughly, I realize the necessity of these standards. Not only does it help me write cleaner, more professional code, but it also makes the debugging process much easier. By maintaining this consistency, I am able to focus more on my code rather than minor formatting issues.

## Conclusion
Coding standards may seem trivial at first, and some may still find them unimportant even after encountering the issues I mentioned above. However, they serve as the foundation for writing readable, consistent, and maintainable code—something that will be invaluable when collaborating with others and in large-scale projects. In an industry driven by teamwork and adaptability, coding standards are not just beneficial but essential for long-term success.
