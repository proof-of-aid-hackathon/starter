# Proof of Aid Hackathon

> **Design the complete system. Build one meaningful part in depth.**

This repository is your team's official Hackathon workspace.

It has been created for your team by the organizers from the official Proof of Aid starter repository. During the Hackathon, you will use it to design your complete Proof of Aid system, build one concrete contribution, document your work, and submit the exact versions to be evaluated.

All submitted work, documentation, demos, and the final pitch must be in **English**.

---

## At a glance

| Question                                            | Answer                                                                                                                    |
| -----------------------------------------------------| ---------------------------------------------------------------------------------------------------------------------------|
| **What are we solving?**                            | The broader Proof of Aid problem.                                                                                         |
| **What are we expected to do?**                     | First design your complete Proof of Aid system. Then choose one meaningful part of that system and implement it in depth. |
| **Do we need to build the whole system?**           | **No.** The complete system is a design exercise. Only one meaningful contribution needs to be implemented.               |
| **Do we have to use blockchain?**                   | Use it where it provides meaningful value.                                                                                |
| **Can we choose our own approach?**                 | Yes. Your system design, technologies, implementation focus, and technical approach are open.                             |
| **Are there mandatory tracks?**                     | No. The contribution areas below are prompts, not tracks.                                                                 |
| **Where does our code go?**                         | `implementation/`                                                                                                         |
| **Where do we explain the project?**                | `SUBMISSION.md`                                                                                                           |
| **How do we submit a checkpoint or final version?** | Push the state to `main` and submit the corresponding **commit SHA** through the official submission form.                |
| **What should we do first?**                        | Understand Proof of Aid and start designing the complete system before narrowing down what you will implement.            |

---

# 1. Proof of Aid in one minute

A real aid process may move through something like:

```text
Need
  ↓
Evidence / verification
  ↓
Funding
  ↓
Delivery
  ↓
Outcome
  ↓
Transparent history
```

Different actors may create information, verify it, provide funding, deliver aid, receive it, or inspect what happened.

Designing Proof of Aid means deciding how these actors, flows, technologies, trust relationships, and real-world events should work together as a coherent system.

There is no single expected architecture.

Your system may involve interfaces, conventional software, APIs, identity, payments, evidence, external systems, data processing, blockchain, or any combination that you can justify.

---

# 2. The challenge

The Hackathon has **two different scopes**.

## Part A — Complete System Design

Design your vision of **Proof of Aid as a complete system**.

We want to understand how you think the full system should work, including:

* the actors involved;
* the end-to-end aid flow;
* the main components;
* the architecture;
* the technologies or approaches you would use;
* why you would use them;
* important design decisions;
* trust assumptions;
* relevant privacy and security considerations;
* important trade-offs and simplifications.

You are **not expected to implement the complete system**.

This part is about demonstrating that you understand the wider Proof of Aid problem and can design a coherent solution to it.

---

## Part B — Implemented Contribution

Once you have a complete system in mind:

1. choose one meaningful area of that system;
2. identify a concrete problem within it;
3. decide how you want to address that problem;
4. implement a demonstrable contribution in depth;
5. validate it through a concrete scenario.

Your implementation should fit coherently into the complete system you designed.

> **Depth matters more than feature count.**

A focused implementation that explores one important problem well is preferable to a shallow implementation of many unrelated features.

---

# 3. Contribution areas

The following areas can help you explore Proof of Aid and later choose where to focus your implementation.

They are **lenses for exploring the problem, not mandatory tracks**.

You may focus on one, combine several, or identify another relevant cross-cutting problem.

You are not expected to answer every question below.

## Claims & Lifecycle

How should an aid need be represented and managed through its lifecycle?

Questions you might explore:

* How can a need be structured clearly and verifiably?
* How should budget changes, milestones, delays, cancellations, or partial execution be represented without losing history?
* How can actors understand the current state and what should happen next?

## Trust, Evidence & Privacy

How can the system show who claims or verifies something, what evidence supports it, and what can be trusted without unnecessarily exposing sensitive information?

Questions you might explore:

* Who verified a need, delivery, or outcome?
* How can something be proven without publishing sensitive documents or personal information?
* How should corrections or conflicting evidence be handled?

## Funding

