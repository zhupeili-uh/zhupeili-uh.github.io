---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "ConnectU"
date: 2026
published: true
labels:
  - Data Structure / Algorithm
  - Backend Development
  - C++
  - Github
summary: "My team developed a robotic mouse that won first place in the 2015 UH Micromouse competition."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

ConnectU is a semester-long software development project for the ECE 367L Data Structures and Algorithms lab, where I acted as a Backend Engineer for a simulated social media startup. The primary objective was to build a fully functional text-based social network capable of handling users, posts, friendships, and algorithmic feeds. The application was developed using C++, with continuous version control managed through GitHub and terminal environments.

To ensure the application could scale efficiently, I manually implemented several core data structures to solve specific backend challenges. I engineered a custom Hash Map with chaining to optimize user lookups to $O(1)$ time complexity, and built a Max Heap (Priority Queue) to power an algorithmic feed that dynamically sorted "viral" posts based on likes and recency. Additionally, the project utilized Linked Lists for dynamic chronological timelines, Binary Search Trees (BST) for alphabetical sorting, and Breadth-First Search (BFS) graph traversal to generate friend recommendations.

Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
