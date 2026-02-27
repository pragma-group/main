# PRAGMA Next

Operational living document for the PRAGMA Group.

---

## What This Document Is

The PRAGMA Group has three documents:

- **pragma.md** - The founding document. What PRAGMA is. Public-facing. Changes slowly through group consensus.
- **pragma-once.md** - The strategy document. Why PRAGMA operates the way it does. Internal. The argument behind the posture.
- **pragma-next.md** - This document. The operational log. What the group has decided, what is open, what comes next. Internal. Changes rapidly, especially in the early period.

This document captures transient knowledge: operational principles from deliberation, open questions awaiting resolution, decisions made and their rationale, and the agenda for upcoming meetings. It is the group's working memory.

---

## How to Contribute

**Adding an item.** Any member can add an item. Tag it with name and date. Place it in the appropriate section.

**Format.** Each logged item follows this pattern:

> **Person Name, Month Day Year:** Content of the item.

**What belongs here:**
- Operational decisions (how the group works day to day)
- Principles proposed by members for discussion or adoption
- Open questions deferred to a future meeting
- Meeting agenda items
- Process observations and lessons learned

**What does NOT belong here:**
- Changes to the founding document (those go through group consensus applied to pragma.md)
- Strategy reasoning (that lives in pragma-once.md)
- Evaluation outputs (those go in Stream 2 papers)

**Items are never deleted.** Superseded items are struck through and annotated with what replaced them. The history is the record.

---

## Operational Principles

These are principles proposed or adopted through group deliberation. Each is tagged with its source.

### From John Lakos

**John Lakos, February 26, 2026:** Principles must be overwhelmingly correct to start. The threshold must be high enough that reasonable people cannot argue with the initial set. Target 95-5 issues or better. Ideally validated through a survey or equivalent consensus mechanism.

**John Lakos, February 26, 2026:** The principle base must grow. As the group captures more expert knowledge and applies it to more papers, the evaluation criteria will expand. Growth is expected and welcome.

**John Lakos, February 26, 2026:** Change must be accommodated. Evaluation criteria will be refined as reality teaches the group what works and what does not. First attempts rarely survive contact with the full range of proposals.

**John Lakos, February 26, 2026:** Revision history is essential. Every principle, every evaluation model, and every output must be versioned so that any prior evaluation can be reproduced against the exact set of principles that produced it. Regression analysis when principles change is basic QC/QA. Implementation: git.

**John Lakos, February 26, 2026:** Every single false positive is ammunition against the group. Every output must be vetted by at least one expert human. No exceptions.

**John Lakos, February 26, 2026:** Two levels of success criteria. Level 1: are we doing what we intended to do? Level 2: is what we are doing having the intended effect? Both are important. The second is existential.

**John Lakos, February 26, 2026:** Call out especially good work, not just problems. If a paper does an especially good job on a principle, note it. If a paper objectively fails to follow a principle, note it. Otherwise: LGTM.

**John Lakos, February 26, 2026:** No "our" and no "should" in public materials. "Our" is alienating. "Should" implies authority. Neither belongs in documents from a group that asks for nothing. (Adopted as the Lakos Principle; see pragma-once.md Section 11.)

### From Joshua Berne

**Joshua Berne, February 26, 2026:** The methodology is reusable with different principles. Others can apply the same evaluation system with their own principles and see what results emerge. (Adopted in pragma.md, item 3 of What We Produce.)

**Joshua Berne, February 26, 2026:** ISO code of conduct expected for members. The internal communication of the group is predicated on all members having agreed to follow the ISO code of conduct. Public mailing lists ask for a similar level of professionalism but cannot guarantee it.

**Joshua Berne, February 26, 2026:** The first product cannot be 100% non-controversial or it will be uninspiring. The group needs to find the right line between providing real constructive feedback and being overly opinionated in initial outputs.

**Joshua Berne, February 26, 2026:** Membership governance is needed before public launch. Who qualifies as a member, how one becomes a member, what qualities and expectations apply. Does not need to be solved immediately but must be addressed in the founding document before it goes public.

### From Vinnie Falco

