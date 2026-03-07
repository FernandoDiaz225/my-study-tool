# Prompt for CSE 463 Study Tool Updates

Copy-paste this into a new Claude chat, along with the `cse463-data.js` file:

---

I have an interactive study tool hosted on GitHub Pages. I need to add new content for **CSE 463 — Introduction to Human Computer Interaction** (Dr. Atkinson, ASU).

**Attached file: `cse463-data.js`** — this contains all my current flashcards, T/F questions, and scenario practice questions for this course.

**Exam format**: 8 items total. Each presents a design scenario and asks you to analyze, diagnose, or suggest improvements using HCI frameworks and concepts from class. Strong answers clearly connect the scenario to relevant course concepts.

**What I need you to do:**
1. Read the attached lecture slides (PPTX files) I'm uploading
2. Generate new flashcards, T/F questions, AND scenario practice questions from the lecture content
3. Add them as a new week/module to the existing data in `cse463-data.js`
4. Give me back the updated `cse463-data.js` file

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
- Scenarios should mirror the exam format: real-world design situations where you diagnose HCI problems
- The variable name must stay `window.CSE463_DATA`
- Add new content as a new module inside the existing `modules` array
- Keep all existing content intact

Here are the new lecture slides: [attach PPTX files]
