# 📘 Grade Book

A simple JavaScript program that calculates the **class average**, determines a **student’s grade**, and outputs a message telling the student whether they passed or failed the course.

## 🚀 Features
- Calculates the **average score** of the entire class.
- Converts a student’s numeric score into a **letter grade** (`A`, `B`, `C`, `D`, `F`).
- Displays a custom message:
  - ✅ Passed the course
  - ❌ Failed the course

## 🛠️ Functions

### `getAverage(scores)`
- Takes an array of numbers (`scores`) as input.
- Returns the **average score** of the class.

### `getGrade(score)`
- Takes a single number (`score`) as input.
- Returns a **letter grade** based on the score:
  - `A` → 90 and above  
  - `B` → 80–89  
  - `C` → 70–79  
  - `D` → 60–69  
  - `F` → below 60  

### `studentMsg(totalScores, studentScore)`
- Takes an array of class scores and one student’s score.
- Uses `getAverage` and `getGrade` to calculate results.
- Returns a message including the class average, student’s grade, and pass/fail status.

## 💻 Example Usage

```js
console.log(studentMsg([92, 88, 12, 77, 57, 100, 67, 38, 97, 89], 37));
// ➡️ Class average: 71.7. Your grade: F. You failed the course.

console.log(studentMsg([56, 23, 89, 42, 75, 11, 68, 34, 91, 19], 100));
// ➡️ Class average: 60.6. Your grade: A. You passed the course.
