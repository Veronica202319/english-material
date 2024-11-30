---
layout: post
title: "Simple English Test Maker"
date: 2024-11-30
---

# Simple English Test Maker

Welcome to the **Simple English Test Maker**! This section helps you create easy and fun English tests to improve vocabulary and grammar skills. Just have fun

---

### How It Works:

1. **Pick a Test Type**:
   - **Multiple Choice Questions**
   - **Fill-in-the-Blank**
   - **True or False**

2. **Add Your Words and Definitions**:
   Enter your custom words and their meanings, and we’ll create questions for you automatically.

---

### Example Test:

#### Word List:
- **Dog**: A domestic animal known as man’s best friend.
- **Run**: To move quickly on foot.
- **Bright**: Giving off lots of light.

#### Generated Questions:

**Multiple Choice Question**:  
What does "Bright" mean?  
- A) To be clever.  
- B) Giving off lots of light.  
- C) Running fast.

**Fill-in-the-Blank**:  
A ________ is a loyal pet to humans.  
(Answer: Dog)

**True or False**:  
"Run" means to sit quietly.  
(Answer: False)

---

### Create Your Own Test:

<div id="quiz-container">
  <h2>Interactive Quiz</h2>

  <!-- Multiple Choice Question -->
  <div>
    <p><strong>What does "Bright" mean?</strong></p>
    <form id="mcq">
      <input type="radio" name="bright" value="A" id="mcq1"><label for="mcq1">A) To be clever.</label><br>
      <input type="radio" name="bright" value="B" id="mcq2"><label for="mcq2">B) Giving off lots of light.</label><br>
      <input type="radio" name="bright" value="C" id="mcq3"><label for="mcq3">C) Running fast.</label>
    </form>
  </div>

  <!-- Fill-in-the-Blank Question -->
  <div>
    <p><strong>Fill in the Blank:</strong> A ______ is a loyal pet to humans.</p>
    <input type="text" id="fitb" placeholder="Your Answer">
  </div>

  <!-- True or False -->
  <div>
    <p><strong>True or False:</strong> "Run" means to sit quietly.</p>
    <form id="true-false">
      <input type="radio" name="run" value="true" id="true"><label for="true">True</label><br>
      <input type="radio" name="run" value="false" id="false"><label for="false">False</label>
    </form>
  </div>

  <button onclick="submitQuiz()">Submit Answers</button>

  <!-- Result Display -->
  <div id="results" style="margin-top: 20px; font-weight: bold;"></div>
</div>

<script>
  function submitQuiz() {
    let score = 0;

    // Multiple Choice Question Scoring
    const mcqAnswer = document.querySelector('input[name="bright"]:checked');
    if (mcqAnswer && mcqAnswer.value === "B") {
      score++;
    }

    // Fill-in-the-Blank Scoring
    const fitbAnswer = document.getElementById("fitb").value.trim().toLowerCase();
    if (fitbAnswer === "dog") {
      score++;
    }

    // True or False Scoring
    const tfAnswer = document.querySelector('input[name="run"]:checked');
    if (tfAnswer && tfAnswer.value === "false") {
      score++;
    }

    // Display Results
    const results = document.getElementById("results");
    results.textContent = `Your score: ${score}/3`;

    // Feedback for incorrect answers
    if (score < 3) {
      results.textContent += " - Keep practicing!";
    } else {
      results.textContent += " - Excellent!";
    }
  }
</script>

