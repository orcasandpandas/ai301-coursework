# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in
the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

[The individual Path Review issue page. A link to the repository or the issue list
does not satisfy this field.]

**Verdict output**

[Your skill's live-mode output for this issue, pasted verbatim and ending with the
fenced JSON verdict block. A summary does not satisfy this field.]

**The verdict must record `accept` for this issue.** Choose an issue your own skill
accepts. If your skill rejects every candidate you try, that is a signal about your
rubric rather than about the issues: revise it and re-run — retries are unlimited and a
partial re-run costs about $0.20 — or run the skill on different candidates. Output
recording `reject` for the issue you chose earns no credit for this field.

```
paste the output here, including the closing JSON block
```

---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

agreement: 7/13 scored items
7 item(s) errored; fix and re-run.
-------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-02  reject  reject   yes
issue-03  reject  reject   yes
issue-04  accept  reject   NO     failed: bounded-scope
issue-05  reject  reject   yes
issue-06  accept  reject   NO     failed: bounded-scope, used-repo (preferred)
issue-07  reject  reject   yes
issue-08  reject  reject   yes
issue-09  accept  reject   NO     failed: bounded-scope, unclaimed
issue-10  reject  reject   yes
issue-11  accept  reject   NO     failed: used-repo (preferred), bounded-scope
issue-12  reject  reject   yes
issue-13  reject  reject   yes
issue-14  accept  reject   NO     failed: bounded-scope
issue-15  reject  reject   yes
issue-16  accept  reject   NO     failed: bounded-scope
issue-17  reject  reject   yes
issue-18  reject  reject   yes
issue-19  accept  reject   NO     failed: used-repo (preferred), bounded-scope
issue-20  reject  reject   yes
```
categories: claimed 4/4  clear-accept 0/8  dead-repo 3/3  policy 1/1  scope 4/4
agreement: 12/20 scored items  (bar: 18/20: below the bar; category floor unmet: no match in clear-accept)
-------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-02  reject  reject   yes
issue-03  reject  reject   yes
issue-04  accept  accept   yes
issue-05  reject  reject   yes
issue-06  accept  accept   yes
issue-07  reject  reject   yes
issue-08  reject  reject   yes
issue-09  accept  reject   NO     failed: unclaimed
issue-10  reject  reject   yes
issue-11  accept  accept   yes
issue-12  reject  reject   yes
issue-13  reject  reject   yes
issue-14  accept  accept   yes
issue-15  reject  accept   NO     graded accept
issue-16  accept  accept   yes
issue-17  reject  reject   yes
issue-18  reject  reject   yes
issue-19  accept  reject   NO     failed: bounded-scope
issue-20  reject  reject   yes
```
categories: claimed 4/4  clear-accept 5/8  dead-repo 3/3  policy 1/1  scope 3/4
agreement: 16/20 scored items  (bar: 18/20: below the bar)
--------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope, unclaimed
issue-02  reject  reject   yes
issue-03  reject  reject   yes
issue-04  accept  reject   NO     failed: bounded-scope, unclaimed
issue-05  reject  reject   yes
issue-06  accept  reject   NO     failed: used-repo (preferred), unclaimed
issue-07  reject  reject   yes
issue-08  reject  reject   yes
issue-09  accept  accept   yes
issue-10  reject  reject   yes
issue-11  accept  reject   NO     failed: unclaimed
issue-12  reject  accept   NO     graded accept
issue-13  reject  reject   yes
issue-14  accept  reject   NO     failed: unclaimed
issue-15  reject  reject   yes
issue-16  accept  reject   NO     failed: unclaimed
issue-17  reject  reject   yes
issue-18  reject  reject   yes
issue-19  accept  reject   NO     failed: bounded-scope, unclaimed
issue-20  reject  reject   yes
```
categories: claimed 4/4  clear-accept 1/8  dead-repo 3/3  policy 0/1  scope 4/4
agreement: 12/20 scored items  (bar: 18/20: below the bar; category floor unmet: no match in policy)
-----------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-02  reject  reject   yes
issue-03  reject  reject   yes
issue-04  accept  reject   NO     failed: bounded-scope
issue-05  reject  reject   yes
issue-06  accept  accept   yes
issue-07  reject  reject   yes
issue-08  reject  reject   yes
issue-09  accept  accept   yes
issue-10  reject  reject   yes
issue-11  accept  accept   yes
issue-12  reject  reject   yes
issue-13  reject  reject   yes
issue-14  accept  reject   NO     failed: bounded-scope
issue-15  reject  reject   yes
issue-16  accept  accept   yes
issue-17  reject  reject   yes
issue-18  reject  accept   NO     graded accept
issue-19  accept  reject   NO     failed: bounded-scope
issue-20  reject  reject   yes
```
categories: claimed 3/4  clear-accept 4/8  dead-repo 3/3  policy 1/1  scope 4/4
agreement: 15/20 scored items  (bar: 18/20: below the bar)
-------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-04  accept  accept   yes
issue-10  reject  reject   yes
issue-14  accept  accept   yes
```
agreement: 3/4 scored items
--------
```
  issue-14: accept
  issue-19: reject
  issue-01: reject
  issue-04: reject

