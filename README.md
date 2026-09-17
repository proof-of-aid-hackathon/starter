# Proof of Aid Hackathon

> **Design the complete system. Build one meaningful part in depth.**

This repository is your team's official Hackathon workspace.

It has been created for your team by the organizers from the official Proof of Aid starter repository. During the Hackathon, you will use it to design your solution, build your prototype, document your work, and submit the exact versions to be evaluated.

All submitted work, documentation, demos, and the final pitch must be in **English**.

---

## At a glance

| Question                                            | Answer                                                                                                                |
| --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| **What are we solving?**                            | A concrete problem within Proof of Aid.                                                                               |
| **Do we need to build the whole system?**           | **No.** Design the complete system, but implement one meaningful part in depth.                                       |
| **Do we have to use blockchain?**                   | **No.** Use it only where it provides meaningful value.                                                               |
| **Can we choose our own approach?**                 | Yes. Your problem focus, architecture, technologies, and implementation scope are open.                               |
| **Are there mandatory tracks?**                     | No. The contribution areas below are prompts, not tracks.                                                             |
| **Where does our code go?**                         | `implementation/`                                                                                                     |
| **Where do we explain the project?**                | `SUBMISSION.md`                                                                                                       |
| **How do we submit a checkpoint or final version?** | Push the state to `main` and submit the corresponding **commit SHA** through the official submission form.            |
| **What should we do first?**                        | Understand the problem, choose a concrete focus, sketch the complete system, and decide what you will actually build. |

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

The challenge is to make some part of that process more **understandable, trustworthy, verifiable, or usable**.

That does not automatically mean putting everything on-chain.

Your solution may involve interfaces, conventional software, APIs, identity, payments, evidence, external systems, data processing, blockchain, or any combination that you can justify.

---

# 2. The challenge

All teams work on the same broad problem: **Proof of Aid**.

Your team should:

1. choose a concrete problem worth solving;
2. design how the complete solution would work;
3. choose one meaningful part of that system;
4. implement that part in enough depth to demonstrate it;
5. explain the important decisions and trade-offs;
6. show it working through a concrete scenario.

> **Depth matters more than feature count.**

Your implemented contribution does not need to cover the complete lifecycle.

It should demonstrate one important claim of your proposed solution.

---

# 3. Contribution areas

These areas are **lenses for exploring the problem, not mandatory tracks**.

You may focus on one, combine several, or address another relevant Proof of Aid problem.

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

Describe where your implementation effort is concentrated across three dimensions:

| Dimension                 | Includes                                                                                                                                |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
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

* describe where your team concentrated its implementation effort;
* are not scores;
* have no ideal distribution;
* should approximately sum to 100%.

A project is not stronger simply because it uses more blockchain.

---

# 5. Your GitHub workspace

## Your team repository

The organizers will assign your team a private repository inside the official Hackathon GitHub Organization.

Conceptually:

```text
<official-hackathon-organization>/team-07
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

## Step 2 — Choose a concrete problem

Before coding, make sure your team can complete this sentence:

> We are addressing **[specific problem]** for **[actor or context]** by **[proposed approach]**.

This can evolve during the Hackathon.

Its purpose is simply to ensure that you are solving something concrete.

---

## Step 3 — Sketch the complete system

Open [`SUBMISSION.md`](./SUBMISSION.md).

Start describing:

* the problem;
* the proposed solution;
* the end-to-end flow;
* the architecture;
* what would exist in the complete system.

Do not wait until Friday to write this.

Treat `SUBMISSION.md` as a **living design document** that evolves together with the implementation.

---

## Step 4 — Decide what you will actually build

Choose one meaningful part of the system and implement it under:

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

## Step 5 — Keep design and reality separate

Throughout `SUBMISSION.md`, distinguish clearly between:

| Status                 | Meaning                                                                           |
| ---------------------- | --------------------------------------------------------------------------------- |
| **Implemented**        | Working code or another demonstrable technical artifact exists in the repository. |
| **Simulated / mocked** | A real component has been replaced or simplified for the prototype.               |
| **Designed only**      | It belongs to the complete proposed system but was not implemented.               |
| **Out of scope**       | It is deliberately excluded from the Hackathon scope.                             |

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

Your final repository must contain:

## `SUBMISSION.md`

A concise explanation of:

* the problem;
* the proposed complete system;
* what you actually built;
* important decisions and trade-offs;
* implementation scope;
* demo and validation;
* limitations;
* AI usage.

## `implementation/`

The technical contribution actually built during the Hackathon.

## `implementation/README.md`

Enough information for another technical person to:

* understand what is there;
* install it;
* configure it;
* run it;
* validate it;
* reproduce the demo.

## A submitted commit SHA

Checkpoints and final submissions are identified by an exact Git commit.

The commit SHA — not the current state of `main` at some later time — defines the submitted version.

---

# 9. Demo expectations

Your demo should prove one concrete thing about your contribution.

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

> An organisation creates an aid claim, a verifier attaches evidence, and the system exposes the resulting verification state.

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

Before the deadline:

1. update `SUBMISSION.md` with your current direction;
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

The final submission works in the same way.

Before the deadline:

1. complete `SUBMISSION.md`;
2. finalize the implementation;
3. test the documented setup and demo;
4. merge any work you want evaluated into `main`;
5. make sure all required files are committed;
6. push `main`;
7. obtain the exact commit SHA;
8. submit your **Team ID + final commit SHA** through the official form.

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

# 13. Evaluation

[ORGANIZERS: INSERT FINAL APPROVED EVALUATION RUBRIC]

The rubric published here before the Hackathon will be the participant-facing evaluation reference.

---

# 14. Schedule

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

# 15. Resources

## Must read

* [ORGANIZERS: ADD CORE PROOF OF AID REFERENCE]

## Recommended

* [ORGANIZERS: ADD RECOMMENDED RESOURCES]

## Optional deep dives

* [ORGANIZERS: ADD OPTIONAL TECHNICAL OR DOMAIN RESOURCES]

You do not need to read every optional resource before starting.

---

# 16. Before submitting

Your submission is ready when:

* [ ] The problem can be understood quickly.
* [ ] The complete proposed system is explained.
* [ ] The implemented contribution is obvious.
* [ ] Implemented, simulated, designed-only, and out-of-scope components are clearly distinguished.
* [ ] Important decisions and trade-offs are explained.
* [ ] The code is under `implementation/`.
* [ ] `implementation/README.md` contains working run instructions.
* [ ] The demo has been tested from its documented initial state.
* [ ] External services, mocks, and safe test credentials are documented where relevant.
* [ ] Known limitations are stated.
* [ ] AI usage is disclosed.
* [ ] All submitted material is in English.
* [ ] Everything to be evaluated is committed and pushed to `main`.
* [ ] The final commit SHA has been submitted through the official form.

If those points are true, your repository is ready for evaluation.