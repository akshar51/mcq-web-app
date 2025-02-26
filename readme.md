# JavaScript MCQ Web Test - Documentation

## Overview
This is a simple multiple-choice question (MCQ) web test built using **HTML, CSS, and JavaScript**. It features a quiz interface with navigation controls, a countdown timer, and a scoring system.

## Features
- **Dynamic Question Loading**: Questions and options are displayed dynamically.
- **User Interaction**: Users can select answers and navigate through questions.
- **Timer Functionality**: A 60-second timer resets per question.
- **Scoring System**: Users receive a final score at the end.
- **Responsive UI**: Styled using CSS for an engaging experience.

## File Structure
```
/ (root directory)
│-- index.html  (Main HTML file with quiz layout)
│-- styles.css  (Contains styling for the UI - optional if separate)
│-- script.js   (Contains quiz logic - optional if separate)
```

## Code Explanation

### 1. **HTML Structure** (`index.html`)
- **Container**: Holds the quiz content.
- **Question Display**: Shows the current question.
- **Options List**: Renders multiple-choice answers dynamically.
- **Buttons**: Controls for navigation (`Next`, `Previous`, `Submit`).
- **Timer**: Displays countdown per question.
- **Result Display**: Shows final score after submission.

### 2. **CSS Styling** (Inline in HTML or separate `styles.css`)
- Defines the layout, colors, and interactive styles for the quiz.
- `.container`: Centralized quiz box.
- `.question`: Styles question text.
- `.options li`: Styles each option with hover effects.
- `.btn`: Button styling for better UX.

### 3. **JavaScript Logic** (`script.js` in `<script>` tag of HTML)

#### **Variables and Data Structure**
- `questions`: Array of objects containing the MCQ data.
- `currentQuestionIndex`: Tracks the active question.
- `userAnswers`: Stores user-selected answers.
- `timeLeft` & `timerInterval`: Handles the countdown timer.

#### **Functions**

- `startTimer()`: Initializes and updates a 60s timer per question.
- `loadQuestion()`: Displays the current question and options.
- `selectOption(option)`: Stores user selection and enables `Next` button.
- `nextQuestion()`: Moves to the next question or submits the quiz.
- `prevQuestion()`: Returns to the previous question.
- `submitQuiz()`: Calculates and displays the final score.

## How to Use
1. Open `index.html` in a browser.
2. Answer the displayed question.
3. Use `Next` and `Previous` to navigate.
4. Click `Submit` on the last question to see your score.

## Live Demo
Check out the live version of the MCQ Web Test here: [MCQ Web App](https://mcq-web-app-phi.vercel.app/)

## Possible Enhancements
- **Persistent Timer**: Use a global countdown instead of per-question reset.
- **Local Storage**: Store progress to allow resumption on refresh.
- **Shuffled Questions**: Randomize question order for variation.
- **Highlight Selected Option**: Improve UX with visual selection feedback.

## Conclusion
This JavaScript MCQ test is a simple and effective quiz system that can be extended for educational or training purposes. 🚀

