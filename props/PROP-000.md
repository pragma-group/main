```
PROP: 000
Title: PRAGMA Proposal Protocol
Author: Vinnie Falco <vinnie.falco@gmail.com>
Status: Adopted
Type: Process
Created: 2026-02-26
Target: (self)
```

## Abstract

A PRAGMA Proposal (PROP) is a numbered document representing the consensus of the PRAGMA Group. Each PROP is a set of instructions that modifies one or more of PRAGMA's generating documents. This PROP defines the protocol, the format, and the lifecycle. It follows its own format and serves as the template for all subsequent PROPs.

## Motivation

PRAGMA produces evaluations, principles, and process documents that evolve over time. Changes to these documents need a formal mechanism that records what changed, why, who proposed it, and whether the group reached consensus. Without such a mechanism, changes accumulate informally and the rationale is lost.

The PROP protocol is modeled on established improvement proposal systems:

- [BIP (Bitcoin Improvement Proposals)](https://bips.dev/3/) - BIP-3, Updated BIP Process, 2025
- [EIP (Ethereum Improvement Proposals)](https://eips.ethereum.org/EIPS/eip-1) - EIP-1, EIP Purpose and Guidelines
- [PEP (Python Enhancement Proposals)](https://peps.python.org/pep-0001/) - PEP-1, PEP Purpose and Guidelines

These protocols have been proven across multiple communities over decades. The PROP protocol adopts their core structure and simplifies it for PRAGMA's scale.

## Specification

### What is a PROP

A PROP is a consensus output of the PRAGMA Group. It is not a suggestion, a discussion document, or a personal opinion. A PROP that reaches Adopted status modifies its target document. The PROP file remains as the permanent record of the change and its rationale.

### Lifecycle

Every PROP progresses through one of these paths:

```
Draft --> Adopted
Draft --> Rejected
Adopted --> Superseded (by a later PROP)
```

- **Draft**: proposed by an author as a pull request to the repository
- **Adopted**: consensus reached through chair-mediated straw poll; pull request merged; target document modified
- **Rejected**: consensus against; PROP preserved as a record of what was considered
- **Superseded**: a later PROP replaces this one; the superseding PROP is noted in the preamble

### Format

Every PROP is a Markdown file containing a preamble and four required sections.

**Preamble.** An RFC 822-style metadata block at the top of the file:

```
PROP: NNN
Title: (50 characters or fewer)
Author: Name <email>
Status: Draft | Adopted | Rejected | Superseded
Type: Principle | Process | Informational
Created: yyyy-mm-dd
Target: (document or PROP being modified, or "new" for new artifacts)
Superseded-By: (PROP number, if applicable)
```

**Required sections:**

- **Abstract** - one paragraph describing what the PROP does
- **Motivation** - why the change is needed; what problem it solves
- **Specification** - the exact change to the target document; precise enough to execute
- **Rationale** - why this approach; what alternatives were considered; how objections were addressed

**Optional trailing section:**

- **Agentic Rule Listing** - if a PROP defines an AI rule, prompt, or command intended for verbatim use, the full text appears in a final section after Rationale. The listing is self-contained and separated by horizontal rules so the chair can copy it into a rule file or paste it directly into a prompt without extracting it from the surrounding PROP text.

### Types

- **Principle** - adds or modifies evaluation criteria in Stream 1
- **Process** - modifies how PRAGMA operates, including PROP-000 itself
- **Informational** - records a decision, observation, or rationale without modifying a target document

### Who Can Propose

Any PRAGMA Group member can propose a PROP by opening a pull request to the repository containing the new PROP file in `props/`. After submitting the pull request, the author announces it to the mailing list.

### Consensus

Discussion happens on the mailing list, not on the pull request. Pull request comments are proprietary to the hosting platform and can be lost; the mailing list is the permanent record. The chair mediates discussion on the list and conducts straw polls there. Disagreements are recorded in the PROP itself before merging. Adoption requires consensus, not unanimity. The chair discovers consensus; the chair does not impose it. Merging the pull request enacts the PROP.

### What a PROP Can Modify

- The operational document (pragma-next.md)
- Stream 1 (evaluation principles and criteria)
- Process rules (including PROP-000 itself)
- Any other artifact in the PRAGMA repository

The founding documents in `const/` carry the highest bar for change. They are not part of the standard PROP lifecycle. Changes require unanimous consent through a separate deliberation process determined by the group.

### Numbering

PROPs are numbered sequentially with three-digit zero-padding: PROP-000, PROP-001, PROP-002. Three-digit padding ensures filesystem sort order matches logical order. PROP-000 is this document. The first real proposal is PROP-001.

### Repository Layout

All PROPs live in `props/`. Filenames follow the pattern `props/PROP-NNN.md`.

PROPs are modified in place when adopted. Git history preserves all prior versions. To see the history of any PROP, consult the git log for that file.

To modify any existing PROP - including PROP-000 - propose a new PROP that targets it. The process governs itself.

### Rejected PROPs

Rejected PROPs are preserved in the repository. They document what was considered and why it was not adopted. Institutional memory includes decisions not to act.

## Rationale

**Why model on BIP/EIP/PEP.** These protocols have been tested across communities ranging from dozens to thousands of participants over periods of ten to twenty years. The core structure (numbered proposals, metadata preamble, required sections, lifecycle states) has proven durable. Adopting a proven model avoids inventing a process from scratch.

**Why simplify.** BIP-3 includes Layer, Deputies, License, Reference Implementation, Backward Compatibility, and Version headers. PRAGMA's scale does not require these. A small group of trusted practitioners operating on a single repository needs less process, not more. If PRAGMA grows to need these elements, a PROP can add them.

**Why self-referential.** PROP-000 follows the format it defines. This eliminates the need for a separate template document and demonstrates the format by example. Every subsequent PROP author can use PROP-000 as the reference.

**Why three-digit numbering.** Filesystem sort order. `PROP-001.md` sorts before `PROP-010.md` sorts before `PROP-100.md`. Two digits would require renaming at PROP-100. Four digits are unnecessary at PRAGMA's expected volume.

**Why modified in place.** Git provides version history automatically. Maintaining separate version files (PROP-000-v1.md, PROP-000-v2.md) duplicates what git already does. The current file always reflects the current state. The history is in the repository.

**Why Lakos Principle applies.** All PROP text follows the Lakos Principle: no "our" or "should." PROPs describe what changes and why. They do not claim ownership or issue directives.

## References

- [BIP-3: Updated BIP Process](https://bips.dev/3/) - Murch, 2025
- [EIP-1: EIP Purpose and Guidelines](https://eips.ethereum.org/EIPS/eip-1) - Ethereum Foundation
- [PEP-1: PEP Purpose and Guidelines](https://peps.python.org/pep-0001/) - Warsaw, Hylton, Goodger
