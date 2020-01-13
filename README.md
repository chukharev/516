# ENGL 516 - Methods of Formal Linguistic Analysis

**Catalog description:** Data and knowledge structures for formal representation of natural language and speech data. Designing and implementing algorithms for automating linguistic analysis tasks. Conceptual issues for natural language and speech processing programming.

**Textbook (required):** [Eloquent Javascript, 3rd edition](https://eloquentjavascript.net/) by Marijn Haverbeke. There is a free online version and a [paperback](https://www.amazon.com/Eloquent-JavaScript-3rd-Introduction-Programming/dp/1593279507/) for $25.

## Tentative Schedule

- W1: [Introduction](https://eloquentjavascript.net/00_intro.html). Foundations of information theory. Numeral systems. [Slides](week1_slides.pptx); [Homework assignments](week1.md)
- W2: Representing information in the computer: logic, numbers, colors, text. [Slides](week2_slides.pptx)
- W3: Representing information in the computer (continued); [Chapter 1: Values, types, and operators.](https://eloquentjavascript.net/01_values.html) [Slides](week3_slides.pptx); [Homework assignments](week3.md)
- W4: [Chapter 2: Program structure.](https://eloquentjavascript.net/02_program_structure.html) See [Chessboard solution](week4_chessboard.txt)
- W5: [Small Project A: Number Guessing Game](#small-project-a) (5%). See [scaffolding assignments](scaffolding.md)
- W6: [Chapter 3: Functions.](https://eloquentjavascript.net/03_functions.html)
- W7: [Small Project B: Caesar Cipher](#small-project-b) (5%).
- W8: [Chapter 4: Data structures: objects and arrays.](https://eloquentjavascript.net/04_data.html)
- W9: [Small Project C: Learner Modeling](#small-project-c) (5%).
- W10: [Chapter 9: Regular expressions.](https://eloquentjavascript.net/09_regexp.html)
- W11: [Small Project D: Haigy Paigy](#small-project-d) (5%). **[Final project](final_project.md) proposals due on Friday**
- W12: [Small Project E: Corpus Processing](#small-project-e) (5%); see [in-class demo code](https://github.com/chukharev/516/blob/master/nov13_demo.html)
- W13: Oral exam - 25% - based strictly on Small Projects A-E. **[Final project](final_project.md) paper drafts due on Friday**
- W14: [Chapter 13: JavaScript and the Browser.](https://eloquentjavascript.net/13_browser.html)
- W15: Final Project Presentations (Final project worth 30%).
- Finals week: Written final exam (worth 20%). **[Final project](final_project.md) papers and programs due on Friday**

## Course Assessment Plan

- Five small projects (A-E): 5% each, 25% total (rubric provided on the assignment sheet for each small project)
- Oral exam based on the small projects: 25% (rubric provided on the study guide)
- Final project: 30% (rubric provided on the assignment sheet)
- Written final exam: 20% (rubric provided on the study guide)

## Course Policies

**Collaborative work.** You may use the help of others to work on your projects. However, you must retain
ownership (authorship) of the code that you submit. If someone helps you write a fragment of your code,
the best way to ensure that you retain ownership is to re-write that fragment of code on your own without
looking at the code that your helper wrote for you. If you borrow code from an online source, you should
cite that source in a comment, e.g.:

```js
// Quick Search implementation from: https://stackoverflow.com/questions/22697936/binary-search-in-javascript
```

The oral exam will be used to ascertain your ownership of the code that you have submitted.

**Attendance and participation.** There are no points for attendance and participation. You can miss any
number of class meetings without penalty. You must complete all coursework regardless of your presence in class.
Please be aware that regular class attendance and active participation is a strong predictor of your final grade
(i.e. non-attending and non-participating students have historically received low grades in this course).

**Preparing for class.** Before each class meeting, you are expected to have done all of the following:

- read and understand the contents of the assigned book chapter;
- run all code examples given in the text of the chapter and make sure that you understand them;
- without looking at solutions, attempt all exercises given at the end of the chapter.

Preparing for class strongly predicts success in learning.

## Assignment Sheets

### General Notes

#### Submission deadlines

Each small project is due by the end of day (23:59) on Wednesday following the week when the project is assigned.
Grades will be given by the end of day on Friday of the week when the project is due.
Formative feedback will be provided by the end of day on Wednesday of the following week.
To keep you on track with the class, late submissions are strongly discouraged. If you must submit a small project late,
you must tell me in advance.

#### Submission procedure

I will access your GitHub
repository after the deadline to retrieve your project file. For each small project, create a file
in your GitHub repository named **projectx.html**, where **x** is the letter designation of the project (**a**-**e**).
Your file name should not contain quotes, spaces,
or any other symbols. Please also note that file names are case sensitive,
so "PROJECTA.HTML" and "projecta.html" are two different files. After you
complete your assignment, do not forget to "commit master" and "push
origin." Make sure that your program carefully follows the input/output protocol described in the assignment directios.

### Small Project A
### Number Guessing Game

**Learning outcome:** After completing this assignment, you will have learned how to
conceptualize and implement in code a simple algorithm. Algorithms are a
foundation of computer science and computational linguistics.

**Broader impact:** The algorithm you will implement in this small project is one of the
fundamental alrogithms used in adaptive computer-assisted language testing. ALT students
have used this algorithm to develop an adaptive test of vocabulary size.

**Programming concepts:** while-loop, binding, string, number, string comparison, condition.

#### Task

Create a web page with an embedded JavaScript program that plays the
"number guessing game" with the user as follows:

1. The user thinks of an integer between 1 and 100 (inclusive).
2. The program needs to repeatedly take guesses at the number the user has in mind.
3. To each of the program's guesses, the user responds "<" if the target
number is less than the program's guess; ">" if the target number is
greater than the program’s guess; or "yes" if the program has guessed the
number correctly.

You need to come up with and implement the most efficient strategy for your
program.

#### Sample game

- Your program (prompt box): `Is your number 23?`
- User (enters into the prompt box): `<`
- Your program: `Is your number 1?`
- User: `>`
- Your program (prompt box): `Is your number 14?`
- User (enters into the prompt box): `yes`
- Your program (alert box): `I won!`

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program follows formatting guidelines: 1 point.
- Your program is able to guess numbers: 1 point.
- Your program guesses numbers in the most efficient way: 2 points.

### Small Project B
### Caesar Cipher

**Learning outcome:** After completing this assignment, you will have learned how to process
strings of text on a character-by-character level, how to extract
characters from strings, how to concatenate strings, and how to convert
characters to their ASCII codes and back.

**Broader impact:** The concepts you will master through this small project are used, explicitly
or implicitly, in all text processing applications.

**Programming concepts:** for-loop, string, character, ASCII code, modular arithmetic; you may want to use [charCodeAt()](https://www.w3schools.com/jsref/jsref_charcodeat.asp) and [fromCharCode()](https://www.w3schools.com/jsref/jsref_fromcharcode.asp).

#### Task

Create a web page with an embedded JavaScript program that implements
Caesar cipher with a user-specified shift for the upper-case and lower-case
English letters. The letters must wrap around.

1. The user is shown a first prompt box and asked to enter a positive or
negative integer representing the desired shift. For example, a left
shift of 3 places would be represented as -3; a right shift of 1 place
would be represented as 1.

2. The user is shown a second prompt box, asking to enter the source
(unencrypted) text.

3. The user is shown an alert box with the encrypted text.

In the encryption process, only letters A-Z and a-z are encoded; other
characters must be left untouched.

#### Sample input/output

- Your program: `Enter shift`
- User: `-5`
- Your program: `Enter text`
- User: `Hello, world!`
- Your program: `Czggj, rjmgy!`

**Note:** The wording of the prompts "Enter shift" and "Enter text" is not
prescribed, but the sequence of prompt boxes must follow the task
description.

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program follows formatting guidelines: 1 point.
- Your program correctly encodes strings that I supply: 3 points.

### Small Project C
### Learner Modeling

**Learning outcome:** After completing this assignment, you will have learned how to model
language learning goals and the current state of language learner using data structures (objects
and arrays) in JavaScript. You will also learn how to develop simple adaptive computer-assisted
language learning algorithms.

**Broader impact:** Learner modeling is a cornerstone of all intelligent CALL and CAT applications.

**Programming concepts:** array, object, random.

#### Task

Write a program that teaches English prepositions using a series of fill-in-the-blank exercises. Each
exercise will be in the following format:

`Are you wearing anything ___ your sweater?`

That is, the exercise will have a sentence with a preposition replaced with a sequence of underscores.
The user of your program will be an English language learner. The user will complete each exercise by
entering the preposition which, in the user's opinion, should be inserted in place of the blank. For example,
a response to the exercise shown above might be:

`underneath`

Your program will show each exercise in a prompt box. After the user enters their response, your program will display
an alert box which can have one of the following two messages:

- a message saying `Correct!` if the user's response was correct; or
- a message displaying the sentence with the correct preposition, for example: `Are you wearing anything underneath your sweater?` if the user's response was not correct.

After presenting this feedback to the user, the program will  move on to displaying the next exercise.

Your program will be tracking the user's progress in the learning of each preposition. At each step, the program
will provide an exercise targeting the preposition which the user has mastered to the least extent. Mastery level
for the preposition *x* should be calculated as the number of times the user has gotten the preposition *x* correct
in exercises less the number of times the user has gotten the preposition *x* wrong.

For example, if learner A responds to two items on preposition *x* and answers them both correctly, then his mastery level for preposition *x* will be 2. If learner B responds to 4 items on preposition *x*, but answers only 2 of them correctly, then his mastery level will be 0.

You should use a JavaScript object in your program to track the user's mastery levels for all prepositions.

You should develop your program so that it supports at least five different prepositions and provides at least
five different exercises for each preposition that your program supports.

#### Sample input/output

- Your program (prompt box): `There is a table ___ the room.`
- User (enters into prompt box): `on`
- Your program (alert box): `There is a table in the room.`
- Your program (prompt box): `The train will arrive ___ two hours.`
- User: `in`
- Your program: `Correct!`

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program follows formatting guidelines: 1 point.
- Your program supports 5 prepositions, and for each preposition it supports 5 possible sentences: 1 point.
- Your program implements a tutoring algorithm consisent with the assignment: 2 points.

### Small Project D
### Haigy Paigy

**Learning outcome:** Through completing this assignment, you will learn to
use regular expressions in JavaScript to perform search and replace operations on strings.
You will also learn to "translate" conceptual definitions of applied linguistic problems into
formal instructions that are programmable for the computer.

**Broader impact:** Regular expressions are helpful in most text processing applications.
Formalizing linguistic problems is a crucial step in programming for any applied linguistic task.
ALT students have widely used regular expressions in their coursework and dissertation projects.

**Programming concepts:** regular expressions.

#### Task

Haigy Paigy is a children's invented language which sounds exactly like English, except that "aig" is inserted before
the rime of each syllable. E.g., the English word "hello" becomes "haigellaigo" in Haigy Paigy.

Write a program in JavaScript that will prompt the user to enter a sentence, automatically translate it from English
into Haigy Paigy, and display the result of the translation as an alert box. In your program, you will need to write
a set of regular expressions that will translate the input sentence into Haigy Paigy.

**Simplifications:** only vowels can be syllable nuclei; the letter "y" always makes a vowel sound; several consecutive
vowel letters always make a single vowel sound; the final "e" is always silent, except when it is the only vowel letter
in the word.

#### Sample input/output

- User: `This is a test.`
- Your program: `Thaigis aigis aiga taigest.`

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program follows formatting guidelines: 1 point.
- Your program correctly translates sentences that I supply: 3 points.

### Small Project E
### Corpus Processing

**Learning outcome:** After completing this assignment, you will have learned how to pre-process
a corpus automatically using string operations in JavaScript, and how to derive basic corpus statistics
based on word counting.

**Broader impact:** ALT students often write scripts for processing corpora for their coursework
and dissertation projects.

**Programming concepts:** split, toUpperCase, toLowerCase, sort.

#### Task

Develop a JavaScript program that does all of the following:

- Asks the user to copy and paste a text into an edit box on the web page.
- Removes punctuation and extra white space.
- Casts all words to the upper case.
- Counts the number of tokens and types in the text.
- Displays a frequency dictionary of the types found in the text, sorted by descending frequency.
- Calculates and displays the type/token ratio.

Please use this [boilerplate file](https://github.com/chukharev/516/blob/master/project_e_boilerplate.html) to assist you with the development of the user interface for this program.

#### Grading (5 points total)

- Your program is syntactically correct: 1 point.
- Your program follows formatting guidelines: 1 point.
- Your program displays the frequency dictionary correctly: 2 points.
- Your program calculates and displays TTR correctly: 1 point.

## Study Guides

### Oral Exam

For the oral exam, I will make an individual one-hour appointment with each student.
We will not meet as a class during the week of oral exam.
The goal of the oral exam is to ascertain your ownership of the code you submitted for the five small projects.

During the exam, I will ask you questions about the code that you have submitted. If you wrote the code yourself,
you will find it easy to answer my questions. I will also ask you to make small changes to your code. Again, if
you have ownership of the code, you will not find it very difficult to make the changes I request.

For each of the five small projects, your performance at the oral exam will be graded according to the following rubric:

- 1 point: you demonstrated no knowledge of programming concepts required to complete the assignment;
- 2 points: your knowledge of programming concepts is unsatisfactory;
- 3 points: there is a serious flaw in your mastery of programming concepts necessary to complete the assignment;
- 4 points: you have a solid knowledge of the relevant programming concepts, but you made a minor mistake;
- 5 points: your knowledge and mastery of the relevant programming concepts is very solid.
