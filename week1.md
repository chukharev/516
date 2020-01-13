# Week 1 Homework Assignments

## A. Prepare answers to the following questions:

1. How many bits of information does a four-digit decimal integer (a whole number in the range between 0000 and 9999, inclusive) contain?

2. Mother tells her child: "If you wash the dishes, then you can go play with your friends." The child does not wash the dishes, but still goes play. Using propositional logic, determine if the child has violated their mother's directions. Let D be 'the child washed the dishes', let P be 'the child played'. Express mother's directions as a compound proposition and determine its truth value. If you find a discrepancy between formal logic and intuition, explain it and re-word the directions using different connectives.

3. Determine the truth value of the compound proposition ((A ∧ (A → B)) → B) for all possible combinations of truth values of the constituent atomic propositions A and B. What is special about this compound proposition? In what ways propositions like this one may be useful?

4. In Europe, dates are written as DD-MM-YYYY (day, month, year), while in many Asian countries the order is YYYY-MM-DD (year, month, day). Which of these two notations is big-endian and little-endian? Which notation is more conisistent with the endianness of the decimal system? What do you think about the way dates are written in the U.S.?

> Note: It is helpful to write down your answers so that you can discuss them with your classmates in class, but you do not need to submit them to the instructor for grading.

## B. Perform the following conversions and be prepared to explain the process that you followed:

1. Convert 7E3<sub>16</sub> to the decimal system.
2. Convert AB<sub>16</sub> to the binary system.

> Note: It is helpful to write down your answers so that you can discuss them with your classmates in class, but you do not need to submit them to the instructor for grading.

## C. Complete the following step-by-step instructions:

1. [Set up your GitHub account](setup_github.md)
2. Submit this assignment by going to the [course website](https://linguatorium.com/portal/) and clicking on "Submit your assignment" under "Setting Up GitHub".

## D. Verify that you understand answers to the following problems (and the thought process behind obtaining these answers):

1. How much information is there in a coin toss? a single dice roll? *(Answers: 1 bit; ~2.58 bits)*

2. Alice is telling Bob about the outcome of the U.S. presidential election (Bob doesn't have prior knowledge of the outcome). The speed of the network connection between Alice and Bob is 10 Mbps (megabits per second). How long will it take Alice to transmit this information to Bob over this network connection? *(Answer: 1/10,000,000-th of a second, or 100 nanoseconds)*

3. Eight teams are playing a soccer tournament using the single-elimination principle: They first play the quarter-final round; then in the semifinal round only four are left; then the two winners of the semifinals meet in the final round to determine the champion. In total, 4 quarter-final matches + 2 semifinal matches + 1 final match = 7 matches are held. Each match contributes one bit of information, so the total information of the tournament is 7 bits. On the other hand, since the tournament selects one champion out of eight teams, the information of the tournament should be log<sub>2</sub>(8) = 3 bits. Explain the inconsistency. *(Answer: The tournament yields additional information besides who came first, i.e. who came second, etc.)*

4. How much information is there in a three-letter English word? Will this amount of information be different for those who know English and for those who don't? Is it possible that the amount of information will vary depending on the word? If so, under what circumstances? *(Answer: The amount of information vary based on the word and the level of the reader's knowledge of English; for non-learner of English who knows the English alphabet, 14.1 bits.)*

5. Alice and Bob are playing the 20-question game. Alice thinks of a natural number from a predefined range, and Bob tries to guess it by asking Alice yes/no questions. What largest predefined range of possible numbers would guarantee that Bob will win the game (using the best-available strategy) regardless of which particular number from the range Alice selects? (<i>Answer: 1 ... 2<sup>20</sup></i>)