How should money be tracked from funding to actual availability and use?

Questions you might explore:

* How do we distinguish donated, received, reserved, and available funds?
* How can funds from different channels or providers be reconciled?
* What determines when funds can be released or used?

## Delivery & Impact

How do we connect funding to real-world execution and outcomes?

Questions you might explore:

* How can the system show that aid was actually delivered?
* How do we distinguish a purchase, a delivery, and an outcome?
* How can beneficiaries or communities confirm or challenge what happened?

## Transparency & UX

How can the history of an aid process be understandable to different actors?

Questions you might explore:

* How can users understand what happened to the money and the aid?
* How should declared, verified, disputed, and uncertain information be distinguished?
* How should information differ for donors, NGOs, auditors, beneficiaries, or other actors?

---

# 4. Implementation dimensions

Once you choose what to implement, describe where that **implementation effort** is concentrated across three dimensions:

| Dimension                 | Includes                                                                                                                                |
| ---------------------------| -----------------------------------------------------------------------------------------------------------------------------------------|
| **UX**                    | User flows, interfaces, dashboards, reporting, visualisation, and interaction design.                                                   |
| **Real-world connection** | Evidence, verification, identity, attestations, oracles, payments, APIs, integrations, external data, and real-world events.            |
| **Blockchain**            | Smart contracts, shared records, on-chain hashes or attestations, settlement, traceability, or other blockchain-based trust mechanisms. |

Example:

```text
UX: 60%
Real-world connection: 30%
Blockchain: 10%
```

These percentages:

* describe where your team concentrated its **implementation effort**;
* are not scores;
* have no ideal distribution;
* should sum to 100%.

They describe the part you actually decided to build, not the complete system design.

---

# 5. Your GitHub workspace

## Your team repository

The organizers will assign your team a private repository inside the official Hackathon GitHub Organization.

Conceptually:

```text
proof-of-aid-hackathon/team-XX
```

This is your **official workspace and submission repository**.

You do not need to:

* fork the public starter repository;
* create another repository;
* change repository visibility;
* invite mentors or jury members;
* manage submission permissions.

The organizers manage repository ownership and access centrally.

> [!IMPORTANT]
> If any team member cannot access the assigned repository, contact the organizers. Do not create a replacement repository under a personal account.

---

## Access and privacy

During the Hackathon:

* your team can read and write to its own repository;
* other participant teams cannot access it;
* organizers can administer it;
* authorized mentors and jury members can read it.

Your repository remains private during the competition.

Even though the repository is private, **never commit real secrets, private keys, production credentials, API secrets, or sensitive personal data**.

---

## `main` is the canonical project state

The state used for checkpoints and final submission must be committed and pushed to:

```text
main
```

You may work directly on `main`.

If your team prefers to use branches, that is also fine. There is no required branching workflow.

However, before a checkpoint or final submission:

> **Make sure everything you want evaluated is committed and available on `main`.**

No Pull Request workflow, GitFlow process, or Release is required.

---

# 6. Start working

## Step 1 — Clone your assigned repository

The organizers will provide your team repository.

```bash
git clone <your-team-repository-url>
cd <repository>
```

Verify that every team member can access it before starting substantial work.

---

## Step 2 — Design the complete Proof of Aid system

Before narrowing your scope, think about how you would design Proof of Aid as a whole.

Open [`SUBMISSION.md`](./SUBMISSION.md) and start working on the **Complete System Design**.

Consider:

* who the actors are;
* how an aid process moves from need to outcome;
* what information exists and where;
* which components are required;
* how those components communicate;
* which technologies or approaches make sense;
* where trust exists;
* what should be verifiable;
* what should remain private;
* where blockchain is useful;
* what important trade-offs your design introduces.

Your design does not need to be final before you start implementing.

It should evolve as your understanding improves.

---

## Step 3 — Choose your implementation focus

Once you have a reasonable view of the complete system, decide where your team wants to go deeper.

Choose:

1. one meaningful area or combination of areas;
2. a concrete problem inside that part of the system;
3. an approach for addressing it.

A useful test is whether you can complete:

> Within our complete Proof of Aid design, we are focusing on **[area]** and addressing **[concrete problem]** by **[approach]**.

This focus may evolve during the Hackathon.

