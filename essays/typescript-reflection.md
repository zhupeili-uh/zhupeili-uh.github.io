---
layout: essay
type: essay
title: E10: "Taming the JavaScript Wild West: First Impressions of TypeScript"
# All dates must be YYYY-MM-DD format!
date: 2026-06-06
published: true
labels:
  - Software Engineering
  - TypeScript
  - Web Development
---

Starting out in modern web development, my first encounters with plain JavaScript felt a lot like walking on a tightrope without a safety net. Coming from a mindset that appreciates structured, hardware-level logic and the strict rules of compiled languages like C++, JavaScript's "anything goes" philosophy was genuinely unsettling. You can pass a string into a mathematical function, and instead of throwing a massive error and stopping the build, JavaScript just shrugs and hands you a `NaN` at runtime. 

Being introduced to TypeScript over the past two weeks of this semester, it felt less like learning a new language and more like putting up guardrails on a dangerous mountain road. To be completely honest, my initial impression is a massive sigh of relief.

<img class="img-fluid" src="https://upload.wikimedia.org/wikipedia/commons/4/4c/Typescript_logo_2020.svg" alt="TypeScript Logo" style="max-width: 200px; margin: 20px auto; display: block;">

## Catching Bugs Before They Hatch

The biggest early revelation for me has been static typing. In standard JavaScript, you often don't realize you've made a terrible mistake until you run the program, click a button, and watch the console turn red with the dreaded `undefined is not a function`. 

TypeScript shifts this paradigm entirely. By forcing you to declare what type of data a variable should hold, the code editor itself becomes your first line of defense. It acts like a strict compiler that catches your typos and logic flaws right as you are typing them. 

Take a look at this simple example:

```typescript
// JavaScript lets this pass, but fails at runtime.
// TypeScript stops you right here with an error.
function calculateArea(radius: number) {
  return Math.PI * radius * radius;
}

// Editor Error: Argument of type 'string' is not assignable to parameter of type 'number'.
let myArea = calculateArea("five"); 
```

As an engineering student, this immediate feedback loop is incredibly satisfying. Even in these early assignments, it is already saving me time by catching simple human errors before they become obscure bugs.

## The Power of Interfaces: A Contract for Data

Another feature that has quickly clicked with me is the concept of `Interfaces`. When dealing with complex data structures, keeping track of exactly what properties an object is supposed to have can be a nightmare. Interfaces solve this by establishing a strict contract.

If I define an interface for a user profile, TypeScript guarantees that any object claiming to be a user profile will have exactly those required properties—no more, no less. It bridges the gap between the rigid, predictable architecture I prefer and the flexible nature of web browsers.

## A Worthwhile Trade-off for the Road Ahead

I will admit that TypeScript requires more upfront work. Writing out types, defining interfaces, and satisfying the compiler's demands takes extra keystrokes and slows down the initial drafting process. 

However, even though we are only a couple of weeks into the course, I can already see that this minor upfront tax is going to be entirely worth it. As we move on to building more complex projects later in the semester, I anticipate that the time lost writing types will be paid back tenfold when I *don't* have to spend hours debugging a missing property. TypeScript doesn't just make the code better; it sets a solid foundation. And in software engineering, starting with confidence in your code's stability is everything.

---
*AI Usage Disclosure: The core ideas, structural perspective, and engineering viewpoints in this essay are entirely my own. I used an AI assistant (Gemini) strictly to help translate my thoughts into fluid English, format the Markdown structure (including headings and code blocks), and ensure grammatical accuracy to meet the professional standards of this portfolio assignment.*
