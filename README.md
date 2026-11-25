# Syed Saleh

**Software Development · Applied AI · Sports Analytics · Compiler Research**

I'm a Computational Modeling & Data Analytics student at Virginia Tech, graduating in May 2028. I build software and data workflows for practical problems—from AI-powered scheduling to baseball scouting—and conduct research on code similarity using LLVM.

I'm interested in internship opportunities in software engineering, data science, and applied AI.

[Portfolio](https://syedsaleh.dev) · [LinkedIn](https://linkedin.com/in/syed-saleh-264134276) · [Email](mailto:salehsyed1010@gmail.com) · [Resume](./syedsaleh_resume_S27.pdf)

---

## Virginia Tech Baseball

**Student Data Analyst · Sep. 2026–Present**

I work with TrackMan data to support player evaluation, opponent scouting, and transfer analysis.

- Collect practice TrackMan data and maintain SQL records for retrieval and analysis by a 15-person analytics team.
- Independently write R scripts for player evaluations and opponent scouting reports using metrics such as weighted on-base average (wOBA), pitch-type splits, and pitcher-handedness comparisons.
- Translate statistical findings into observations coaches can use for game preparation and player development.
- Evaluate potential transfers using other schools' TrackMan data, comparing player strengths and weaknesses with Virginia Tech's roster needs.

### Pitch-Tipping Detection — In Development

`Python` · `Computer Vision` · `Pose Estimation` · `TrackMan`

Developing a pipeline that connects pitching videos with TrackMan pitch-type labels and uses pretrained pose estimation to identify potential early pitch-tipping cues.

The planned workflow extracts body-position and delivery-timing measurements, accounts for body size and camera view, and produces annotated comparisons and reports for coaches. Evaluation will use separate recording sessions to test whether findings carry over to new footage.

**Processing target:** predict pitch type within three seconds per eligible clip, including preprocessing and inference. This is a development target, not a measured result or a claim of live, before-release prediction.

---

## Research

### LLVM Code Retrieval Under LLM Rewriting

`Python` · `C` · `LLVM IR` · `Clang` · `Linux` · `Project CodeNet`

Faculty-funded undergraduate research under **Prof. Kirshanthan Sundararajah** investigating whether compiler-derived features preserve enough implementation detail to connect an LLM-rewritten C program with its recorded original.

**Status:** Study design and protocol complete; pipeline built; experiments underway.

- Built a reproducible Python/Clang pipeline for selecting CodeNet programs, generating controlled LLM rewrites, compiling at `-O0` and `-O2`, running sample tests, and extracting LLVM IR features.
- Extract opcode bigrams within basic blocks and rank candidate originals using Jaccard similarity.
- Compare the primary representation with source-token trigrams, instruction distributions, and instruction counts.
- Evaluate retrieval using top-1 performance, mean reciprocal rank, and paired problem-level bootstrap comparisons.
- Retain generation records, compilation failures, and eligibility decisions to support reproducibility.

The study measures retrieval of known original–rewrite relationships and sensitivity to compiler optimization. It does not claim to prove authorship or detect plagiarism.

---

## Featured Projects

### AI Receptionist System

`Node.js` · `Azure AI Foundry` · `Azure OpenAI` · `Azure Cognitive Search` · `Azure Speech-to-Text` · `Azure SQL` · `Twilio` · `n8n` · `Google Calendar API`

Built with a five-person team during my internship at the South Asian Business Council of Virginia and piloted with **four local businesses**.

The system connects voice requests with business information and scheduling workflows, using retrieval-augmented generation to ground responses and backend integrations to check availability, book appointments, and process cancellations.

I owned Twilio voice/SMS integration and n8n calendar workflows, contributed to backend integration, and investigated slow availability lookups. Narrowing retrieval to the requested employee and time window reduced unnecessary processing.

**Pilot result:** 60 of the first 100 calls required no human escalation.

### Airedale Applied Intelligence Challenge — 2nd Place

`Engineering Analytics` · `Scenario Analysis` · `Investment Modeling` · `Technical Communication`

Our team, **init2winit**, earned second place in the Airedale Applied Intelligence Challenge at Virginia Tech in November 2026.

The team's analysis connected manufacturing, testing, service, and warranty records across **3,000 equipment units** and evaluated investment scenarios within a **$750,000 budget**.

I refined the presentation and recommendations and **presented independently at the live finals**, explaining the evidence, financial assumptions, and limitations behind the proposed investments.

The financial results were modeled projections, not realized savings.

[View Team Repository](https://github.com/syedsalehdev/airedale-init2winit)

### AI Stock Research Assistant

`Python` · `SEC EDGAR API` · `Pandas` · `BeautifulSoup` · `OpenAI Embeddings` · `NLP`

Built a pipeline to collect SEC filings and financial news, structure text for analysis, and explore sentiment using embeddings and language-model classification.

Developed experimental buy/sell/hold signals and backtested them against historical price data.

[View Repository](https://github.com/syedsalehdev/stockai) · [Watch Demo](https://youtu.be/2n7ENayA7ok)

### YouTube-to-MP3 Converter

`Python` · `FFmpeg` · `yt-dlp`

A Python tool that retrieves available audio streams using yt-dlp and converts them to MP3 through FFmpeg, with configurable bitrates and batch processing from a list of links.

[View Repository](https://github.com/syedsalehdev/youtube2mp3)

---

## Additional Experience

### AI & Data Science Intern — South Asian Business Council of Virginia
*Aug. 2025–Dec. 2025 · Ashburn, VA*

- Led a five-member team through architecture decisions, development, and a four-business pilot of the AI receptionist described above.
- Implemented voice and scheduling integrations using Twilio, n8n, and the Google Calendar API.
- Evaluated Twilio against self-hosted Asterisk, considering pilot volume, development effort, operating costs, and delivery timelines.
- Diagnosed availability-query delays and improved retrieval efficiency.

### Founder & Co-President — CodeAcademyX
*Sep. 2022–Jun. 2025 · Ashburn, VA*

- Co-founded a coding education program for underserved youth and taught **40+ students** through **20+ workshops** and mentoring sessions.
- Developed and taught a Python curriculum covering data structures, algorithms, and problem-solving patterns, including sliding windows, two pointers, and BFS/DFS.
- Supported **20+ students** in completing NeetCode 50.
- Measured performance using the same LeetCode-based assessment before and after instruction; average scores increased from **3/20 to 16/20**.
- Managed **eight volunteers** and tracked attendance and student performance using Google Sheets and Forms.

### Federal Technology & Contracts Intern — Applied Federal Technologies
*Sep. 2024–Jan. 2025 · Ashburn, VA*

- Built a Python/Pandas pipeline to screen **500+ federal opportunities** using SAM.gov and USAspending.gov data across cloud computing, cybersecurity, AI/ML, and IT modernization.
- Refined rule-based scoring to consider company capabilities, NAICS codes, and keyword relevance when prioritizing feasible opportunities.
- Maintained a SQL-backed tracker of **100+ qualified RFIs, RFPs, and Sources Sought notices**, recording deadlines, agency contacts, and review status.
- Reviewed procurement requirements across **40+ agencies** and mapped opportunities to company capabilities.

### Student Researcher — NASA HUNCH Program
*Aug. 2022–Mar. 2023*

- Designed and iterated on a lunar rover wheel prototype for lunar surface operations.
- Presented the final design to engineers at NASA Langley Research Center.

---

## Technical Skills

**Languages:** Python, Java, C/C++, JavaScript, SQL, R, C#, MATLAB

**Software & Integration:** Node.js, REST APIs, webhooks, Twilio, Google Calendar API, n8n

**Data & AI:** Pandas, data preprocessing, NLP, embeddings, retrieval-augmented generation, statistical analysis, API-based data collection

**Cloud:** Azure AI Foundry, Azure OpenAI, Azure Cognitive Search, Azure Speech-to-Text, Azure SQL Database

**Tools:** Git, Linux, LLVM, Clang, FFmpeg, yt-dlp

---

## Current Focus

- Building and evaluating computer-vision workflows for baseball analytics
- Studying how compiler optimization changes code-similarity signals
- Improving reproducibility and evaluation in applied AI projects
- Developing reliable backend integrations and data pipelines

---

## Education

**Virginia Tech**  
B.S. in Computational Modeling & Data Analytics  
**Expected graduation: May 2028** 

**Coursework:** Data Structures & Algorithms, Object-Oriented Programming, Low-Level Programming, Linear Algebra, Discrete Math, Multivariable Calculus, Probability & Statistics

Involved with Virginia Tech's AI & Machine Learning Club, CyberVT, and the hackathon community.

---

## Contact

[Email](mailto:salehsyed1010@gmail.com) · [Portfolio](https://syedsaleh.dev) · [LinkedIn](https://linkedin.com/in/syed-saleh-264134276) · [View Resume](./syedsaleh_resume_S27.pdf)
