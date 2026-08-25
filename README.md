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

## How to use this

These are skills for Claude, not a command-line tool. There is nothing to
install and nothing to import — you describe the work and the matching skill
fires on its own.

**In Claude Code or Cowork**, once the skills are on your machine:

```bash
bash ~/Desktop/agent/_setup/sync-skills.sh
```

That clones every agent repository and links its `skills/` into `~/.claude/skills`,
so they are available in every session and every folder. Re-run it whenever one of
these repositories ships something new — it pulls rather than re-clones.

Then simply ask. Each skill's `description` frontmatter is written to match how
the request actually gets phrased, in English or Turkish, so you do not name the
skill and generally should not have to think about which one applies.

**If nothing fires**, that is a defect in the skill rather than in how you
asked. The description was written for the wrong phrasing. Say what you asked
and what you expected, and it gets fixed — that feedback is more valuable than
working around it.

**What is actually built** is listed under Contents below and in the Done
section of [BACKLOG.md](BACKLOG.md). Everything under Queue is planned and does
not exist yet.

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

`agents/` and `examples/` are empty so far.

## Roadmap

See [BACKLOG.md](BACKLOG.md). The first unchecked item is the one being built.

## Contents

| Skill | What it does |
| --- | --- |
| [basvuru-takip](skills/basvuru-takip) | Track job and internship applications in one file: what was sent when, what came back, and who is owed a follow-up. |
| [cv-uyarla](skills/cv-uyarla) | Adapt a CV to a specific posting against the posting's own wording, without inventing experience. |
| [mulakat-hazirlik](skills/mulakat-hazirlik) | Prepare for a named interview: the questions that role actually asks, and the answers evidenced from your own history. |

These arrived already written and in daily use, rather than being built against the queue below — which is why most carry no item number. Some have Turkish bodies: they were written in the language they are used in, and translating them is a queue item rather than a blocker.

Everything still under Queue in [BACKLOG.md](BACKLOG.md) does not exist
yet.
## Licence

MIT. See [LICENSE](LICENSE).
