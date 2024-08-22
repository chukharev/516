# ENGL 5160 "Methods of Formal Linguistic Analysis"

**Catalog description:** Data and knowledge structures for formal representation of natural language and speech data. Designing and implementing algorithms for automating linguistic analysis tasks. Conceptual issues for natural language and speech processing programming.

**Course Materials:** The Python Workbook by Ben Stephenson, freely available from the publisher here (log in through ISU library is required to gain free access to the book): https://link.springer.com/book/10.1007/978-3-030-18873-3

**Learning Objectives:**

After completing this course, you will be able to:

- understand the scope and goals of computer programming in applied linguistics research and practice
- develop scripts in Python that manipulate textual data using built-in methods, regular expressions, and character-wise operations
- implement data analysis procedures using lists, dictionaries, and loops
- implement computational procedures that input and output plain text files
  
**Required Technology:**

A laptop

**Course Requirements:**

1. Class participation and project work (20%)
2. In-class quizzes (10% each, total 70%)
3. Individual oral examination (10%)

**1. Class participation:**

You are expected to attend each class session on time and to be prepared with completed assignments, including small projects that are relevant to the applied linguistics field. You should be prepared to actively participate in class discussions and to demonstrate that you have
adequately prepared for the class session. Attendance is expected in this class, although there is no
automatic grade penalty for missing a specific number of class sessions. If you do miss class, it is your
responsibility to catch up with the material by obtaining notes from a classmate.

**2. Seven quizzes:**

We will complete seven paper-based, in-class quizzes throughout this course. These will be designed to allow you to
demonstrate your knowledge of key concepts and mastery of skills that we will learn in class. If you miss a quiz (or miss any points on a quiz that you wish to make up for), you will have an opportunity to answer similar questions during your individual oral exam appointment.

**3. Individual oral examination:**

Toward the end of the semester, I will schedule an individual meeting with every student to assess their
knowledge and skills.

**Tentative Schedule (subject to change)**

| Weeks | Topic |
|------|-------|
| 1 | Introduction |
| 2 | Python programming |
| 3-4 | Decision making |
| 5-6 | Repetition |
| 7-8 | Lists |
| 9-10 | Regular expressions |
| 11-12 | Dictionaries |
| 13-14 | Files |
| 15 | Oral exams |

# Project 1: Python Programming

Two researchers independently annotated the pronunciation of *N* minimal-pair utterances by language learners. Each utterance was annotated as containing either the phoneme **A** or the phoneme **B**. The annotation task was a binary forced-choice task, and both researchers annotated all *N* utterances without skipping any of them. Assume that the probability of each phoneme in an utterance was *p*(*A*) = *p*(*B*) = .5. The two researchers agreed in their annotation decisions for *M* utterances.

Develop a program that asks the user to input two integers: *N* and *M*. These numbers must be requested in this sequence. Calculate and output two measures of inter-annotator agreement: (1) simple percent agreement and (2) Krippendorff’s alpha. Calculate simple percent agreement between the annotators as the proportion of utterances on which the annotators agreed. Calculate Krippendorff's alpha using the formula: *alpha* = 1 – *Do*/*De*, where *Do* is the observed rate of disagreement between the annotators (i.e., the proportion of utterances on which the annotators disagreed) and *De* is the rate of disagreement between annotators that is expected by chance (in this example *De* = .5). Simple percent agreement and Krippendorff's alpha must be output as decimal fractions with two digits after the decimal point.

# Project 2: Decision Making 

