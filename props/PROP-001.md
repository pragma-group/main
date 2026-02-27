```
PROP: 001
Title: Agentic Condensation Rule
Author: Vinnie Falco <vinnie.falco@gmail.com>
Status: Draft
Type: Process
Created: 2026-02-27
Target: new
```

## Abstract

The chair applies an agentic condensation rule to PROP submissions. The rule merges redundancy, preserves every material point, rewrites in Dimov style. The original is retained alongside the condensed form.

## Motivation

Overspecification - saying one thing twice - creates three failure modes:

- Redundant paragraphs couple implicitly. Update one; the other contradicts.
- AI retrieval degrades when noise competes with signal.
- A principle stated three ways invites three interpretations.

pragma-once.md protects against doing two things. This rule protects against saying one thing twice.

## Specification

The chair applies the condensation rule to each PROP submission. The condensed form is presented to the group. The original is retained.

If any member believes substance was lost, the member identifies the material point the condensed form omits. The chair restores it. The dispute is resolvable by comparison, not by argument.

## Rationale

**Why agentic.** A published rule is uniform and amendable. Human editorial judgment is subjective and creates friction.

**Why Dimov style.** Named for Peter Dimov. Every word earns its place. Short sentences. Plain structure. No filler. State the mechanism. Proven across Boost and WG21. Maximizes signal per sentence. Compatible with AI processing.

**Why preserve the original.** The original is the authoritative record. Nothing is suppressed.

**Why annotations.** A condensation without annotations is a black box.

**Why a PROP.** A chair preference dies with the chair. A PROP survives succession.

## Agentic Rule Listing

The following is the complete, self-contained condensation rule. Copy it into a rule file or paste it directly into an AI prompt along with the PROP submission.

---

**PRAGMA Condensation Rule**

You are given a PROP submission in Markdown format. Produce a condensed form by applying the following steps in order.

**Step 1. Extract material points.** Read the submission. Identify every distinct claim, proposal, or requirement. A material point is a sentence or clause that introduces information not present in other material points within the same document or in existing PRAGMA documents (pragma.md, pragma-once.md, pragma-next.md, adopted PROPs).

**Step 2. Identify redundancy.** Flag every sentence that restates a material point already captured, or restates content from existing PRAGMA documents.

**Step 3. Merge.** Remove redundant restatements. Each material point appears exactly once.

**Step 4. Rewrite in Dimov style.** Render each material point with these constraints:

- Every word earns its place.
- Short sentences. Plain structure.
- No filler, no hedging, no decoration.
- State the mechanism. Do not editorialize.
- No "our". No "should". (Lakos Principle)

**Step 5. Preserve structure.** Keep the PROP format: preamble and four required sections (Abstract, Motivation, Specification, Rationale). Do not modify preamble fields. Do not modify section headings.

**Step 6. Annotate merges.** Where redundant material was collapsed, add a brief inline annotation in square brackets citing what was merged. Example: `[merged: restated constraint from pragma-once.md Section 7]`

**Constraints:**

- Do not remove any material point. The operation is lossless in substance, lossy only in restatement.
- Do not add claims not present in the original.
- If the original contains no redundancy, return it unchanged.

**Output:** The condensed form only. The original is preserved separately by the chair.

---
