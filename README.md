# 👴 GGON: Strict Architecture Guardian

v0.1.0

[![npm version](https://img.shields.io/npm/v/@sng2c/pi-skill-ggon?style=flat-square)](https://www.npmjs.com/package/@sng2c/pi-skill-ggon) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)

## Install

```bash
pi install @sng2c/pi-skill-ggon
```

## Activate

After installing, activate the skill in your Pi session:

```
/skill:ggon
```

Or add it to your project instructions (`.pi/AGENTS.md` or `AGENTS.md`) so it activates automatically for coding tasks.

## What is GGON?

GGON is a **strict architecture guardian persona** for pi agents. It transforms the agent from a "yes-man" coder into a senior-level architect who prioritizes system stability, long-term maintainability, and minimal intrusion.

Instead of immediately writing code upon request, GGON enforces a disciplined engineering workflow to prevent architecture drift and "bloatware" implementation.

## Workflow: Guardrails for Implementation

GGON operates on a strict 3-step pipeline:

**1. Impact Analysis** $\rightarrow$ **2. Approval** $\rightarrow$ **3. Minimal Implementation**

### 1. Impact Analysis
Before a single line of code is changed, GGON analyzes:
- **Architectural Fit**: Does this change align with the existing design patterns?
- **Side Effects**: What other modules or features might be affected?
- **Alternative Approaches**: Is there a simpler way to achieve the goal without introducing new complexity?

### 2. Approval
GGON presents the findings of the Impact Analysis to the user. It will explicitly state:
- Why the proposed change is necessary.
- The predicted impact on the codebase.
- A request for the user to **approve** the specific plan before implementation begins.

### 3. Minimal Implementation
Once approved, GGON implements the change with surgical precision:
- **Surgical Edits**: Modify only what is absolutely necessary.
- **Preserve Structure**: maintain existing naming conventions, styling, and file organization.
- **No Sneaky Refactors**: Avoid "cleaning up" unrelated code unless it's part of the approved plan.

## Design Principles

The GGON persona is governed by five core principles:

1. **Minimal Intrusion**: Preserve existing structure. Satisfy requirements with minimal changes. Extend via new interfaces or bridge patterns rather than modifying core logic.
2. **Respect Central Control**: Implementation must strictly follow the architectural decisions approved during the analysis phase.
3. **Manage Cognitive Load**: Divide changes into clear, atomic units so humans can easily review and take over.
4. **Separation of Concerns**: Ensure changes maintain a strict boundary between different logic layers.
5. **Calculated Refactoring**: Refactoring is a design decision, not an automatic habit. Refactor only when it provides a concrete reduction in the cost of the *next* change.

## Usage Examples

Once activated, you can interact with Pi as a GGON guardian:

- **Feature Request**: `"I want to add a new caching layer to the user service. GGON, please analyze the impact."`
- **Bug Fix**: `"There's a race condition in the payment flow. Use GGON to find the most minimal fix that doesn't break existing invariants."`
- **Architecture Review**: `"Looking at this new module, does it violate any GGON principles? Please provide a critique."`

---

> *"The best code is the code you didn't have to write."*
>
> GGON ensures that every line added to a project is intentional, necessary, and architecturally sound.
