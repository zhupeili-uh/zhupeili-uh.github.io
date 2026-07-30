---
layout: essay
type: essay
title: "Beyond the Code: The Architectural Blueprints of Club Hub"
# All dates must be YYYY-MM-DD format!
date: 2026-07-30
published: true
labels:
  - Software Engineering
  - Design Patterns
  - Next.js
  - Club Hub
---

<img class="img-fluid" src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Architectural blueprints and tools on a table">

*Photo by [Daniel McCullough](https://unsplash.com/@d_mccullough) on Unsplash*

## Reinventing the Wheel is Exhausting

Imagine you are tasked with building a physical clubhouse for the student organizations at the University of Hawaiʻi at Mānoa. You wouldn't start by inventing a new type of door hinge, nor would you spend weeks figuring out the physics of how a roof should drain water. You would use established architectural blueprints. You know a standard door works; you just need to adapt its size and color to your building. 

In software engineering, these universal blueprints are known as **design patterns**. They are not finished pieces of code that you can just copy and paste. Rather, they are proven, standardized, and reusable conceptual solutions to commonly occurring problems in software design. They give developers a shared vocabulary. When a senior engineer says, "Let's use an Observer here," everyone in the room instantly understands the architecture being proposed, saving hours of explanation.

## Laying the Foundation for Club Hub

When our team set out to build **Club Hub**—a centralized directory web application designed to connect students with campus clubs—we knew things could get messy quickly. Managing a full-stack application using Next.js, Bootstrap, and a PostgreSQL database requires strict organization. Without established blueprints, our codebase would have turned into a fragile house of cards. 

Instead of guessing our way through the architecture, we relied on a few key design patterns to keep the application scalable and maintainable.

## The Bouncer at the Door: The Singleton Pattern

One of the most immediate challenges we faced involved our database. In Next.js, the development environment utilizes "hot-reloading." Every time you save a file, the server restarts. If you simply create a new Prisma database client on every reload, you will quickly exhaust your PostgreSQL connection limit, crashing the application.

To solve this, we implemented the **Singleton Pattern**. The Singleton ensures that a class has only one instance and provides a global point of access to it. Think of it as a strict bouncer at the entrance of our Club Hub building. No matter how many people (or hot-reloads) try to enter, the bouncer ensures there is only one official guest log (database connection) being used.

Here is how we applied it in our code:

```typescript
import { PrismaClient } from '@prisma/client'

// Prevent multiple instances of Prisma Client in development
const globalForPrisma = globalThis as unknown as {
  prisma: PrismaClient | undefined
}

export const prisma = globalForPrisma.prisma ?? new PrismaClient()

if (process.env.NODE_ENV !== 'production') globalForPrisma.prisma = prisma
```

By storing the Prisma instance in the global scope, we guarantee that the rest of our application always interacts with a single, shared connection pool. 

## Building Blocks: The Composite Pattern 

Because we built Club Hub using React (via Next.js) and Bootstrap, we inherently embraced the **Composite Pattern**. This structural pattern allows you to compose objects into tree structures to represent part-whole hierarchies. It lets clients treat individual objects and compositions of objects uniformly.

In our UI design, a simple HTML button is an object. A `ClubCard` component that displays a club's logo, name, and description is a composition of smaller elements (images, text, buttons). A `ClubDirectoryGrid` is a composition of multiple `ClubCard` components. 

Because of the Composite pattern, rendering a single card or rendering a grid of fifty cards is handled with the exact same logic. We snap these React components together like LEGO bricks, allowing us to build complex, responsive user interfaces without duplicating code.

## The Takeaway

Writing code without design patterns is like trying to build a skyscraper without a blueprint. You might get the first few floors to stand up, but eventually, the structure will collapse under its own weight. By utilizing patterns like the Singleton and Composite, Club Hub wasn't just a project that worked—it was a project built on a solid, professional engineering foundation.

---

*Disclaimer: In accordance with the course academic guidelines for ICS 314, I would like to declare that I utilized an AI assistant (Gemini) to help brainstorm the "architectural blueprint" analogy, structure the narrative flow, and assist with grammar refinement for this essay. The core concepts, project details (Club Hub), and code examples reflect my actual coursework and understanding.*