---

## Step 4 — Build the contribution

Implement your selected contribution under:

[`implementation/`](./implementation/)

Your implementation can involve:

* frontend;
* backend;
* smart contracts;
* APIs;
* data processing;
* identity;
* payments;
* verification;
* attestations;
* integrations;
* dashboards;
* infrastructure;
* scripts;
* mocks;
* or any combination that supports your contribution.

There is no required technology stack.

---

## Step 5 — Keep design and implementation separate

The complete system you propose will probably be much larger than what you can implement during the Hackathon.

That is expected.

Your documentation must make the boundary clear.

Use these statuses when describing the relationship between your system design and prototype:

| Status                 | Meaning                                                                           |
| ---------------------- | --------------------------------------------------------------------------------- |
| **Implemented**        | Working code or another demonstrable technical artifact exists in the repository. |
| **Simulated / mocked** | A real component has been replaced or simplified for the prototype.               |
| **Designed only**      | It belongs to the complete proposed system but was not implemented.               |
| **Out of scope**       | It is deliberately excluded from the proposed Hackathon scope.                    |

The jury should never have to guess which category something belongs to.

---

# 7. Repository structure

Your repository starts with:

```text
/
├── README.md
├── SUBMISSION.md
└── implementation/
    └── README.md
```

You may organize `implementation/` however your project requires.

For example:

```text
implementation/
├── frontend/
├── backend/
├── contracts/
└── README.md
```

or:

```text
implementation/
├── pipeline/
├── scripts/
└── README.md
```

These are examples only.

Keep the root repository simple unless your project genuinely requires additional top-level files.

---

# 8. What you must deliver

Your final submission has **two main parts**.

## A. Complete System Design

Documented in `SUBMISSION.md`.

It should explain your complete vision for Proof of Aid:

* system vision;
* actors and end-to-end flow;
* architecture and components;
* proposed technologies or approaches;
* important design decisions;
* justification and trade-offs.

You are not expected to implement all of this.

---

## B. Implemented Contribution

Also documented in `SUBMISSION.md`, with the code under `implementation/`.

It should explain:

* the area you chose to explore;
* the concrete problem you identified;
* why you chose that problem;
* your approach;
* how it fits into the complete system;
* what you actually built;
* what is mocked, simulated, designed only, or out of scope;
* how the implementation is validated.

---

## `implementation/README.md`

This must contain enough operational information for another technical person to:

* understand what is there;
* install it;
* configure it;
* run it;
* validate it;
* reproduce the demo.

---

## A submitted commit SHA

Checkpoints and final submissions are identified by an exact Git commit.

The commit SHA — not the current state of `main` at some later time — defines the submitted version.

---

# 9. Demo expectations

The demo concerns your **implemented contribution**, not the complete system design.

It should prove one concrete thing about what you built.

A useful structure is:

```text
Initial state
    ↓
Action
    ↓
System behaviour
    ↓
Observable result
```

Instead of:

> We will show our platform.

prefer something like:

> An organisation creates an aid claim, a verifier attaches evidence, and the implemented component exposes the resulting verification state.

Your demo may use mocked or simulated components.

If it does, identify them explicitly.

If the demo depends on:

* a deployed service;
* external API;
* test wallet;
* test credentials;
* seeded database;
* blockchain network;
* manually operated component;

document everything required in `implementation/README.md`.

---

# 10. Thursday checkpoint

[ORGANIZERS: CONFIRM CHECKPOINT DEADLINE AND ADD SUBMISSION FORM]

There is **no separate checkpoint document**.

The checkpoint is a snapshot of your normal project repository at a specific commit.

At checkpoint time, `SUBMISSION.md` should contain at least:

* your current complete-system vision;
* a first end-to-end flow and architecture;
* your chosen implementation area;
* the concrete problem you are addressing;
* your planned approach;
* the current implementation dimensions;
* what currently works;
* what is still missing or simulated.

Before the deadline:

1. update `SUBMISSION.md`;
2. make sure the relevant implementation is pushed;
3. make sure everything to be reviewed is on `main`;
4. create a checkpoint commit;
5. push `main`;
6. obtain the exact commit SHA;
7. submit your **Team ID + commit SHA** through the official checkpoint form.

