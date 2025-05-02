---
title: Automatic Grading System for first year Computer Science Courses
slug: autograding-cs
---
## Intent

Guidelines to develop a reliable automated feedback and grading systems for simple coding problems (e.g. as used in first-year Computer Science (CS) courses)', going beyond the simple pass/failing of test cases.

## Problem

Automatic grading systems have the potential to be highly beneficial in CS courses. By providing immediate feedback to coding exercises, they could help guiding students in their coding practices. Additionally, they could reduce bias and guarantee a more uniform grading. However, when automatic grading is achieved only by scoring passed or failed test cases (checking if the students output matches the expected output for a given input), the feedback provided to the students can be too limited and fail to reward correct elements the student was able to include in their solution.

## Solution

This play guides the reader through steps they can take to create a more pedagogically sound automatic grading system, using Bash scripting.

## Applicability

The proposed automatic grading system could be beneficial to first year CS students or other beginner programmers by providing them with immediate feedback for their coding exercises. The Bash scripting implementation is flexible and can adapt to different frameworks (the source's authors have used it in the Virtual Programming Lab (VPL), a plugin for the Moodle learning environment, and MULE, a browser-based Integrated Development Environment (IDE).

The proposed solution may require some investment in terms of time and effort to create the necessary scripts and test cases for each coding exercise. 

This grading system may not be suitable for the grading of more complex coding exercises. 

## How to Implement

The automatic grading system, which operates using Bash scripting, should carry out the following actions:
1. Compile the students code and check for errors. If compilation errors occur, the student should be informed through an error message so that they can fix their solution. At this stage, it is also important to check that the submission is not empty.
2. Use `grep` functionality to identify patterns that match to concepts being assessed. Regular expressions (regex) are used to find patterns in the code that match concepts in the programming language of choice, even if they are not entirely correct (e.g. commas instead of semicolons are used in a Java for loop).
3. Provide input and expected output for a series of test cases to verify that the student's solution works correctly. Test cases should have enough coverage to guarantee that all requirements are met. For failed test cases, the proposed solution's output and the expected correct output are shown to the student so that they can take steps to fix the issue. 
4. Assign marks appropriately for: 
    1. Providing a solution that compiles
    2. Including in the solution code constructs that match the topics being assessed
    3. Passing the test cases
5. Provide feedback for the students. This may happen at different stages of the exercise (if the code does not compile, if the expected code constructs are not included, and/or if the solution fails test cases).

## Source

Source: Hegarty-Kelly, Emlyn, and Dr Aidan Mooney. "Analysis of an automatic grading system within first year computer science programming modules." In Proceedings of the 5th Conference on Computing Education Practice, pp. 17-20. 2021. DOI: https://doi.org/10.1145/3437914.3437973

Described by: Giulia Toti, giulia.toti@ubc.ca

## Community Discussion

Community members are free to comment on, ask questions about, share
experiences, or otherwise contribute to knowledge about this play by
posting comments below.
See {% include chapter-link.html slug="join-discussions" %} for details.

* Insert a comment here.

Automated grading is certainly the way to go, but it needs to be bulletproof, especially in introductory courses, and especially for coding assignments that are built-upon over time. I was advising a student who had fallen behind in a self-paced course that had automated the grading system – the course was a prerequisite to progress in the degree. I had the student walk me through how she was working through the coding assignment, which had a series of automated test data that were run to test her code. Each and every version of code had to be checked into GitHub before testing would proceed. What she did not understand was that she was breaking the code that had worked on earlier tests to pass later ones, and then the earlier tests were failing without telling her why. While she eventually understood this, she was already past the midterm stage and eventually failed the course and had to repeat it. Not only does automated grading need to be bulletproof, but students also need to be comfortable asking for help and receiving it in a timely manner. An AI assistant could be useful here, assuming it had specific knowledge of how the automated grading system worked and could coach a student through some of the rough spots or provide hints to lines of specific code that are problematic. In lieu of this, students should have ready resources to visit their instructor or TAs, and receive SMART feedback. In large introductory classes, this may be difficult to achieve. A fee-based automated grading tool like PrairieLearn would be great to adopt, but it may be cost-prohibitive for some public institutions.