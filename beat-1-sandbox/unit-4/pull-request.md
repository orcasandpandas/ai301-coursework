# Unit 4 — Test and Submit

Path: `beat-1-sandbox/unit-4/pull-request.md`

Record of the pull request you opened against the Path Review repo, and of the evaluation
runs that produced `eval-run.txt`. This file is graded at the path above; a copy kept
anywhere else in the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the wrong
label is not graded.

---

## Your pull request

**Pull request**

[Link to the pull request you opened. It must be the pull request's own page on the Path
Review repo, not your fork's branch page.]

**Branch**

[The name of the branch the pull request comes from, exactly as it appears in your fork.
The naming shape is a type prefix, then the issue number, then a short description. **The
issue number in the branch name must be the number of the issue the pull request fixes** —
a name carrying any other number does not satisfy this field.]

## Eval iterations

Answer all four sections. Quote source text directly; paraphrase does not satisfy these
fields.

**Run history**

[The agreement score of each run you did, in order. A single run is a complete answer if
only one run occurred. **The last score in your list must match the agreement line in the
`eval-run.txt` you committed** — that file is the record of your final run.]
I got a score of 18/20 on my first run

**Package analysis**

[Pick one scored package (`pkg-01` through `pkg-20` — the four `calib-` packages are never
scored). Name it by id, say what your rubric decided and what the gold label said, and
explain why your rubric read it that way.]
I decided to look at pkg-18, as the gold label said it would be rejected and unreviewable while my rubric accepted it.  Looking at my rubric's unreviewable section, it likely missed this one because the only flaw in this PR was a single line of code that was commented out, with the rest of the file following the rubric.  My rubric says to "Fail if unrelated changes, temporary artifacts, or other unexplained modifications materially obscure the intended work or prevent meaningful review." and I believe that technically this one line may have been seen as not significant enough to prevent review or obscure the intended work.
**Check rationale**

[Quote one check from the `rubric.md` you uploaded to `tools/pr-precheck/`, exactly as it reads now.
Then say why it reads that way — what you revised to get there, or what you rejected in
favour of it.]
> | not tested | The test evidence read against the plan's test plan, the changed behavior in the diff, and any relevant repository checks identified in repo-facts | The evidence provides observable support that the changed behavior works as intended and addresses the relevant problem. Relevant repository checks should be run. If a check cannot be run, the limitation and its reason must be disclosed, and the remaining evidence must still provide a reasonable basis for review. Fail when there is no meaningful evidence of behavior or required checks are skipped without adequate explanation.
The reason this check asks for repository checks more broadly rather than a more specific one asking for procedures is because I found that often, asking for steps would exclude tests that may have been done outside of the CLI, and added the possibility of passing of an explanation for a lack of a check was added.

**Trade-offs**

[Every check gives something up. Any one of these is a complete answer: a package whose
result it changes, a canary you re-ran with `--only`, a case you accept it will miss, or a
stated reason nothing changed elsewhere. "Nothing changed, and here is how I know" earns
the point in full when the reason follows.]
I accepted that this check would miss with pkg-02 and other such packages where the description disclosed why testing couldn't be done because defining a reasonable basis is difficult, and I think it's better to have a false negative due to difficulty detecting the reason for lack of testing than to have a false positive.

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/pr-precheck/`.
