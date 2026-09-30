# Unit 2 — Claim and Reproduce

Path: `beat-1-sandbox/unit-2/reproduction.md`

Record of your claim and reproduction on the issue you chose in Unit 1, and of the
evaluation runs that produced `eval-run.txt`. This file is graded at the path above; a copy
kept anywhere else in the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the wrong
label is not graded.

---

## Your identity upstream

**GitHub username**

orcasandpandas
---

## Posted upstream

**Claim comment**

[Link to the comment where you claimed the issue. Use the comment's own permalink, not the
issue page on its own. **Then paste the text of that comment underneath the link** — the
pasted text is what this field is graded on, so copy across what you actually posted.]

**Reproduction comment**

[Link to the comment where you posted your reproduction. It must record the environment
(OS, relevant versions, code state), steps a stranger could follow, and what you observed.
**Then paste the text of that comment underneath the link** — the pasted text is what this
field is graded on, so copy across what you actually posted.]

## Eval iterations

Answer all four sections. Quote source text directly; paraphrase does not satisfy these
fields.

**Run history**
```
item    gold    verdict  agree  note
pkg-01  accept  reject   NO     failed: claim-specific
pkg-02  reject  reject   yes    
pkg-03  accept  accept   yes    
pkg-04  reject  reject   yes    
pkg-05  accept  reject   NO     failed: env-recorded
pkg-06  reject  reject   yes    
pkg-07  accept  reject   NO     failed: env-recorded
pkg-08  reject  reject   yes    
pkg-09  accept  accept   yes    
pkg-10  accept  reject   NO     failed: env-recorded
pkg-11  accept  reject   NO     failed: env-recorded
pkg-12  accept  reject   NO     failed: env-recorded
pkg-13  reject  reject   yes    
pkg-14  reject  reject   yes    
pkg-15  reject  reject   yes    
pkg-16  reject  reject   yes    
pkg-17  reject  reject   yes    
pkg-18  reject  reject   yes    
pkg-19  reject  reject   yes    
pkg-20  reject  reject   yes    
```


```
item    gold    verdict  agree  note
pkg-01  accept  accept   yes    
pkg-02  reject  reject   yes    
pkg-03  accept  accept   yes    
pkg-04  reject  reject   yes    
pkg-05  accept  accept   yes    
pkg-06  reject  reject   yes    
pkg-07  accept  reject   NO     failed: env-recorded
pkg-08  reject  reject   yes    
pkg-09  accept  accept   yes    
pkg-10  accept  accept   yes    
pkg-11  accept  accept   yes    
pkg-12  accept  accept   yes    
pkg-13  reject  reject   yes    
pkg-14  reject  reject   yes    
pkg-15  reject  reject   yes    
pkg-16  reject  reject   yes    
pkg-17  reject  reject   yes    
pkg-18  reject  reject   yes    
pkg-19  reject  reject   yes    
pkg-20  reject  reject   yes    
```

categories: clear-accept 7/8  disclosure 1/1  no-evidence 4/4  unfollowable-comms 3/3  wrong-target 4/4
agreement: 19/20 scored items  (bar: 18/20: PASS)


**Package analysis**

pkg-10 I felt was an interesting one because it forced me to reconsider my rule for behavior-matches; originally, it only checked if both the Issue and repro showcased similar behavior, but I found pkg-10 showed different behavior yet also specified the behavior was unreproducible, giving it an accept according to gold.  From this, I added a stipulation to my behavior-matches check that it could still pass if the behavior doesn't match as long as this is explicitly communicated, allowing me to get pkg-10 correct on the final run.

**Check rationale**

`The reproduction steps should provide enough detail for another person to repeat the setup and trigger the reported behavior without guessing. They should include the relevant setup commands, dependencies, configuration changes, and inputs needed for this particular reproduction. Details that do not apply to the issue do not need to be included, so for example a system-level issue would not need to specify installation.`
Originally, this check looked for a sequence of steps showing installation, setup, configuration, and execution.  I wanted to think about what would be needed for someone to go to a new system to running the software and came up with this sequence.  However, I found that some issues involved packages that already existed on the PC or involved browser frameworks and decided to remove the step involving installation.  I kept the specifications asking for configuration and setup to be included, as I feel those are relatively universal actions when working with any software.

**Trade-offs**

When I first ran my checks, I got many errors from false negatives with an overly strict environment, so I altered it to look for tool version and OS at the bare minimum.  I was having a similar issue with too many false negatives while checking steps followed as I failed to account for problems related to software that didn't need to be installed, and made it check for the minimum of setup, configuration, dependencies and inputs.  I think these both establish a solid baseline that's relatively universal no matter the format of the software, and going any further seems to result in many false negatives.

---



Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/repro-check/`.