item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-04  accept  reject   NO     failed: bounded-scope
issue-14  accept  accept   yes
issue-19  accept  reject   NO     failed: bounded-scope
```
agreement: 1/4 scored items
-------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-04  accept  accept   yes
issue-14  accept  accept   yes
issue-19  accept  reject   NO     failed: bounded-scope
```
agreement: 2/4 scored items
--------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-02  reject  reject   yes
issue-03  reject  reject   yes
issue-04  accept  accept   yes
issue-05  reject  reject   yes
issue-06  accept  accept   yes
issue-07  reject  reject   yes
issue-08  reject  reject   yes
issue-09  accept  accept   yes
issue-10  reject  reject   yes
issue-11  accept  accept   yes
issue-12  reject  accept   NO     graded accept
issue-13  reject  reject   yes
issue-14  accept  accept   yes
issue-15  reject  accept   NO     graded accept
issue-16  accept  accept   yes
issue-17  reject  reject   yes
issue-18  reject  accept   NO     graded accept
issue-19  accept  reject   NO     failed: bounded-scope
issue-20  reject  reject   yes
```
categories: claimed 3/4  clear-accept 6/8  dead-repo 3/3  policy 0/1  scope 3/4
agreement: 15/20 scored items  (bar: 18/20: below the bar; category floor unmet: no match in policy)
--------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-12  reject  reject   yes
issue-14  accept  accept   yes
issue-15  reject  accept   NO     graded accept
issue-18  reject  accept   NO     graded accept
issue-19  accept  reject   NO     failed: bounded-scope
```
agreement: 2/6 scored items
------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-12  reject  reject   yes
issue-14  accept  accept   yes
issue-15  reject  reject   yes
issue-18  reject  reject   yes
issue-19  accept  reject   NO     failed: bounded-scope
```
agreement: 4/6 scored items
------
```
item      gold    verdict  agree  note
issue-01  accept  reject   NO     failed: bounded-scope
issue-02  reject  reject   yes
issue-03  reject  reject   yes
issue-04  accept  accept   yes
issue-05  reject  reject   yes
issue-06  accept  accept   yes
issue-07  reject  reject   yes
issue-08  reject  reject   yes
issue-09  accept  accept   yes
issue-10  reject  reject   yes
issue-11  accept  accept   yes
issue-12  reject  reject   yes
issue-13  reject  reject   yes
issue-14  accept  accept   yes
issue-15  reject  reject   yes
issue-16  accept  accept   yes
issue-17  reject  reject   yes
issue-18  reject  reject   yes
issue-19  accept  reject   NO     failed: bounded-scope
issue-20  reject  reject   yes
```
categories: claimed 4/4  clear-accept 6/8  dead-repo 3/3  policy 1/1  scope 4/4
agreement: 18/20 scored items  (bar: 18/20: PASS)
--------
**Issue analysis**

```
item      gold    verdict  agree  note
issue-19  accept  reject   NO     failed: bounded-scope
```
My rubric's decision was that this issue should be rejected while the gold label said it was to be accepted.  The reasoning was that the scope was beyond what a beginner would be able to do.

**Check rationale**

`| bounded-scope | The issue body and thread | The issue must NOT be an umbrella issue (a list of sub-items meant to be split into several separate tasks), nor can it be a pure usage question such as "how do I run this".  If there is discussion on the software design, this check can still pass if it's shown that a maintainer resolved it.  Either of these following conditions must be met: The issue should be smaller in scope with a limited number of impacted files and should be solvable without knowledge of the full repository's structure, or the issue should detail what files need to be changed and specify what may need to be added. Factors such as the opener of the issue being a maintainer or labels such as `good-first-issue` should allow for more leniency for this check. Even if all previous conditions are met, this check could fail if there is an extensive history of abandoned attempts by multiple contributors over several years| required |`

Checking if a scope fits beginners was the most difficult part of this assignment for me, so I decided to partially think about what would make sense for me: I came to the basic conclusion of a focused problem with a defined solution, and from there came up with what consituted a focused issue along with what kinds of issues would be best for beginners (hence how I arrived at those that either were small in scope or explained the files in the issues).  I used some of the suggested evidence-guide.md rational, such as checking for multiple abandoned attempts which I thought made sense as a final check.  

**Trade-offs**

The quoted check did result in two false negatives with issue-01 and issue-19, and it is a little restrictive in some areas such as requiring generally what files may need to be changed, but I feel it acts as a good threshold to see what kinds of problems will almost certainly be suitable for beginners, and that removing those conditions would lead to more false positives, which I feel are more serious than false negatives.
---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.


**Selection rationale**
``
[Answer all three:

1. The issue's fit to your interests and to the time available.
I decided to select issue number 40 because I am interested in learning about front end UI and I feel its more comprehensible to someone who hasn't used the repo before.
2. What the verdict identified correctly, and what you weighed that the rubric could
   not.
The verdict did identify correctly that both issues generally passed as they had a defined scope and were open, but it could only account for what I wrote in my description to match which I may prefer more; everybody has a different preference for what they may want to work on at a moment in time which can't quite be expressed in a brief summary, and I preferred 40 over 69 despite the AI ranked 69 higher.
3. The anticipated difficulty in claiming it.
I think that this issue will have average to below average difficulty in claiming it as there are no comments on it asking to contribute and its a front-end issue.
---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
`Both candidates are in the scoped repo (codepath/pathreview-ai301-fa26-s3); issue 40 was listed twice, so I graded two unique candidates. Repo facts gathered live against today, 2026-09-23.

