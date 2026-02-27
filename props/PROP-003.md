```
PROP: 003
Title: Membership Lifecycle
Author: Vinnie Falco <vinnie.falco@gmail.com>
Status: Draft
Type: Process
Created: 2026-02-27
Target: new
```

## Abstract

This PROP defines the specific mechanics for PRAGMA membership: size limits, inactivity timeouts, and succession. It operationalizes the principles defined in `pragma-pack.md`.

## Motivation

`pragma-pack.md` establishes that the group must be small and active. It does not define "small" or "active." Without specific numbers, these principles drift. A group of 50 is not small. A member who hasn't voted in two years is not active. This PROP sets the parameters.

## Specification

### 1. Size Cap

The active member cap is **9**.

Expansion beyond 9 requires unanimous consent of the active members. The cap forces the group to make hard choices about composition. If a new perspective is needed, and the group is full, the group must decide if the new perspective is more valuable than an existing one, or if the expansion is justified.

### 2. Inactivity Timeout

Inactivity is defined as missing **3 consecutive evaluation cycles**.

A member who meets the inactivity definition is automatically moved to **Emeritus** status. This is not a punishment. It is a garbage collection mechanism for the voting pool.

### 3. Emeritus Status

Emeritus members retain:
- Access to the private mailing list.
- Ability to participate in discussions.
- Ability to propose PROPs.

Emeritus members do not:
- Vote in straw polls.
- Count toward the quorum or the size cap.

An Emeritus member can return to Active status if a slot is available and the Chair approves.

### 4. Succession

The Chair appoints a successor. The appointment is confirmed by a **majority vote** of the active members.

If the Chair vacates the position without appointing a successor, the active members elect a new Chair by majority vote.

## Rationale

**Why 9.** The "two-pizza rule." 9 people can have a single conversation. 20 people cannot. High-bandwidth communication requires a small graph.

**Why 3 cycles.** PRAGMA operates on the WG21 mailing cadence (monthly/bimonthly). Missing 3 cycles means missing ~6 months of work. A member who has been absent for 6 months has lost context.

**Why Chair appoints.** PRAGMA is a vision-driven organization (Layer 0). The Chair is the guardian of that vision. Succession by appointment ensures continuity of the founding intent. Confirmation by vote prevents the appointment of a tyrant.

**Why a PROP.** These numbers may need adjustment. If 9 proves too small, or 3 cycles too short, the group can amend this PROP. The principles in `pragma-pack.md` remain fixed; the parameters in `PROP-003` evolve with evidence.