A frequent task in automated writing evaluation (AWE) is computationally generating the correct 
(expected) text to determine whether the text produced by the writer matches this expectation (and if it  doesn't, then, for example, feedback to the writer may be provided).

For this assignment, you will develop a program that generates the expected indefinite article for an English singular noun. Your program should ask the user to input a noun, and then should output this noun with an indefinite article ("a" or "an") in front of it. Use the following rules for determining the correct article: if the noun starts with a vowel, the article is "an"; if the noun starts with a consonant, the article is "a". Your program must take into account your choice of at least three exceptions (words that start with a "vowel letter" but a consonant sound, e.g. "a university", not "*an university"). 

**Sample input:** `apple`

**Sample output:** `an apple`

# Project 3: Repetion

A common statistical measure of central tendency is the trimmed mean, which is similar to the mean (average) of the sample values, but is calculated after certain parts of the sample at the high and low end are discarded. The idea behind calculating the trimmed mean is that removing outliers may improve the usefulness of the statistical measure.

Develop a program that computes the trimmed mean of a sample of test-takers' scores, discarding the 
maximum and the minimum values. For example, the trimmed mean of scores { 2, 3, 1, 4, 10.5, 10.5 } is 
(2+3+4)/3 = 3. In this example, the value 1 is discarded because it is the minimum value, and both of the 
values { 10.5, 10.5 } are discarded because they are the maximum values.

The user should be prompted to enter test-takers' scores one by one. Assume that all scores on the test are 
positive floating point numbers. The value 0 in user input will indicate that no further scores will be 
entered. Your program should then output the trimmed mean as a decimal fraction with three digits after 
the decimal point, or display an appropriate error message if there are not any values left in the sample 
after trimming.

Please note that in writing code for this project you _cannot_ use lists.

**Example input:**

2<br>
3<br>
1<br>
4<br>
10.5<br>
10.5<br>
0

**Example output:**

3.000

# Project 4: Lists 

In computational and corpus linguistics, an n-gram is defined as a contiguous sequence of n items from a 
given sample of text or speech (typically a corpus). The items can be phonemes, syllables, letters, or 
words, according to the specific application of n-gram modeling. 

Develop a program that takes two inputs (in this sequence): a string of text, and _n_ (the natural number signifying the quantity of elements in each n-gram).

Your program should output all word n-grams that appear in the input text. If an n-gram appears multiple times, it should only be output once. Output each n-gram on a 
new line. For this assignment, separate words by space only, consider lowercase and uppercase letters to 
be different, and do not remove or otherwise manipulate punctuation. The n-grams should be sorted alphabetically in your output.

**Example input:**
<br>how much wood would a woodchuck chuck if a woodchuck could chuck wood<br>3

**Example output:**
<br>a woodchuck chuck<br>a woodchuck could<br>chuck if a<br>could chuck wood<br>how much wood<br>if a woodchuck<br>much wood would<br>wood would a<br>woodchuck chuck if<br>woodchuck could chuck<br>would a woodchuck

# Project 5: Regular Expressions 

One of the most widely implemented steps in computational pipelines for the automatic processing of natural texts is data cleaning (normalization). The quality of data cleaning may determine the success of the downstream analysis procedures.

Develop a program that asks the user to enter a string of text and outputs the string after the following cleaning steps:

(1) sequences of non-alphanumeric characters should be replaced with a single space, with the exception of punctuation characters that should be preserved;

(2) extraneous spaces before or after punctuation characters (following the U.S. typesetting conventions) should be removed.

**Sample input:**

```
This is  ~~~ a test ! ***
```

**Sample output:**

```
This is a test!
```

# Project 6: Dictionaries 

Corpus methodologies in linguistics rely largely on counting the raw and normed frequencies of 
occurrence of features of interest, such as words or grammatical patterns, in text corpora (i.e., large and structured collections of texts).

Develop a program that takes as input a string of text, and outputs the frequency list of all words appearing in this text. The list should be sorted by descending raw frequency of occurrence. Each word should be cast to lowercase, output on a separate line, and followed by its raw frequency of occurrence (i.e., the number of times this word appears) in the input text. The word and its frequency should be separated by a single space character.

Assume that all words are separated by a single space character in the input text, and no punctuation is present in the input. For this assignment, upper-case and lower-case letters should not be treated as different letters. 

**Sample input:**

```
Hello hello world 
```

**Sample output:**

```
hello 2 
world 1
```

# Project 7: Files

For this project, you will be provided with a folder named `data` containing multiple plain text files. Each 
file contains multiple texts that are rated for holistic text quality. The name of each file is the name of the 
rater who performed text quality ratings in that file. For example, file name `Ted.txt` indicates that the 
rater Ted completed ratings within that file. Each file contains the texts being rated, where each text is 
followed by the rating of text quality in the following format:

```
***** ID:  7500-l6avln1x-j895n58yY ; RATING: 4 
```

Here `ID` is a unique identifier of the text, and `RATING` is the numerical rating of the holistic text 
quality of that text on an integer scale. 

Develop a program that outputs a spreadsheet in the CSV (comma-separated volume) format, where each 
row represents a text, and each column represents a rater. 
  
See example below: 

```
ID,Ted,Jane,Mary 
6452-fksjfksdjfsl,4,,3 
4567-cjansdhcsd,2,3,1 
...    
```

Note that not all raters have rated all texts, therefore some of the cells in the output spreadsheet will be 
blank. The output file must be named `ratings.csv` and placed in the `data` folder alongside the input text 
files. Note that your program will need to determine the list of text IDs and rater names automatically 
from the input text files that are provided. 