Shared repo facts: owner codepath, collaborator Aburke225 last commit 2026-09-16 (7 days ago) · last push 2026-09-16 · stars 5 · archived false · no releases at all · docs/CONTRIBUTING.md sets AI-relevant conditions (green CI, remove xfail markers, no bulk lint fixes) but states no AI ban · 0 pull requests in the repo, open or closed.

Ranked read-out

1. #69 — Output parser crashes on a top-level JSON array fallback — accept
- active-maintainer pass — collaborator Aburke225 committed 2026-09-16, 7 days ago (<30).
- used-repo fail (preferred, no verdict effect) — push recency and stars pass (2026-09-16; 5 stars) but the repo has no releases, so "latest release within 180 days" cannot be met.
- bounded-scope pass — one bug, two named files (rag/generator/output_parser.py, tests/unit/test_output_parser.py), 2–4h, good first issue + tier-1, opened by a COLLABORATOR; not an umbrella, not a usage question, no abandoned attempts.
- unclaimed pass — three claim comments (Yina-Mu 09-20, tonybuii2003 09-21, hanluu1 09-23) but all are author_association: NONE, i.e. classmates; the Path Review house rule says student claims don't block. No assignee, no linked PR, zero PRs in the repo.
- contribution-policy pass — CONTRIBUTING.md imposes conditions only, no AI prohibition.

