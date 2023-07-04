# Knowledge Comprehension AI

## Summary
This AI should read the exam´s questions and results so it can:
* Suggest how to Fix the way a question is asked so it may assure is correctly comprehended.

And report
* A list of the less comprehended topics/concepts by the students.
* A list of the less-mentioned words by the students.

## Background
* Professors ask questions based on the topics/knowledge they require the student should know. 
* Each professor has their way of writing questions.
* Maybe there is a correlation between the way a question is asked and the given answer.

## How is it used?
It may be used to fix the way questions are asked and clear the misunderstanding of wrong-asked questions. 
It also can improve the way professors.

## Data sources and AI methods
Database of all the main words contained in the most wrong-answered questions

Example

* Suppose it is known in a certain exam that there is a 1 in a 1000 chance that a student answers wrong because of a certain word. 
* Suppose it is also known that a word is read 99% accurate?
* What is the probability that a student who answered wrong misread that word?

To find the solution: 
P(H), P(E/H), and P(E).

P(H) = 1/1000 = 0.001 (Since there is a 1% chance of inaccurate reading)

P(E/H) = 0.99 this is given since 99% of the time is a known word.

Now P(E) = P(E/H) x P(H) + P(E/~H) x P(~H), where ~H means you don't know it.

So, P(~H) = 99/100 = 0.999.

And, P(E/~H) = 0.01

Hence, P(H/E) = 0.99 x 0.001/ (0.001 x 0.99 + 0.999 x 0.01) = 0.09.

This means that the student would have a 9% chance of a correct answer not knowing the word.


## Challenges
* Several data years of the same exam
* Typing a lot of data
* Get basic information of each person who answered the exam

## What next?
* Find a list of big-scale exams that may have not changed in several years and get the approval to be tested.

## Acknowledgments
There are uncontrolled factors such as:
* Previous Knowledge of each student
* Metal condition at the time the exam is answered
* Stress Factor