For example:

```bash
git status
git add .
git commit -m "Thursday checkpoint"
git push origin main
git rev-parse HEAD
```

The final command returns something like:

```text
4ab731c2d82a...
```

That SHA identifies the exact checkpoint state.

After submitting it, **continue working normally**.

Later commits do not change the submitted checkpoint.

---

# 11. Final submission

Before the deadline:

1. complete the **Complete System Design** in `SUBMISSION.md`;
2. complete the **Implemented Contribution** documentation;
3. finalize the implementation;
4. test the documented setup and demo;
5. merge any work you want evaluated into `main`;
6. make sure all required files are committed;
7. push `main`;
8. obtain the exact commit SHA;
9. submit your **Team ID + final commit SHA** through the official form.

Recommended final check:

```bash
git status
git log -1 --oneline
git push origin main
git rev-parse HEAD
```

Submit the SHA returned by the final command.

**[ORGANIZERS: ADD FINAL SUBMISSION FORM]**

> [!IMPORTANT]
> The commit SHA submitted through the official form defines the version that will be evaluated.

You do **not** need to write the final SHA inside `SUBMISSION.md`.

After the submission deadline, the organizers will make team repositories read-only for participants.

You will still be able to access your project while preparing the pitch, but the evaluated submission will remain frozen.

---

# 12. AI usage

AI tools are allowed.

Your team must disclose meaningful AI use in `SUBMISSION.md`, including:

* tools used;
* what they were used for;
* relevant generated or assisted parts;
* how those outputs were reviewed, tested, or validated.

You do not need to document every autocomplete suggestion.

> Your team must be able to explain and technically defend everything submitted.

---

# 13. Schedule

## Thursday 24

| Time            | Activity                                                             |
| --------------- | -------------------------------------------------------------------- |
| 08:30           | Accreditation                                                        |
| 09:00           | Welcome and talks                                                    |
| ~11:00          | Breakfast, remaining team formation, and Hackathon start — Room 3.01 |
| Rest of the day | Development and mentoring                                            |

[ORGANIZERS: ADD CHECKPOINT TIME IF CONFIRMED]

## Friday 25

| Time        | Activity                          |
| ----------- | --------------------------------- |
| Morning     | Development and mentoring         |
| **14:00**   | **Final submission deadline**     |
| 14:00–15:00 | Participant lunch and jury review |
| 15:00       | Finalists announced               |
| 15:00–16:00 | Pitch preparation                 |
| 16:00       | Pitches                           |
| 17:00       | Awards and closing                |

[ORGANIZERS: ADD FINAL PITCH DURATION AND Q&A FORMAT WHEN CONFIRMED]

---

# 14. Resources

## Must read

* [ORGANIZERS: ADD CORE PROOF OF AID REFERENCE]

## Recommended

* [ORGANIZERS: ADD RECOMMENDED RESOURCES]

## Optional deep dives

* [ORGANIZERS: ADD OPTIONAL TECHNICAL OR DOMAIN RESOURCES]

You do not need to read every optional resource before starting.

---

# 15. Before submitting

Your submission is ready when:

### Complete System Design

* [ ] Your vision of the complete Proof of Aid system is clear.
* [ ] The main actors and end-to-end flow can be understood quickly.
* [ ] The architecture and major components are explained.
* [ ] Important technology choices or approaches are justified.
* [ ] The main design decisions, assumptions, and trade-offs are explicit.

### Implemented Contribution

* [ ] The implementation focus is clearly derived from the complete system.
* [ ] The concrete problem addressed by the implementation is clear.
* [ ] It is obvious what your team actually built.
* [ ] Implemented, simulated, designed-only, and out-of-scope elements are clearly distinguished.
* [ ] The code is under `implementation/`.
* [ ] `implementation/README.md` contains working run instructions.
* [ ] The demo has been tested from its documented initial state.
* [ ] External services, mocks, and safe test credentials are documented where relevant.
* [ ] Known limitations are stated.

### Submission

* [ ] AI usage is disclosed.
* [ ] All submitted material is in English.
* [ ] Everything to be evaluated is committed and pushed to `main`.
* [ ] The final commit SHA has been submitted through the official form.

If those points are true, your repository is ready for evaluation.