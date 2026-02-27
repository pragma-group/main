# Mitigating Overspecification

Overspecification is scope creep applied to depth. This document identifies the risk and proposes a workflow.

---

## 1. THE THESIS

pragma-once.md protects against doing two things. This document protects against saying one thing twice.

A group of thorough practitioners will produce thorough documents. Thoroughness that adds signal is valuable. Restatement that restates settled points is not thoroughness. It is overspecification: redundant depth that dilutes the document it inhabits.

Overspecification is not a character flaw. It is a systemic risk. Any group that values completeness will produce it. The question is not whether it appears but whether the process detects it.

---

## 2. WHAT OVERSPECIFICATION IS

Three forms:

- **Redundant restatement.** The same claim expressed in different words within the same document. Each restatement creates an implicit dependency on every other. Update one, and the others contradict it.

- **Exhaustive elaboration of settled points.** A principle that has been adopted does not need re-derivation in every document that references it. A citation suffices.

- **Restating existing documents.** A PROP that repeats what pragma-once.md already says adds no information. It adds a second location for the same information, which is a maintenance liability.

The test is functional: does this sentence introduce information not present elsewhere in the document or its references? If not, it is a candidate for removal.

Overspecification is not the same as thoroughness. Thoroughness covers necessary ground. Overspecification covers the same ground twice.

---

## 3. WHY IT MATTERS

**Contradiction.** Two paragraphs that say the same thing will eventually say different things. One gets updated. The other does not. The document now contains a contradiction. Contradictions in institutional documents are silent failures - they produce wrong behavior without raising an error.

**AI degradation.** PRAGMA artifacts are processed by AI tooling. AI retrieval accuracy degrades when noise competes with signal. Context windows that fill with restated content leave less room for novel content. Overspecified documents produce worse AI output than concise documents containing the same information.

**Interpretive divergence.** A principle stated three ways invites three interpretations. Each reader latches onto the phrasing closest to the reading they prefer. A principle stated once, precisely, constrains interpretation to one reading.

---

## 4. THE WORKFLOW

When a PROP is submitted, the chair applies the agentic condensation rule before presenting it to the group.

1. Author submits a PROP. Any length. Any style.
2. The chair applies the condensation rule (PROP-001).
3. The rule merges redundancy, extracts material points, rewrites into Dimov style.
4. The original submission is preserved alongside the condensed form.
5. The chair presents the condensed form to the group for discussion.

If the submission contains multiple independent proposals, the chair asks the author to break it into separate PROPs. This is not a new rule. The chair already has authority over output standards under pragma-once.md Section 7.

No author is asked to write differently. The input channel accepts everything. The process handles compression.

**Rule.** The workflow adds a tool to the chair's process. It does not add a constraint to the author's.

---

## 5. THE AGENTIC RULE

The condensation rule is itself a PROP: PROP-001. It goes through PROP-000's consensus process. The group adopts it.

What the rule specifies:

- Merge redundant restatements into single assertions
- Preserve every material point - nothing is discarded
- Rewrite in Dimov style: every word earns its place, short sentences, plain structure, no filler, no hedging, no decoration
- Flag claims that restate existing PRAGMA documents
- Produce the condensed form alongside the original

The rule is published. Anyone can inspect it, challenge it, or propose modifications through a subsequent PROP. If the rule is wrong, the PROP process corrects it.

**Rule.** The condensation rule is a consensus artifact. It is not the chair's opinion. It is not editorial preference. It is a published, adopted, amendable process rule.

---

## 6. WHAT THE RULE PRESERVES

Every material claim survives condensation. The operation is lossless in substance and lossy only in restatement.

The original submission is always available. The condensed form is what the group works from. If any member believes the condensation lost substance, the original is the reference. The dispute is resolvable by comparison.

Nothing is suppressed. Nothing is overruled. The author's contribution is preserved in full. The condensed form is a lens, not a gate.

---

## 7. THE CHAIR'S EXISTING AUTHORITY

pragma-once.md Section 7: "A chair defines process: quality criteria, evaluation methodology, scheduling, output standards, self-assessment metrics."

Output standards include format and density. The condensation workflow is an output standard. Asking an author to break an overspecified PROP into parts is an output standard decision. No new authority is created. The workflow operates within the chair's existing latitude.

The succession responsibility: the chair transmits the understanding of why this workflow exists and how to adapt it as AI tooling changes. The current constraints are documented in the stream's process materials. The principle - that physical packaging is constrained by the processing medium - lives in the role.

---

## 8. COMMON QUESTIONS

**"This is censorship."**
The original is preserved. Substance is extracted, not suppressed. Censorship removes content. Condensation removes restatement.

**"The AI might miss nuance."**
The condensed form is advisory. The original is the reference. Any member can challenge the condensation by pointing to material in the original that the condensed form omits.

**"Thoroughness is a virtue."**
Thoroughness that adds signal is. Restatement is not thoroughness. The distinction is testable: does this sentence introduce information not present elsewhere in the document?

**"This adds process overhead."**
The agentic rule is automated. It adds a tool to the chair's workflow. It does not add a step to the author's.

**"Who decides what is redundant?"**
The rule does. The rule is published. The rule is adopted by consensus. If the rule is wrong, a PROP can amend it.
