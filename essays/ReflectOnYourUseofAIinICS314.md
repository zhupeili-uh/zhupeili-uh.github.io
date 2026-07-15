---
layout: essay
type: essay
title: "Experience - My Use of AI Technical Essay"
# All dates must be YYYY-MM-DD format!
date: 2026-08-06
published: true
labels:
  - AI Use
  - Web Development
---


# Reflecting on My Use of AI in ICS 314: A Journey Through Modern Software Engineering Education

The integration of Generative Artificial Intelligence (AI) has initiated a paradigm shift in computer science education, particularly within the domain of Software Engineering. As modern development practices transition from manual syntax verification to high-level architectural oversight, the role of an educator and student must adapt. In the context of ICS 314 (Software Engineering) at the University of Hawaiʻi at Mānoa, this evolution is highly visible. This essay offers an in-depth, scholarly reflection on my personal experiences utilizing various AI models—specifically ChatGPT and GitHub Copilot—as cognitive partners throughout the Summer 2026 semester. By analyzing specific course elements, learning impacts, and the delicate balance between convenience and deep understanding, this reflection maps the challenges and opportunities of AI-enhanced learning.

## I. Introduction

Traditionally, introductory software engineering courses heavily emphasized syntax memorization, API navigation, and boilerplate structural generation. However, the emergence of Large Language Models (LLMs) has commoditized these lower-level tasks. In ICS 314, our learning curve revolved around mastering core development workflows, including responsive web design, functional programming paradigms, TypeScript type safety, and full-stack integration using Next.js. Throughout this journey, AI tools served as a dynamic, instantaneous resource.

The primary tools integrated into my daily workflow were OpenAI's ChatGPT (for conceptual explanations, script generation, and structured debugging) and GitHub Copilot (acting as an inline, predictive autocomplete engine within Visual Studio Code). While these models provided substantial acceleration in writing boilerplate code, their implementation also introduced distinct cognitive friction, requiring rigorous oversight to ensure academic integrity and true comprehension of the underlying architectural principles.

## II. Personal Experience with AI: Fourteen Key Course Elements

To evaluate the true utility of AI across the ICS 314 curriculum, this section dissects my interaction with these technologies across fourteen core course elements. Each analysis includes specific use cases, prompt examples, and an assessment of the associated costs and benefits.

| Course Element | AI Utilized? | Primary Tool | Overall Utility Rating |
| :--- | :---: | :--- | :--- |
| **1. Experience Quizzes (e.g., E18, E19, E20)** | Yes | ChatGPT | Moderate (Double-edged sword) |
| **2. Practice Quizzes** | Yes | ChatGPT | High (Excellent diagnostic tool) |
| **3. Formal Quizzes (e.g., Quiz 3, Quiz 8)** | No | None | N/A (Critical for self-evaluation) |
| **4. Portfolio Essays** | Yes | ChatGPT | High (Grammar & flow optimization) |
| **5. Final Project (Digits)** | Yes | Copilot & ChatGPT | Extremely High (State & route debugging) |
| **6. Learning Concepts / Tutorials** | Yes | ChatGPT | High (Customized analogies) |
| **7. Discord / Class Discussions** | No | None | N/A (Sought genuine connection) |
| **8. Asking/Answering "Smart-Questions"** | Yes | ChatGPT | High (Structure refinement) |
| **9. Coding Examples** | Yes | ChatGPT & Copilot | High (Instant syntax reference) |
| **10. Explaining Code** | Yes | ChatGPT | Extremely High (Deconstructing templates) |
| **11. Writing Code (e.g., Islandsnow)** | Yes | Copilot | High (Autocompleting Bootstrap classes) |
| **12. Documenting Code** | Yes | Copilot | High (Consistent JSDoc generation) |
| **13. Quality Assurance (e.g., ESLint errors)** | Yes | ChatGPT | Extremely High (Rapid linting resolution) |
| **14. Git/Workflow Optimization** | Yes | ChatGPT | Moderate (Git conflict recovery) |

---

### 1. Experience Quizzes (e.g., E18, E19, E20)
During the functional programming modules (E18, E19, and E20), where we had to manipulate data using Underscore.js, I turned to ChatGPT to conceptualize map/filter pipelines. 

> **Prompt:** > `"Write a TypeScript function using Underscore.js to filter an array of student objects with GPA > 3.5 and map them to return only their names."`

* **Benefits & Costs:** The primary benefit was the speed with which I could grasp the chaining syntax of Underscore. However, the cost was immediate: ChatGPT frequently hallucinated older ES5 syntax instead of modern, type-safe TypeScript. I spent significant time debugging type errors, teaching me that AI code cannot be blindly accepted without manual verification.

---

### 2. Practice Quizzes
Before engaging in timed, graded events, I utilized AI to generate variations of sample problems.

> **Prompt:** > `"Here is a sample practice quiz question on JavaScript scope. Can you generate three similar multiple-choice variations and explain the underlying scope rules for each?"`

