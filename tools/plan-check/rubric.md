# Rubric: is this reproduction package ready to post?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever
checks you define here. It ships empty on purpose: the judgment is your
work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four
   columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where in the package. Name
     the part (the claim comment, the repro report's environment
     record, the artifacts read against the issue's description, the
     repo-facts block) or a location from your
     references/evidence-guide.md. "The report" is not a source; "the
     output excerpt read against the error the issue describes" is.
   - Pass condition: a decision rule about the OUTCOME that someone
     else could apply and get your answer. Judge the thing itself (does
     the artifact show the issue's behavior?), never the write-up's
     shape (how many steps it has, how long it is, whether it uses a
     template's headings). Structure-shaped checks are what make
     graders disagree with themselves.
   - Weight: `required` (a fail here holds the package) or `preferred`
     (never changes the verdict).

2. A verdict rule below the table: how the check grades combine into
   accept (ready) or reject (hold), including how `unclear` is
   treated. The verdict space is binary. If you write no rule for
   `unclear`, the skill treats it as fail.

Cover what actually gets bad packages posted. The lecture named the
proof families: the environment is recorded, the steps are complete
and followable, the behavior shown matches the issue (not an adjacent
one), the outcome is stated honestly (an evidenced cannot-reproduce is
a pass, a confident wrong-target is not), and the words respect the
repo's conventions. A rubric that ignores a family will fail eval
packages designed around that family.
-->

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
|env-recorded|The environment line for the repro report|The environment line for the repro report must include the operating system used for the repro, the version of the tool being used, and the specific commit being tested|Required|
|steps-followable|The body for the repro report|The environment should identify the tool or software being tested and the version and operating system used for the reproduction. When a specific commit is relevant to the issue or reproduction, the commit being tested should also be identified or any difference should be called out.|Required|
|behavior-matches|The reproduction steps should provide enough detail for another person to repeat the setup and trigger the reported behavior without guessing. They should include the relevant setup commands, dependencies, configuration changes, inputs, and software commands needed for this particular reproduction. Details that do not apply to the issue do not need to be included.|Required|
|claim-specific|Repro candidate claim comment|The claim must identify the specific issue being claimed and clearly state what the contributor intends to do next. It must not claim that the issue has already been reproduced or understood when the claim is being made before reproduction.|Required|
|conventions|The candidate claim/repro comments and the repository's contribution policy in repo-facts|The comments must follow any communication or AI-use disclosure requirements stated by the repository's contribution policy. If the policy requires disclosure of AI assistance, the relevant comment must contain that disclosure.|Required|

## Verdict rule

<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict;
unclear counts as fail." -->
All of the listed checks are required for this program to pass, as they are all vital to ensuring the reproduction report has full integrity and accuracy