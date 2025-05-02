---
title: Specs grading plus grading for equity
slug: specs-plus-equity
---
## Intent

Utilize aspects of specifications grading and grading for equity to increase learner's motivation to learn.  

## Problem

Traditional points-based grading systems have been found to have a variety of concerns including the effectiveness, 
reliability, accuracy, and necessity of grading. 
In addition, intrinsic motivation has been found to be negatively impacted by points-based grading systems.
Learner's focus on grades for extrinsic motivation has been found to result in increases in learner anxiety and 
their motivation to cheat.

## Solution

This play combines aspects of specifications grading and grading for equity to achieve the goals of 
+ allowing for re-submission of assignments
+ retaking of examinations
+ reducing numeric grades, in favor of complete/incomplete

## Applicability

This play was implemented in three sections of an upper level undergraduate computer science elective course
(database systems). 
The three sections had a total of 67 learners.

There can be a significant burden to develop alternative versions of exams to allow for retakes. 
Also, extra time is needed to proctor examination retakes and evaluate regrade requests.

This play has not been implemented in other settings to know if the level or
enrollment of the course could impact its effectiveness.

## How to Implement

1.  **Assessment:** Manually assessed assignments are identified as complete or incomplete,
and included detailed feedback to allow the learner to improve. 
When automated assessment tools generate a numeric grade,
a numerical threshold of 85% was used to determine complete/incomplete.

2. **Regrade requests:** Although it may be philosophically desirable to allow unlimited regrades,
concerns about the number and quality of regrades can arise.
To reduce these concerns, establish category limits for each grade level.
For example, learners can submit a regrade request for up to 5 labs and/or reading activities while still 
meeting the A level.

The following table provides an example of how the course grade was determined.
Note that to earn a given course grade a learner must meet (or exceed) all specifications listed in that grade's column.
For example, if a learner had everything for A, but used 7 regrades, they would earn a C.
Also note that it is a combination of the quantity of items completed in relation to the quantity 
of re-takes/re-submissions that determines the course grade.

| Assignment (qty) | Goal             |                    A                    |                    B                     |                     C                     |
|---------------|------------------|:---------------------------------------:|:----------------------------------------:|:-----------------------------------------:|
| Readings (15)<br/><br/>Labs (23)<br/><br/>Regrades | Complete (> 85%)<br/><br/>Complete (> 85%)<br/><br/>Use no more than | All but 2<br/><br/>All but 2<br/><br/>5 | All but 3<br/><br/>All but 4<br/><br/>6  | All but 4<br/> <br/>All but 6<br/><br/>7  | 
|Exams (4)<br/><br/>Exam Retakes | Complete (> 85%)<br/><br/>Use no more than |             All<br/><br/>2              |           All but 1<br/><br/>3           |           All but 2<br/><br/>4            |
|Final Exam | Score at least |                 90%                  |                  80%                  |                  70%                   |

## See Also

_____________________List any other related plays here as a bullet list of chapter links.
Then remove this text._

## Source

Source: Ryan Stephen Mattfeld. 2023. 
Improving Student Motivation through an Alternative Grading System. 
_J. Comput. Sci. Coll. 39, 5 (November 2023)_, 86–95. 
https://doi.org/10.1145/3328778.3366956

Described by: David Largent (dllargent@bsu.edu)

________________Be sure to add the source
to {% include chapter-link.html slug="references" %} as well._

## References

________________Insert references to publications or web pages describing, evaluating, or
sharing experiences with this technique. Then remove this text._

## Community Discussion

Community members are free to comment on, ask questions about, share
experiences, or otherwise contribute to knowledge about this play by
posting comments below.
See {% include chapter-link.html slug="join-discussions" %} for details.

* Insert a comment here.

Are there are folks who support and use specs grading but are not bought into grading for equity? It seems like grading for equity incorporates many aspects of specs grading (using Talbert’s EMRN rubric or the GTMJ rubric introduced earlier). When combined with low-stakes assignments and regrading with SMART feedback whenever possible, I posit that grading for equity would generally result in stronger mastery than specs grading alone. It may be more challenging to implement and teach specs grading in a course that has been traditionally graded, especially if that course is a pre-requisite for continuing in the degree program or is an upper-level course required for graduation. If individual assignments are a binary pass/fail until mastery, student perceptions of success in the course may be impacted, so an instructor will have to continually socialize the message about mastery vs. grades. It also carries a risk for junior faculty whose tenure decision may depend on student evaluations.
