# Password Strength Checker

A lightweight, browser-based tool that evaluates password strength using basic security guidelines and provides real-time feedback to help users create stronger passwords.

**Live Demo:** [Try Password Strength Checker](https://darshankalburgi19.github.io/password_strength_checker/)

**Repository:** [GitHub Repository](https://github.com/DarshanKalburgi19/password_strength_checker)

---

## Overview

Password Strength Checker is a simple web application developed using HTML, CSS, and vanilla JavaScript.

It evaluates a password based on its length, character variety, and predictable patterns. As the user types, the application updates the strength estimate, visual progress bar, security checklist, and improvement suggestions.

The project was developed as an educational prototype to demonstrate front-end development, JavaScript logic, input handling, and basic software testing concepts.

## Features

- **Real-Time Evaluation:** Updates the password strength estimate while typing.
- **Strength Classification:** Categorizes passwords as Weak, Medium, or Strong.
- **Visual Strength Meter:** Displays a progress bar based on the calculated score.
- **Security Checklist:** Checks password length, uppercase letters, lowercase letters, numbers, and special characters.
- **Improvement Suggestions:** Provides feedback on missing security criteria.
- **Common Pattern Detection:** Identifies certain predictable starting patterns such as `password`, `qwerty`, `admin`, `12345`, and `letmein`.
- **Show/Hide Password:** Allows users to toggle password visibility.
- **Responsive Interface:** Adapts to different screen sizes.
- **Privacy-Focused Processing:** Evaluates passwords locally in the browser without sending or saving the entered password.

## Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling, layout, and responsive design |
| JavaScript | Password evaluation and dynamic functionality |
| GitHub Pages | Application hosting and deployment |

No external libraries, frameworks, backend server, or database are required.

## How It Works

The application evaluates the entered password using a rule-based scoring system.

### Evaluation Criteria

| Criterion | Score |
|---|---:|
| At least 8 characters | +15 |
| At least 12 characters | +20 |
| At least 16 characters | +15 |
| Contains uppercase letters | +10 |
| Contains lowercase letters | +10 |
| Contains numbers | +10 |
| Contains special characters | +15 |
| At least 8 unique characters | +5 |
| **Maximum Score** | **100** |

If a password begins with one of the recognized common patterns, its score is capped at 25.

### Strength Classification

| Score | Classification |
|---|---|
| Below 40 | Weak |
| 40–69 | Medium |
| 70–100 | Strong |

The application also updates the checklist and displays suggestions based on the password's characteristics.

**Important:** This is an educational scoring heuristic, not a cryptographic password-strength estimator. It does not calculate password entropy, check breached-password databases, or guarantee account security.

## Application Architecture

The application follows a simple client-side architecture:

```text
        USER
          |
          v
    WEB BROWSER
          |
          v
   HTML + CSS LAYER
   (User Interface)
          |
          v
   JAVASCRIPT LAYER
   (Password Evaluation)
          |
          v
   RESULT DISPLAY
          |
    -----------------
    |       |       |
  Score  Checklist  Suggestions
```

All password evaluation takes place inside the user's browser.

## Getting Started

You can run the project locally without installing any additional dependencies.

### 1. Clone the Repository

```bash
git clone https://github.com/DarshanKalburgi19/password_strength_checker.git
```

### 2. Open the Project Folder

```bash
cd password_strength_checker
```

### 3. Run the Application

Open `index.html` in any modern web browser.

Alternatively, open the file directly from your file manager.

No build process or local server is required.

## Testing

The application can be evaluated through manual functional testing.

Important testing scenarios include:

- Opening the application and checking its initial state.
- Entering passwords of different lengths.
- Checking uppercase, lowercase, numeric, and special characters.
- Testing recognized common password patterns.
- Verifying Weak, Medium, and Strong classifications.
- Checking real-time updates while typing.
- Testing the Show/Hide password functionality.
- Refreshing the application and checking its initial state.
- Checking the interface on different screen sizes.

## Privacy and Security Considerations

- Password evaluation is performed locally in the browser.
- The application does not send entered passwords to a backend server.
- The application does not save entered passwords.
- No database or external password-checking service is used.

**Safety recommendation:** Use sample passwords for testing. Never enter a password that you currently use for an important account.

## Limitations

- Uses a basic rule-based scoring system.
- Does not perform cryptographic entropy analysis.
- Does not check passwords against known data breaches.
- Does not identify every possible dictionary word or predictable password pattern.
- A Strong classification does not guarantee that a password is secure.

## Future Improvements

Possible future enhancements include:

- Integration with a more advanced password-strength estimation algorithm.
- Detection of additional weak and predictable password patterns.
- Optional breached-password checking through a privacy-preserving service.
- More detailed password improvement recommendations.
- Accessibility and interface improvements.

## Deployment

The application is hosted using GitHub Pages.

**Live Application:**  
https://darshankalburgi19.github.io/password_strength_checker/

**Source Code:**  
https://github.com/DarshanKalburgi19/password_strength_checker

## Author

**Darshan Kalburgi**

GitHub: [@DarshanKalburgi19](https://github.com/DarshanKalburgi19)

---

*Developed as an educational project to demonstrate web development, JavaScript-based logic, and software testing concepts.*
