---
layout: post
title: "Simple English Test Maker"
date: 2024-11-30
---

## Simple English Test Maker

Welcome to the **Simple English Test Maker**! This tool allows you to create fun and simple English tests to practice vocabulary and grammar.

### How It Works:

1. **Choose a Test Type**:
   - **Multiple Choice Questions**
   - **Fill-in-the-Blank**
   - **True or False**

2. **Add Your Words and Definitions**:
   Enter the words you want to test on, and we’ll automatically generate questions for you!

### Example:

#### Word List:
1. **Apple**  
   Definition: A round fruit with red, yellow, or green skin and a sweet taste.

2. **Run**  
   Definition: To move quickly using your legs.

3. **Happy**  
   Definition: Feeling good or pleased.

#### Generated Test:

**Multiple Choice Question**:  
What does "Apple" mean?  
- A) A round fruit with red, yellow, or green skin and a sweet taste.  
- B) A type of vegetable.  
- C) A vehicle for transportation.

**Fill-in-the-Blank**:  
The sun is very bright and makes me feel _______.  
(Answer: Happy)

**True or False**:  
"Run" means to walk slowly.  
(Answer: False)

### Start Creating Your Own Test!

Use the form below to input words and definitions, and our system will generate a test for you.

---

#### Optional Feature: Link a Code Form (Optional for GitHub Pages)

If you'd like to make this interactive and allow users to input their own words and generate tests dynamically:
1. Use a JavaScript-based test generator (hosted locally).
2. Add a form to collect inputs:

```html
<form id="test-maker">
  <label for="word">Enter Word:</label>
  <input type="text" id="word" name="word" required>
  
  <label for="definition">Enter Definition:</label>
  <input type="text" id="definition" name="definition" required>
  
  <button type="submit">Generate Test</button>
</form>

<div id="generated-test"></div>

<script>
  document.getElementById("test-maker").addEventListener("submit", function(event) {
    event.preventDefault();
    const word = document.getElementById("word").value;
    const definition = document.getElementById("definition").value;
    
    document.getElementById("generated-test").innerHTML = `
      <h3>Your Test:</h3>
      <p><b>Word:</b> ${word}</p>
      <p><b>Definition:</b> ${definition}</p>
      <p><b>Question:</b> What does "${word}" mean?</p>
      <ul>
        <li>${definition}</li>
        <li>Another option</li>
        <li>Yet another option</li>
      </ul>
    `;
  });
</script>
