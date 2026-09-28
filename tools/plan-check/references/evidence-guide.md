# Evidence guide: where proof lives in a reproduction package

<!--
THIS IS THE PART YOU WRITE (new this week: Unit 1 handed you this file
finished; the scaffolding fades). The skill uses this guide as its map:
for every kind of proof a rubric check names, this file says WHERE to
find it in a package and WHAT GOOD LOOKS LIKE when you do.

Under each family heading below, write:

- Where it lives: the exact places to look. In an eval bundle (which
  section of the package: the issue context, the repo-facts block, the
  claim comment, the repro report and its parts). In live mode (where
  on GitHub or in the draft: the issue thread, the repo's docs, the
  student's draft comment).
- What good looks like: one or two sentences someone else could apply.
  Prefer observable conditions ("the versions named match what the
  issue targets, or the difference is called out") over adjectives
  ("environment is thorough").

A rubric check whose evidence this guide cannot locate is a check
nobody else can execute; the rubric swap showed you what that feels
like. Write the map you wish your grader had.
-->

## Environment

<!-- Where the environment record lives, and what a sufficient one
looks like against the issue's stated target. -->
The environment record lives in the repro report's environment section.  A good environment section states the name of the tool (which can be compared with the name listed in the README file of the repository), the version of the tool that is being tested, the version of the operating system being used for testing and the specific commit you are working off of.  You can check repo-facts to see the version of the issue being tested and ensure it matches the reproduction environment.  If the version of the tool in `repo-facts` does not match the version of the tool used in the reproduction environment, this should be explicitly called out.



## Steps

<!-- Where the reproduction steps live, and what makes them followable
by a stranger, starting state to trigger. -->
The reproduction steps live in the repo report and broadly showcase two stages: preparation and execution.  The preparation describes what steps are needed to go from a clean environment to the specific conditions that the reproduction occured under (so it should include how the software was downloaded, how it was activated and what changes may have been made to its configuration).  The execution should then be a step by step guide on how we go from starting the software to ending up at the error, with every command fully documented.  Minimal guesswork should be required so someone else could reproduce the bug through reading the sequence of steps provided. 

## Behavior shown

<!-- Where the artifacts live (output excerpts, logs, screenshots),
and what it means for an artifact to show the issue's behavior rather
than an adjacent one. -->
Arifacts of the reported behavior being described lives in the issue context, while artifacts of the reproduced behavior live in the repro report.  Compare the artifacts in the reproduction report with the issue context to ensure they showcase similar behavior, such as showing the same errors in the log outputs and/or same unexpected results.  

## Honesty

<!-- Where claims and their backing meet: how to tell a report that
says exactly what happened (including an honest cannot-reproduce) from
one that claims more than its evidence shows. -->
The claims made in the repro report should be supported by the documented
environment, preparation, execution, and observed behavior. A report should
only claim that the issue was reproduced when the evidence shows the reported
behavior occurred under the documented conditions. If the reported behavior
cannot be reproduced, the report should state that honestly rather than
claiming a successful reproduction.

## Comms

<!-- Where the words meet the repo: the claim comment against the
issue, the comments against the repo's stated templates and
contribution policy (including AI-use disclosure requirements), and
what specific-and-honest looks like next to boilerplate. -->
The claim and reproduction comments live in the issue thread, or in the
student's draft comments during live mode. Check the repository's contribution
policy and stated comment templates for any required content or disclosures.
A good claim comment identifies the specific issue and what the student plans
to investigate without claiming results that have not yet occurred. A good
reproduction comment clearly states what was observed and includes any
required AI-use disclosure. Comments should provide specific information
relevant to the issue rather than relying on generic or boilerplate wording.