---
name: "basvuru-takip"
description: "İş ve staj başvurularını tek dosyada takip eder — yeni başvuru ekler, durumları günceller, hangisine ne zaman dönüş yapılması gerektiğini söyler. \"Başvuru ekle\", \"başvurularım ne durumda\", \"şu şirkete başvurdum\", \"kimden dönüş bekliyorum\", \"takip maili atmalı mıyım\" dendiğinde kullan. Also triggers on \"add an application\", \"where do my applications stand\", \"I applied to this company\", \"who still owes me a reply\", \"should I send a follow-up\". CV'yi ilana göre uyarlamak için cv-uyarla, mülakat hazırlığı için mulakat-hazirlik kullan."
---

# Tracking applications

One source of truth: `kariyer/basvurular.md`. Create it if it does not exist.

## Table format
```
| Company | Role | Channel | Applied | Status | Last contact | Next step | Note |
```
**Status** is one of: `gonderildi` · `okundu` · `gorusme` · `teklif` · `red` ·
`sessiz` · `vazgectim`

Under each row, write the link to the posting and the contact person if there is
one.

## When adding a new application
If a posting link is given, **read it**: pull out the role, the company, the
closing date and the qualifications sought. Do not ask the user for these; take
them from the posting. If you cannot reach it, say so.

Add the row and **put a date** in the `Next step` column — seven working days
out is the default for a follow-up.

## When asked "where do things stand"
Do not dump the raw table. Produce this:

```
## Waiting on action (N)
- Company — Role — what to do — how many days it has been waiting

## Movement
- (anything whose status changed in the last 7 days)

## Silent  (14+ days with no reply)
- Company — send a follow-up?

## Summary
X active · Y interviewing · Z closed
```

## The follow-up email
Draft one for anything in `sessiz`:
- Four to six sentences, one question
- Show renewed interest without a pleading tone
- Add something concrete: a new project, a relevant development
- **Do not send it. Show the draft.**

## Rules
- Write dates as `YYYY-MM-DD`. Not "last week".
- Do not delete rejections; mark them `red` — seeing which kind of role produced
  which outcome reveals a pattern over time.
- If three or more rejections arrive at the same stage (always at the technical
  interview, say), point that out; a pattern is not a coincidence.
