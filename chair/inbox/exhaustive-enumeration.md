# Exhaustive Enumeration

PROP-001 handles redundant restatement. This document identifies a complementary failure mode that the condensation rule does not detect.

---

## 1. THE THESIS

Overspecification has two forms. PROP-001 addresses one. The chair's judgment addresses the other.

The first form is redundant restatement: the same material point expressed multiple times. The condensation rule detects this mechanically. It merges restatements, preserves each point exactly once, and produces a condensed form. The rule handles it. The chair applies the rule.

The second form is exhaustive enumeration: many distinct material points, each stated once, accumulating to a volume that defeats the document's usability. Every point is non-redundant. Every point passes the condensation rule unchanged. The document grows not by saying one thing twice but by saying thirty things once.

The condensation rule is structurally blind to the second form. It preserves all material points. That is its design. When every point is distinct, there is nothing to merge. The rule returns the document unchanged. The volume persists.

---

## 2. HOW EXHAUSTIVE ENUMERATION ARISES

A criteria-driven practitioner identifies a gap in a specification. The gap is real. The practitioner proposes an amendment. The amendment is a new material point - information not present in the existing document.

Then another gap. Another amendment. Another material point.

Each amendment is individually justified. Each passes the condensation rule. Each is non-redundant. The failure mode is not in any single amendment. It is in the accumulation. A specification with thirty non-redundant clauses is as hard to read as a specification with ten clauses each stated three times. Both are thirty effective paragraphs. The condensation rule compresses the second to ten. It leaves the first at thirty.

The mechanism is different from redundant restatement. The practical effect on document usability is the same.

---

## 3. WHY THE CONDENSATION RULE CANNOT ADDRESS IT

The condensation rule's definition: "A material point is a sentence or clause that introduces information not present in other material points." Exhaustive enumeration introduces information. Each point is novel. The rule's filter passes every one.

Adding a novelty filter to the condensation rule would require the rule to judge which material points are essential and which are deferrable. That is a judgment about priorities, not about redundancy. Priority judgment is the chair's function, not the rule's.

The condensation rule is a tool. The chair is the architect. Tools detect patterns. Architects make decisions about what to build and when.

---

## 4. THE CHAIR'S ROLE

When the condensation rule returns a document largely unchanged but the document is long, the chair asks a different question: not "which points are redundant?" but "which points are necessary for the current deployment?"

A specification that preemptively addresses every edge case is a monolithic design. A specification that addresses the common case and defers edge cases to future amendments is an incremental design. Incremental design ships sooner, accumulates field evidence before extending, and avoids specifying solutions to problems that may not arise.

The chair's judgment call: when a PROP accumulates non-redundant amendments, ask whether each amendment is necessary now or deferrable to a future PROP when evidence supports it.

This is not a rule. It is guidance. The chair exercises judgment within the latitude pragma-once.md Section 7 grants.

---

## 5. THE PRINCIPLE

Ship the base. Extend when evidence supports it.

A PROP that specifies success metrics, edge-case boundaries, deployment procedures, review checkpoints, and style-dispute resolution before it has been applied once is specifying answers to questions that have not yet been asked. Some of those questions may never arise. Some may arise differently than anticipated. Preemptive specification locks in answers that field experience would have improved.

The same principle appears in pragma-once.md Section 8: "Adding scope before the group has demonstrated that single scope produces value is premature. Ship the base. Extend when the evidence supports it."

Applied to specification depth: adding precision before the group has demonstrated that the base specification is insufficient is premature. Ship the base. Amend when the evidence supports it.

---

## 6. WHAT TO WATCH FOR

Signs that exhaustive enumeration is occurring:

- A PROP's amendment list grows faster than its deployment history.
- Amendments address scenarios the group has not encountered.
- The condensation rule returns a document unchanged but the document exceeds the length of the documents it modifies.
- Discussion shifts from "does this work?" to "what about this edge case?" before the base has been tested.

None of these is disqualifying. Each is a signal that the chair may want to suggest deferral rather than specification.

---

## 7. THE RELATIONSHIP TO PROP-001

PROP-001 and this guidance are complementary.

| Failure mode           | Mechanism                        | Detection             | Resolution            |
|------------------------|----------------------------------|-----------------------|-----------------------|
| Redundant restatement  | Same point stated multiple times | Condensation rule     | Merge to single point |
| Exhaustive enumeration | Many distinct points stated once | Chair's judgment      | Defer to future PROPs |

The condensation rule is automated, published, and consensus-adopted. This guidance is a suggestion in the chair's inbox. The asymmetry is intentional. Redundancy detection is mechanical. Priority judgment is not.

---

## 8. COMMON QUESTIONS

**"Is this telling the chair to reject amendments?"**
Defer, not reject. An amendment deferred to a future PROP is not lost. It is sequenced. The material point is noted. The specification grows when evidence supports it rather than when imagination anticipates it.

**"How does the chair know which amendments are deferrable?"**
Ask: has the group encountered the scenario this amendment addresses? If not, the amendment is preemptive. Preemptive amendments may be correct. They are also candidates for deferral.

**"Does this apply to the chair's own amendments?"**
Especially. The chair who recognizes this pattern in submissions and not in the chair's own process modifications has a blind spot. Self-assessment is part of the chair's contract (pragma-once.md Section 7).

**"This document is itself preemptive."**
The inbox can hold one.
