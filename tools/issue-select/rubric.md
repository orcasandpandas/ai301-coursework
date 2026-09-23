# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| active-maintainer | `repo-facts` block: repository owner activity and contributor activity dates | The repository owner has documented activity within the past 90 days, or at least one repository contributor has documented activity within the past 30 days. | required |
| used-repo | Check `repo-facts` for `latest release`, `last push to any branch`, star count on top of the repo page and check the repo line for an archive tag  | For this check, the latest release must be within the last 180 days while the last push to any branch should be within the last 90 days, and the star count must be  at least 5. | preferred |
| bounded-scope | The issue body and thread | The issue must NOT be an umbrella issue (a list of sub-items meant to be split into several separate tasks), nor can it be a pure usage question such as "how do I run this".  If there is discussion on the software design, this check can still pass if it's shown that a maintainer resolved it.  Either of these following conditions must be met: The issue should be smaller in scope with a limited number of impacted files and should be solvable without knowledge of the full repository's structure, or the issue should detail what files need to be changed and specify what may need to be added. Factors such as the opener of the issue being a maintainer or labels such as `good-first-issue` should allow for more leniency for this check. Even if all previous conditions are met, this check could fail if there is an extensive history of abandoned attempts by multiple contributors over several years| required |
| unclaimed | Issue comments and dates, Assignees box, linked PRs, and relevant claim/development labels | The issue must have no current evidence that another contributor is actively working on it and/or copmleted it. Fail if there is an assignee with recent activity, an open linked PR addressing the issue, or a recent comment explicitly stating that someone is working on or taking the issue. A claim or work signal that is more than 90 days old may be treated as stale unless there is newer evidence of continued work. Labels such as `up-for-grabs` or `help-wanted` do not by themselves establish that an issue is claimed. | required || contribution-policy | The `Contribution Policy` line under repo facts | This check only fails if the policy explicitly forbids AI-assisted work | required |


## Verdict rule

<!-- State how the grades above combine into accept or reject, and how
unclear is treated. Example shape (write your own): "accept if every
required check passes; preferred checks never change the verdict, they
rank accepted issues; unclear counts as fail." -->

Accept if every required check passes; any check that is unclear will be counted as a fail, and preferred checks will not impact the outcome but will affect the ranking; an issue where the preferred issue is met alongside all other issues will be ranked higher and will be marked as a `clear-accept`.