**Vinnie Falco, February 26, 2026:** Evaluation models are not one-size-fits-all. A bug fix, a library proposal, and a core language extension require different evaluation criteria. Without a categorization step, there is no way to route a paper to the right model. Categorization is not an opinion about quality. It is the prerequisite for applying evaluation models at all.

**Vinnie Falco, February 26, 2026:** Every mailing analysis begins with a categorization pass. The pass is procedural and unopinionated. It assigns each paper to a category. Opinionated evaluation follows only after routing is complete.

**Vinnie Falco, February 26, 2026:** The taxonomy is a group decision, formalized through a PROP. Until the PROP is adopted, no evaluation can run because there is nothing to route against.

**Vinnie Falco, February 26, 2026:** The taxonomy does not need to be exhaustive before work begins. An "uncategorized" category allows the group to ship a useful categorization without gating it on a complete taxonomy. Papers that do not fit an existing category are placed in "uncategorized" and the taxonomy grows as the group learns what categories are needed.

**Vinnie Falco, February 27, 2026: The Bearing Canary.** Every mailing evaluation includes a one-line statement: "The PRAGMA founding documents have not changed since [date]." The bearing is from pragma-once.md Section 5: a lighthouse holds a bearing; everything else changes. The canary is the warrant canary pattern: its presence is the signal; its absence is the alarm. The Bearing Canary is verifiable - anyone can check `git log const/` and confirm. It costs nothing to maintain when true. It accumulates credibility over time: the same date printed eighteen months later is a credential. If the founding documents change, the date updates visibly. If the line disappears from a mailing, that absence is itself the signal. The Bearing Canary belongs in the mailing evaluation output template once that template is defined.

---

## Open Questions

Items deferred to the first meeting or future deliberation.

**The two-layer question.** Which principles belong in a fixed category and which evolve? Lakos and Berne have different positions. pragma-once.md Section 5 frames the question. The group must deliberate.

**Membership criteria.** Who qualifies as a member? What are expectations? How does someone join? (Berne raised, deferred to meeting.)

**Chair appointment.** Berne has been proposed. The chair discovers consensus; the chair does not impose it. Must be formalized at the first meeting.

**Code of conduct.** Adopt the ISO code of conduct for the members list? (Berne proposed.)

**Principle validation.** How to survey or otherwise validate that initial principles meet the 95-5 threshold. (Lakos proposed; method TBD.)

**Success metrics.** Process metrics (are we executing?) vs. outcome metrics (is it working?). Lakos's two-level framework. How to measure each. What timeframe before outcome metrics are evaluated.

**First evaluation target.** Which WG21 mailing does the group respond to first? The categorization taxonomy must be defined (via PROP) before the first evaluation can run. The categorization pass itself can target any published mailing and is unopinionated. The first opinionated evaluation follows once the taxonomy and at least one evaluation model are in place.

**Public vs. WG21-only participation.** The public mailing list is open to everyone. The private list is restricted to WG21 members (see pragma-once.md Section 12). Is there a membership distinction between the two? (Deferred.)

---

## Meeting Agenda: First Meeting

Accumulated from founding deliberations, February 26, 2026.

1. Chair appointment
2. The two-layer question: institutional values vs. evaluation criteria
3. Initial principle selection: methodology and threshold
4. Membership criteria and governance
5. Code of conduct adoption
6. Success metrics: Lakos two-level framework
7. First evaluation target: which mailing?
8. Paper categorization taxonomy: categories, partial-categorization approach, PROP path
9. Email vs. meeting cadence: how the group communicates between meetings

---

## Decisions Log

Decisions made by the group, recorded with date and rationale.

**February 26, 2026:** The founding document (pragma.md) adopts the Lakos Principle: no "our" and no "should" in public materials. Document scrubbed and republished. (Proposed by John Lakos, adopted immediately by consensus.)

**February 26, 2026:** The founding document adds a purpose sentence: "Standardization proposals benefit from principled, independent evaluation against disclosed criteria." (Proposed in response to Joshua Berne's feedback that the document lacked stated purpose.)

**February 26, 2026:** The founding document makes evaluation models explicitly reusable: "disclosed, so anyone can verify, challenge, or apply them with different principles." (Proposed by Joshua Berne.)

**February 26, 2026:** The founding document simplifies to one public mailing list. Private list rationale documented in pragma-once.md Section 12.