* **Benefits & Costs:** This diagnostic use of AI was highly beneficial. It allowed me to identify gaps in my understanding of closures and scope without risking my grade. The cost was minimal, though it occasionally required re-prompting when the AI generated overly simplistic variants.

---

### 3. Graded Quizzes (e.g., Quiz 3, Quiz 8)
I made a conscious decision **never** to use AI during official, timed quizzes. 

* **Rationale:** Graded quizzes represent a baseline self-assessment. Resorting to AI under timed stress would bypass my own cognitive retrieval process, which is essential for long-term retention. While I might have completed the quizzes faster, I would have sacrificed genuine self-evaluation and risked violating academic standards.

---

### 4. Portfolio Essays
When writing technical reflections for my portfolio site (hosted via GitHub Pages at `zhupeili-uh.github.io`), I used ChatGPT as a structural editor.

> **Prompt:** > `"Review this technical reflection on TypeScript for clarity, tone, and grammar. Keep my personal voice but correct any passive phrasing."`

* **Benefits & Costs:** It greatly polished the prose, making my reflections sound concise and professional. The cost was the risk of "homogenization"—if left unedited, the AI-generated tone can sound generic. I had to actively rewrite sections to inject my actual coding perspective back into the text.

---

### 5. Final Project (Digits)
In developing the Next.js address book application, *Digits*, AI was crucial for managing routes and component communication.

> **Prompt:** > `"In Next.js, I have an edit form that needs to fetch data by ID from a local MongoDB schema using Meteor methods. Why is the state not updating when the route changes?"`

* **Benefits & Costs:** It acted as a highly competent senior developer, pinpointing asynchronous hook rendering issues in seconds. This saved hours of frustration. However, the cost was the complexity of integration: I had to thoroughly read, modify, and manually type the suggested code blocks to ensure I understood the architectural changes.

---

### 6. Learning Concepts and Tutorials
When faced with dense frameworks, I used AI to demystify complex documentation, like the transition from React state hooks to full Next.js context providers.

> **Prompt:** > `"Explain the React useContext hook using a simple analogy related to a central post office, rather than using complex coding jargon."`

* **Benefits & Costs:** Breaking down complex software abstractions into simple analogies accelerated my conceptual learning. The cost was that these analogies sometimes oversimplified edge cases, which required me to go back to the MDN Web Docs for accurate implementation details.

---

### 7. Answering Questions in Class or on Discord
I chose **not** to use AI to formulate answers or contributions in class or on Discord.

* **Rationale:** Collaborative community spaces thrive on organic, human-to-human interaction. Posting an AI-generated, perfectly curated answer on Discord detracts from the authentic shared learning environment of my peer group. Communicating my personal, raw problem-solving process proved much more valuable.

---

### 8. Asking or Answering a "Smart-Question"
When preparing questions to post in developer forums, I used AI to ensure I was following structured debugging guidelines.

> **Prompt:** > `"I want to ask a smart question about a TypeScript generic error. How should I format my current setup, expected behavior, and attempted fixes to be clear and polite?"`

* **Benefits & Costs:** It taught me the discipline of structured communication. By organizing my question properly, I was often able to solve the bug myself just by reviewing the formatted prompt.

---

