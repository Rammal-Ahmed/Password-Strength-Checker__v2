# Password Strength Checker (Version 2)

![Python](https://img.shields.io/badge/Python-3-blue)
![Version](https://img.shields.io/badge/Version-2.0-green)
![Type](https://img.shields.io/badge/Type-CLI-lightgrey)

A command-line program written in Python that checks how strong a password is.
You type a password, it tests five rules, shows a tick or cross for each one,
and gives a final rating: **Strong**, **Medium** or **Weak**. You get three tries.

This is **Version 2** of my Password Validator, rebuilt to be cleaner, more
detailed and closer to how a real tool would behave. I made it while learning
Python in my AI data science and data analytics course.

## What's new in Version 2

The first version only checked for letters, a number and an `@` sign, and gave
a simple pass or fail. This version is a clear step up:

| | Version 1 | Version 2 |
|---|---|---|
| Rules checked | Letters, a number, an `@` sign | 5 full rules: length, uppercase, lowercase, number, special character |
| Special characters | `@` only | Any of `@ # $ % & !` |
| Feedback | One pass/fail result | A ✔ / ✘ line for every rule, so you see exactly what is missing |
| Result | Accepted or rejected | Strength rating: Strong, Medium or Weak |
| Attempts | Single check | Three tries with a counter |
| Code structure | One script | Separate functions, constants, and a `main()` entry point |

## What it checks

| Rule | Requirement |
|------|-------------|
| Length | At least 8 characters |
| Uppercase | At least one capital letter |
| Lowercase | At least one small letter |
| Number | At least one digit |
| Special character | At least one of `@ # $ % & !` |

## How the rating works

- **Strong**: all 5 rules passed
- **Medium**: 3 or 4 rules passed
- **Weak**: 2 or fewer rules passed

## How to run

1. Make sure Python 3 is installed.
2. Clone the repository:
   ```
   git clone https://github.com/Rammal-Ahmed/Password-Strength-Checker.git
   ```
3. Open the folder and run:
   ```
   python password_strength_checker.py
   ```

## Sample output

```
========================================
        PASSWORD STRENGTH CHECKER
========================================

Enter a Password (try 1/3): hello123

  ✘  At least 8 characters
  ✘  An uppercase letter
  ✔  A lowercase letter
  ✔  A number
  ✘  A special character (@#$%&!)

Strength: Weak
Please try again.

Enter a Password (try 2/3): Hello@2026

  ✔  At least 8 characters
  ✔  An uppercase letter
  ✔  A lowercase letter
  ✔  A number
  ✔  A special character (@#$%&!)

Strength: Strong
Password Accepted. Well done!
```

## What I practised

- `for` loops with an `else` block
- Functions and constants
- Dictionaries and `any()` for rule checking
- Formatted console output

## Ideas for Version 3

- Hide the password while typing with `getpass`
- Reject very common passwords like `password123`
- Add a small GUI version

## About me

**Rammal Ahmed**

**AI & Data Science Enthusiast** | **Microsoft Dynamics 365 CRM Developer** | **Power Platform** | **UI/UX Designer** | **Graphic Designer & Illustrator**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rammal-ahmed-58184b325)
[![GitHub](https://img.shields.io/badge/GitHub-Rammal--Ahmed-181717?style=flat&logo=github)](https://github.com/Rammal-Ahmed)

<div align="center">

If you found this useful, consider giving it a star ⭐

**I truly value your feedback and welcome any suggestions for improvement**

**Always open to fresh perspectives, constructive feedback, and new ideas**


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

**Project Status:** Completed

</div>
