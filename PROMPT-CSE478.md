# Prompt for CSE 478 Study Tool Updates

Copy-paste this into a new Claude chat, along with the `cse478-data.js` file:

---

I have an interactive study tool hosted on GitHub Pages. I need to add new content for **CSE 478 — Foundations of Data Visualization** (Dr. Atkinson, ASU).

**Attached file: `cse478-data.js`** — this contains all my current flashcards, T/F questions, and scenario practice questions for this course.

**Exam format**: 8 items, each with 3 questions. Most present a short scenario or code example and ask you to analyze it using course concepts. Answers should clearly explain reasoning and connect to class ideas.

**What I need you to do:**
1. Read the attached lecture slides (PPTX files) I'm uploading
2. Generate new flashcards, T/F questions, AND scenario practice questions from the lecture content
3. Add them as a new week/module to the existing data in `cse478-data.js`
4. Give me back the updated `cse478-data.js` file

**Data format reference:**

```javascript
// Flashcard:
{ q: "Question text", a: "Answer text" }

// True/False:
{ s: "Statement to evaluate", ans: true, e: "Explanation shown after answering" }

// Scenario (exam-style):
{ scenario: "A real-world situation description...", question: "What does the student need to analyze?", answer: "Model answer connecting to course concepts...", concepts: ["concept1", "concept2"] }
```

**Important:**
- Scenarios should mirror the exam format: real-world situations analyzed with course concepts
- The variable name must stay `window.CSE478_DATA`
- Add new content as a new module inside the existing `modules` array
- Keep all existing content intact

Here are the new lecture slides: [attach PPTX files]