### 9. Coding Examples
For quick syntax reference (such as Underscore's `_.pluck` or `_.groupBy`), AI served as an immediate, interactive cheat sheet.

> **Prompt:** > `"Show me a basic example of _.pluck extracting the 'id' field from an array of objects."`

* **Benefits & Costs:** Saved me from digging through poorly formatted legacy documentation. The cost was minimal, though it occasionally produced JavaScript code when I needed TypeScript, requiring manual type casting.

---

### 10. Explaining Code
When starting out with complex boilerplate configurations for Next.js or React, I used ChatGPT to break down the templates line-by-line.

> **Prompt:** > `"Analyze this Next.js middleware file and explain exactly what each import and rewrite rule is doing."`

* **Benefits & Costs:** This was incredibly helpful. Demystifying security rules and redirection protocols built solid mental models of our web infrastructure. There were very few costs associated with this practice, as it was strictly analytical.

---

### 11. Writing Code (e.g., Islandsnow, Maui Brewing)
During user interface mocks (like reproducing the layout of the *Islandsnow* homepage), I used GitHub Copilot to autocomplete repetitive HTML structures and Bootstrap components.

* **Benefits & Costs:** This streamlined my workflow immensely. It instantly generated responsive grids (`col-md-4`, `row`, etc.) and navigation dropdown configurations, allowing me to focus on styling. The downside was that Copilot often suggested outdated Bootstrap v4 structures instead of modern v5 classes, forcing me to review and fix the code manually.

---

### 12. Documenting Code
For code documentation, I relied on GitHub Copilot to generate structured JSDoc comments.

> **Prompt (via inline comment trigger):** > `/** Generates a list of names sorted alphabetically */`

* **Benefits & Costs:** It automated the repetitive task of writing comments, ensuring consistent JSDoc standards across my files. The cost was that it sometimes suggested comments that were far too wordy or generic, requiring me to simplify them for readability.

---

### 13. Quality Assurance (e.g., ESLint/TypeScript Errors)
Fixing ESLint rules and subtle TypeScript compilation warnings was one of my most common use cases for AI.

> **Prompt:** > `"How do I resolve the ESLint error: 'prop-types is missing in props validation' in my React component when I am already using TypeScript types?"`

* **Benefits & Costs:** This saved me countless hours of troubleshooting. AI quickly identified the conflict between standard ESLint rules and TypeScript typing setups, suggesting the exact compiler configurations to ignore redundant checks.

---

### 14. Git/Workflow Optimization
During branch merges or sudden merge conflicts when updating repositories, I used ChatGPT to safely resolve version control errors.

> **Prompt:** > `"I ran 'git pull origin main' on my local branch and got a merge conflict in package-lock.json. What are the safest steps to resolve this without breaking dependencies?"`

* **Benefits & Costs:** This prevented me from accidentally wiping out my local commits or corrupting my project configurations. The cost was that it required double-checking each command step-by-step to avoid running irreversible global resets.

---

## III. Impact on Learning and Understanding

Evaluating the overall impact of AI on my education reveals a complex dynamic. When used correctly, AI served as an excellent teaching assistant, offering customized feedback and analogies that made tough topics much more approachable. It essentially acted as an instant feedback loop, reducing the downtime spent stuck on simple typos or syntax errors and allowing me to dive straight into functional and full-stack system architecture.

However, the risk of "cognitive offloading" was a constant challenge. It is incredibly easy to rely too heavily on these tools, copy-pasting code block after code block without actually understanding how they work. To counter this, I developed a strict personal rule: **never commit any code suggested by AI that I couldn't explain or recreate myself from scratch.** By turning AI's output into a study guide rather than a final solution, I was able to build deeper problem-solving skills and truly internalize the concepts.

## IV. Practical Applications Outside ICS 314

Beyond the structured assignments of ICS 314, I applied these AI-assisted development practices to personal projects. For instance, in automated scripting tasks and exploratory API setups, I utilized ChatGPT to rapidly prototype data parsers. 

These real-world challenges highlighted the true strength of AI: rapidly generating boilerplates to bridge the gap between different environments. By automating repetitive backend configurations, I could spend my energy on high-level design choices, illustrating how AI can help engineers tackle complex software challenges in the real world.

## V. Challenges and Opportunities

The most prominent challenge of using AI in ICS 314 was dealing with **syntactic hallucination**. Because AI models are trained on historical data, they struggle to distinguish between deprecated framework features and modern standards. For example, when building our Next.js pages, AI frequently suggested older React patterns that contradicted our modern linting rules, resulting in confusing compilation errors.

Despite these issues, there are huge opportunities here for computer science education. Future courses could lean into AI as an active "pair programmer" rather than trying to ban it. Teaching students how to write effective prompts, analyze AI-generated code, and identify logical bugs could be incredibly valuable, helping prepare us for a modern industry where AI-assisted development is the standard.

## VI. Comparative Analysis: Traditional vs. AI-Enhanced Learning

Comparing traditional computer science education with an AI-enhanced approach reveals significant differences in student engagement, knowledge retention, and practical skill development.

| Dimension | Traditional Education Paradigm | AI-Enhanced Educational Paradigm |
| :--- | :--- | :--- |
| **Engagement** | Often leads to frustration due to syntax blockers, resulting in longer downtime. | Keeps momentum high by resolving minor syntax issues quickly, allowing focus on design. |
| **Knowledge Retention** | Reinforced through repetition and manual error correction, though it can be slow. | Shorter feedback loops can reduce retention if code is copied blindly without review. |
| **Skill Development** | Focuses heavily on syntax fluency, typing accuracy, and manual debugging. | Prioritizes high-level system design, prompt design, and code auditing. |

While traditional methods are great for teaching syntax and manual debugging, they can slow down progress. AI-assisted learning, on the other hand, lets students jump straight into complex architectures and design choices. However, to keep knowledge retention high, we must complement this speed with structured, independent assessments like quizzes to ensure the core concepts stick.

## VII. Future Considerations

Looking ahead, the role of AI in software engineering is only going to grow. We will likely see highly specialized models integrated directly into IDEs, handling everything from basic testing to deployment pipeline optimizations.

Because of this, software engineering courses should shift their focus from syntax fluency to **architectural evaluation, prompt design, and system integration**. Success won't just be about writing code; it will be about our ability to manage, direct, and audit AI systems to build secure, robust software.

## VIII. Conclusion

My experience using AI in ICS 314 has been transformative. It has shown me that tools like ChatGPT and GitHub Copilot are incredibly powerful multipliers for development speed and productivity. However, they are not a substitute for core computer engineering principles. Without a solid understanding of clean code, type safety, and system architecture, AI-generated code can easily fall apart.

To make the most of AI in future courses, I recommend integrating prompt design, code auditing, and security reviews directly into the syllabus. By treating AI as a collaborative partner rather than an easy shortcut, we can prepare the next generation of engineers to lead and innovate in an AI-driven industry.
