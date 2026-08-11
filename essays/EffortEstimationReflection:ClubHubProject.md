---
layout: essay
type: essay
title: "Effort Estimation Reflection: Club Hub Project"
date: 2026-08-10
published: true
labels:
  - Estimation log
---


Reflecting on the development of the Club Hub project across its three milestones, I found the process of effort estimation to be a highly insightful exercise. Overall, I found estimating to be relatively manageable, though it certainly required careful forethought. 

Having about a year of prior software development experience gave me a solid baseline to draw from. I found that breaking the project down into granular issues made estimating much easier. For example, rather than estimating "backend development" as a monolithic block, estimating the time for form submissions separately from NextAuth.js role-based access control allowed for much tighter and more realistic predictions. To track my time, I relied on a strict timer, which removed any guesswork. Interestingly, my estimated times ended up matching my actual coding effort almost perfectly—such as estimating and executing the M3 Playwright acceptance tests in exactly 180 minutes. The hardest part of the process, however, was accounting for the psychological pressure; knowing there was a running timer and an estimated target occasionally made the debugging phases feel more urgent and stressful.

Despite the challenges, this estimation process was incredibly helpful. First, it forced me to mentally architect the solution before writing a single line of code. When assigning 120 minutes to populate the PostgreSQL database with real University of Hawaii organization data, I had to preemptively think about data structures and seeding scripts, which ultimately streamlined the actual implementation. Secondly, keeping a centralized estimation log was vital for our team dynamics. It provided clear visibility into the workload distribution across all team members, ensuring that no single person was overwhelmed during any specific milestone. It kept our overall project velocity predictable and transparent.

While I am proud of the accuracy of my estimates, there is definitely room for improvement, particularly in how I categorize my time. Reviewing my logs, I noticed a significant blind spot: I recorded zero minutes of "Non-Coding Effort" for almost all of my assigned tasks. In reality, software engineering involves substantial non-coding work. Tasks assigned to me, such as creating UI/UX mockups in M1, planning database schemas, or configuring continuous integration pipelines via GitHub Actions, heavily involve system design, reading documentation, and planning logic. Because I relied purely on a running timer from start to finish, I inadvertently rolled all this research and planning time directly into my "Coding Effort." 

To do this better in the future, I plan to strictly separate my tracking into two distinct phases: system design/research (non-coding) and active implementation (coding). By pausing the coding timer while I am reading documentation or sketching out UI layouts, I will gain a much more accurate picture of how much time I spend problem-solving versus how much time I spend actively typing syntax. This refinement will make my future project planning even more precise and professional.
