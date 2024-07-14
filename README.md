
# Exam Project

This project is a simple exam paoject that allows users to sign up, log in, and take a timed multiple-choice quiz. The application is built using HTML, CSS, and JavaScript. It includes features such as a timer, question navigation, and result display.

## Features

- User Registration and Login
- Multiple-choice questions with navigation
- Timed exam (2 minutes)
- Result display with correct and incorrect answers
- Responsive design

## Table of Contents

- [Getting Started](#getting-started)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Functionality](#functionality)
- [Credits](#credits)

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

You need a web browser to run this project. No additional software or libraries are required.

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/afathelbab/examproject.git
   ```
2. Navigate to the project directory:
   ```sh
   cd examproject
   ```
3. Open `index.html` in your web browser to start the application.

## Usage

1. **Sign Up**: Register a new user by providing an email and password.
2. **Login**: Log in with the registered email and password.
3. **Take the Exam**: 
   - Navigate through the questions using the "Previous" and "Next" buttons.
   - Skip questions and come back to them later if needed.
   - The timer will count down from 2 minutes, turning red when less than 1 minute remains.
4. **Submit the Exam**: After answering the questions, submit the exam to see your results.
5. **View Results**: The results page will display your score and which questions were answered correctly or incorrectly.

## File Structure

```
/project-root
├── /assets
│   ├──/css
│   │  │── style.css
│   │  ├── login.css
│   │  ├── signup.css
│   │  └── exam.css
│   └──/js
│      ├── signup.js
│      ├── login.js
│      └── exam.js
├── index.html
├── signup.html
├── login.html
└── exam.html
```

## Functionality

### HTML

- **index.html**: Landing page with navigation to Sign Up and Login pages.
- **signup.html**: Sign-up page for user registration.
- **login.html**: Login page for user authentication.
- **exam.html**: Exam page with multiple-choice questions, timer, and result display.

### CSS

- **styles.css**: Contains styles for all the pages, including form styles, button styles, and result display styles.

### JavaScript

- **signup.js**: Handles user registration and stores the user data in `localStorage`.
- **login.js**: Handles user login by verifying the credentials from `localStorage`.
- **exam.js**: Manages the quiz functionality, including loading questions, navigation, timer, and result calculation.

### Key Functions in `exam.js`

- **loadQuestion(index)**: Loads the specified question and its choices, shuffling the choices each time.
- **updateNavigationButtons()**: Updates the state of the "Previous" and "Next" buttons.
- **prevQuestion()**: Navigates to the previous question.
- **nextQuestion()**: Navigates to the next question.
- **skipQuestion()**: Skips the current question.
- **saveAnswer()**: Saves the selected answer for the current question.
- **submitExam()**: Submits the exam and displays the results.
- **startTimer(duration, display)**: Starts the countdown timer for the exam.

## Credits

This project was developed by Ahmed Fathelbab. Feel free to use and modify the code as needed. Contributions are welcome!