Fit: Victor's ground is Python and ML tooling, and this is a Python bug in the RAG generator's output parser. It ships its own oracle — the covering test is @pytest.mark.xfail under manifest id H-02, so the fix is verified by the test flipping, not by judgment. That directly serves the "avoid hallucinations, make sure the program has the full required context" goal: two files, an exact error (AttributeError: 'list' object has no attribute 'items'), and a pass/fail check.

2. #40 — Add a "Copy link" button to share a public review summary — accept
- active-maintainer pass — same evidence, commit 2026-09-16.
- used-repo fail (preferred) — no releases.
- bounded-scope pass — meets the rubric's second branch: the body names the files to change (ReviewPage.tsx, shareService.ts, api/routes/reviews.py) and specifies what to add (shareable link, login-free read-only view, 30-day expiry); opener is a COLLABORATOR, which the rubric says earns leniency; no umbrella list, no abandoned attempts. Tension worth noting: at 5–8h and tier-2, spanning React plus a new unauthenticated expiring-token API route, this is a feature, not a small fix — it passes only because the rubric's "names the files and says what to add" branch is satisfied. If you don't want that branch to carry issues this size, that's a rubric edit, not a grading one.
- unclaimed pass — no comments, no assignees, no linked PRs.
- contribution-policy pass — no AI ban.

Neither is a clear-accept: the preferred used-repo check fails for both, because the repo publishes no releases.

[
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/69",
    "checks": [
      {"name": "active-maintainer", "grade": "pass", "evidence": "Collaborator Aburke225 committed to main on 2026-09-16, 7 days before today (2026-09-23), within the 30-day contributor window."},
      {"name": "used-repo", "grade": "fail", "evidence": "GET /releases/latest returns none, so the 180-day release condition fails; push 2026-09-16 and 5 stars would otherwise pass, archived: false."},
      {"name": "bounded-scope", "grade": "pass", "evidence": "Two named files, 2-4h estimate, 'good first issue' + 'tier-1' labels, opened by a COLLABORATOR; concrete AttributeError, no umbrella list, no prior attempts."},
      {"name": "unclaimed", "grade": "pass", "evidence": "No assignee, no linked PR, zero PRs in the repo; the three claim comments are all author_association NONE (classmates), which the Path Review house rule says do not block."},
      {"name": "contribution-policy", "grade": "pass", "evidence": "docs/CONTRIBUTING.md sets conditions (green CI, remove xfail markers) and states no prohibition on AI-assisted work."}
    ],
    "verdict": "accept"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/40",
    "checks": [
      {"name": "active-maintainer", "grade": "pass", "evidence": "Collaborator Aburke225 committed to main on 2026-09-16, 7 days before today (2026-09-23), within the 30-day contributor window."},
      {"name": "used-repo", "grade": "fail", "evidence": "GET /releases/latest returns none, so the 180-day release condition fails; push 2026-09-16 and 5 stars would otherwise pass, archived: false."},
      {"name": "bounded-scope", "grade": "pass", "evidence": "Body names the three files to change and what to add (shareable link, read-only view, 30-day expiry) and the opener is a COLLABORATOR; passes the rubric's 'details the files' branch despite the 5-8h tier-2 size."},
      {"name": "unclaimed", "grade": "pass", "evidence": "Zero comments, no assignees, timeline shows only three label events from 2026-09-10, and the repo has no pull requests at all."},
      {"name": "contribution-policy", "grade": "pass", "evidence": "docs/CONTRIBUTING.md sets conditions (green CI, remove xfail markers) and states no prohibition on AI-assisted work."}
    ],
    "verdict": "accept"
  }
]`
