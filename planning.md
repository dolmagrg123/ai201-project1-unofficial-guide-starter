# Project 1 Planning: The Unofficial Guide

> Write this document before you write any pipeline code.
> Your spec and architecture diagram are what you'll use to direct AI tools (Claude, Copilot, etc.) to generate your implementation — the more specific they are, the more useful the generated code will be.
> Update the Retrieval Approach and Chunking Strategy sections if you change your approach during implementation.
> Update this file before starting any stretch features.

---

## Domain

<!-- What domain did you choose? Why is this knowledge valuable and hard to find through official channels? -->

This project focuses on UC Berkeley off-campus housing experiences and advice gathered from student discussions, housing guides, and community resources. Students often rely on Reddit threads, housing forums, and unofficial recommendations to learn about apartment quality, landlord reputations, neighborhood safety, housing costs, and common rental scams.

This knowledge is difficult to find because it is scattered across many websites and discussion threads rather than being available in a single searchable source. The Unofficial Guide uses Retrieval-Augmented Generation (RAG) to consolidate this information and provide grounded, cited answers to students' housing-related questions.


---

## Documents

<!-- List your specific sources: URLs, subreddit names, forum threads, or file descriptions.
     Aim for at least 10 sources that together cover different subtopics or perspectives within your domain. -->

| #  | Source                                       | Description                                                                                  | URL or location                                                                                                                                      |
| -- | -------------------------------------------- | -------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1  | UC Berkeley Off-Campus Housing Office        | Official university guidance on finding off-campus housing and student resources             | [https://och.berkeley.edu/](https://och.berkeley.edu/)                                                                                               |
| 2  | UC Berkeley Housing Website                  | University housing overview and off-campus housing options                                   | [https://housing.berkeley.edu/explore-housing-options/off-campus-housing/](https://housing.berkeley.edu/explore-housing-options/off-campus-housing/) |
| 3  | Berkeley Basic Needs Center                  | Student support resources including housing insecurity and emergency housing help            | [https://basicneeds.berkeley.edu/housing-security](https://basicneeds.berkeley.edu/housing-security)                                                 |
| 4  | Berkeley Student Cooperative (BSC)           | Cooperative housing options, cost info, and student living experiences                       | [https://www.bsc.coop/](https://www.bsc.coop/)                                                                                                       |
| 5  | UC Berkeley ASUC Off-Campus Housing Guide    | Student-created housing guide and advice portal                                              | [https://www.ocf.berkeley.edu/~asucrh/offcampushousing/](https://www.ocf.berkeley.edu/~asucrh/offcampushousing/)                                     |
| 6  | Reddit r/berkeley – Housing Discussions      | Student experiences, landlord reviews, and housing advice threads                            | [https://www.reddit.com/r/berkeley/](https://www.reddit.com/r/berkeley/)                                                                             |
| 7  | Reddit Search: Off-Campus Housing            | Collection of multiple student threads on housing search and tips                            | [https://www.reddit.com/r/berkeley/search/?q=off+campus+housing](https://www.reddit.com/r/berkeley/search/?q=off+campus+housing)                     |
| 8  | Reddit Search: Apartment Advice              | Student discussions about apartments, rent, and neighborhoods                                | [https://www.reddit.com/r/berkeley/search/?q=apartment](https://www.reddit.com/r/berkeley/search/?q=apartment)                                       |
| 9  | RateMyDorms Berkeley Reviews                 | Student reviews of dorm and living experiences (useful for comparison to off-campus housing) | [https://www.ratemydorms.com/school/University-of-California-Berkeley](https://www.ratemydorms.com/school/University-of-California-Berkeley)         |
| 10 | North Berkeley Properties Housing Scam Guide | Real-world landlord and scam awareness guide for student renters                             | [https://www.northberkeleyproperties.com/avoiding-housing-scams/](https://www.northberkeleyproperties.com/avoiding-housing-scams/)                   |


---

## Chunking Strategy

<!-- How will you split documents into chunks?
     State your chunk size (in tokens or characters), overlap size, and explain why those
     numbers fit the structure of your documents.
     A review-heavy corpus warrants different chunking than a long FAQ. -->

**Chunk size:**

**Overlap:**

**Reasoning:**

---

## Retrieval Approach

<!-- Which embedding model are you using (e.g., all-MiniLM-L6-v2 via sentence-transformers)?
     How many chunks will you retrieve per query (top-k)?
     If you were deploying this for real users and cost wasn't a constraint, what tradeoffs
     would you weigh in choosing a different embedding model — context length, multilingual
     support, accuracy on domain-specific text, latency? -->

**Embedding model:**

**Top-k:**

**Production tradeoff reflection:**

---

## Evaluation Plan

<!-- List your 5 test questions with their expected correct answers.
     Questions should be specific enough that you can judge whether the system's response
     is right or wrong. "What are good dining halls?" is too vague.
     "What do students say about wait times at [dining hall name] during lunch?" is testable. -->

| # | Question | Expected answer |
|---|----------|-----------------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |

---

## Anticipated Challenges

<!-- What could go wrong? Name at least two specific risks with reasoning.
     Consider: noisy or inconsistent documents, missing source attribution, off-topic
     retrieval, chunks that split key information across boundaries. -->

1.

2.

---

## Architecture

<!-- Draw a diagram of your pipeline showing the five stages:
     Document Ingestion → Chunking → Embedding + Vector Store → Retrieval → Generation
     Label each stage with the tool or library you're using.
     You can use ASCII art, a Mermaid diagram, or embed a sketch as an image.
     You'll use this diagram as context when prompting AI tools to implement each stage. -->

---

## AI Tool Plan

<!-- For each part of the pipeline below, describe:
     - Which AI tool you plan to use (Claude, Copilot, ChatGPT, etc.)
     - What you'll give it as input (which sections of this planning.md, which requirements)
     - What you expect it to produce
     - How you'll verify the output matches your spec

     "I'll use AI to help me code" is not a plan.
     "I'll give Claude my Chunking Strategy section and ask it to implement chunk_text()
     with my specified chunk size and overlap" is a plan. -->

**Milestone 3 — Ingestion and chunking:**

**Milestone 4 — Embedding and retrieval:**

**Milestone 5 — Generation and interface:**
