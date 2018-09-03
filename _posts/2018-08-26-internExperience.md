---
title: 2018 Summer Intern Experience
date: 2018-08-26 21:04:09
categories:
- technical
---

This was my experience interning at Amazon as a SDE (software development engineer) intern in the summer of 2018.
For non-disclosure reasons, I can't really explain to the fullest granularity what I worked on this summer, but in general terms: I created API calls for a domain object  used in an internal system.

### Things I have learned:
Through the internship, I got very hands on with AWS services like DynamoDB and Cloudformation. Prior to the internship, I did have a brief 3 weeks introduction to relational databases, so I was vaguely familiar with their design. However, the API calls I were working on relied on DynamoDB, a non-relational database system. I had to get familiar with non-relational table design (Hash Key, Sort Key, Global Secondary Indexes ) as well as querying and batch querying techniques. Another thing was how to design APIs. Writing code to error handle and deliver the correct results was done through multiple layers. I had to utilize software design principles such as facade, data access object, and dependency injection that I've only read about in the software engineering course I took last semester.
After developing the calls, I had to make sure to write unit and integration tests through Groovy, a Google framework for Java tests. Through that, I discovered how to test layer by layer through mocking, as well as the importance of line and branch coverage.

Summary: I got very familiar with AWS services and other internal tools, as well as software design structures.

### Things I have enjoyed:
After getting close to the full-time employees on my team, I realized that they were on a different level than me in terms of code quality. The code I pushed out in the beginning of the internship pales in comparison to the effortlessly modular code that they wrote. My mentor recommended me read "Clean Code: A Handbook of Agile Software Craftsmanship", by Robert C. Martin, or so he called it "The Bible of Coding". Over the course of the internship, I felt like taking notes from both this book, and my mentor, my code increased in terms of readability and refactorability.

Another aspect of the internship I enjoyed was meeting old high school friends. Given the ~1500 interns at Amazon in Seattle this summer, and a high school that primarily focused on the STEM subjects, it wasn't a surprise that I would bump into some people from my old high school.
It was very thought-provoking talking to them, not only reminiscing about old times, but also about future plans that seem unreachable right now (prestigious graduate schools, research under renowned professors, and so on).
It was refreshing talking to friends I had lost contact to as well as make new friends, and to realize that I was pretty unaccomplished compared to a lot of them; I realized that I was unsatisfied with being average, so that sort of shook me awake.

Summary: Learning from full-time engineers and the knowledge they had, and meeting old friends who were also interns.

### Overall:
I feel like I grew a lot as a software engineer during this summer. Working for one of the largest tech companies opened my eyes to what the industry is like, and what I can do from now until graduation to prepare myself for it. Hmm, I wonder what I'll be doing next summer?

- Andrew

