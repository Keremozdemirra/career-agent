# career-agent

Agents and skills for applications, interviews and the decisions around them.

Job applications reward specificity and almost everything about the
process pushes towards generality — the CV rewritten to fit every posting, the
cover letter that could be sent anywhere, the interview answer that describes a
role rather than a decision.

This repository holds the agents and skills for the specific version: a CV
tailored to what a particular posting is actually screening for, preparation
built around the decisions you actually made, and the parts nobody prepares for
because they feel like formalities.

## What this is not

It does not invent experience. A skill here that improves a CV by
adding something that did not happen has failed, and the check for that is
explicit in each one.

It does not apply on anyone's behalf or send anything.

It does not know what any particular company wants. It works from what the
posting says and what can be found, and marks the rest as inference.

## Layout

```
agents/
  <name>.md           one specialist, its brief and its boundaries
skills/
  <name>/
    SKILL.md          the instruction, with triggering description frontmatter
    scripts/          only where deterministic code beats instruction
examples/
  <name>/             worked example on real input, with the output committed
```

## Roadmap

See [BACKLOG.md](BACKLOG.md). The first unchecked item is the one being built.

## Planned contents

Nothing here is built yet. This table is the intended shape, and the daily loop
fills it in one item at a time.

| # | Skill | What it does |
| --- | --- | --- |
| 001 | [read-the-posting](skills/read-the-posting) | Work out what a posting is actually screening for, separating the requirements from the boilerplate and the negotiable from the hard filters. |
| 002 | [tailor-the-cv](skills/tailor-the-cv) | Reorder and re-emphasise real experience against a specific posting, with a hard rule against adding anything that did not happen and a check that enforces it. |
| 003 | [evidence-bank](skills/evidence-bank) | Build the reusable store of what you actually did — the decision, the constraint, the outcome, the number — so tailoring is selection rather than invention. |
| 004 | [cover-letter-that-is-not-generic](skills/cover-letter-that-is-not-generic) | Write the letter that could only have been sent to this employer, and the test that proves it. |
| 005 | [interview-prep](skills/interview-prep) | Prepare around the decisions you made rather than the roles you held, including the questions that are actually being asked underneath the ones asked out loud. |
| 006 | [technical-case-prep](skills/technical-case-prep) | Work through the case formats that appear in consulting and finance interviews, with the reasoning made visible rather than the answer memorised. |
| 007 | [questions-to-ask](skills/questions-to-ask) | The questions that tell you whether to accept, as opposed to the ones that perform interest. |
| 008 | [offer-comparison](skills/offer-comparison) | Compare offers on what actually differs — trajectory, autonomy, what you will be doing on a Tuesday — with compensation as one input rather than the frame. |
| 009 | [application-tracker](skills/application-tracker) | Track what was sent where, what stage each is at, and what follow-up is due, so the pipeline is visible rather than remembered. |

## Licence

MIT. See [LICENSE](LICENSE).
