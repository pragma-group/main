```
PROP: 002
Title: Commit Message Questions
Author: Vinnie Falco <vinnie.falco@gmail.com>
Status: Draft
Type: Process
Created: 2026-02-27
Target: new
```

## Abstract

Every commit message answers five questions. The diff records what changed. The answers record what the diff cannot.

## Motivation

A commit message that restates the diff adds nothing. The only non-trivial content is what the committer knows that the diff does not contain: the trigger, the driver, the rationale, the rejected alternatives, the invisible context.

Layer 0 value 6.4: "Knowledge transmission over knowledge hoarding."

## Specification

The committer answers these questions. "N/A" with a brief reason if a question does not apply.

**1. What triggered this change?**

**2. Who drove it?**

**3. Why this approach?**

**4. What was considered and not done?**

**5. What context is not visible in the diff?**

Format:

```
<summary, under 72 characters>

Triggered by:
Driven by:
Rationale:
Considered:
Context:
Keywords: <human-supplied: topics, documents, members, PROPs>
Tags: <AI-generated: see Agentic Rule Listing>
```

## Rationale

**Why questions, not fields.** A question invites a sentence. A field label invites a word.

**Why "considered and not done."** Rejected alternatives decay fastest. The decision survives in the artifact. The alternatives survive nowhere unless recorded here.

**Why "context not visible in the diff."** By definition, not recoverable from any other source.

**Why N/A.** Friction degrades compliance. "N/A" is an answer. Silence is not.

**Why a PROP.** Conventions decay. Questions survive succession.

## Agentic Rule Listing

Generates the Tags line from the diff and the human answers. Tags are retrieval tokens for `git log --grep` and tooling. Cheaper than parsing the diff.

---

**PRAGMA Commit Tag Rule**

Given a git diff and the human-written fields (Triggered by, Driven by, Rationale, Considered, Context, Keywords):

1. Extract from the diff: file paths, section headings, PROP numbers, member names, document sections cited.
2. Extract from the human answers: proper nouns, PROP numbers, document names, concept names.
3. Deduplicate against the human-supplied Keywords.
4. Emit: `Tags: <comma-separated, alphabetical>`.

Do not fabricate tags. Every tag traces to the diff or the human answers.

---
