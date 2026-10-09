# Project Brief: Migrating Micro-Finance Tools to Git & GitHub

## Context & Organizational Mission
You have joined a micro-finance startup dedicated to empowering low-income individuals by broadening access to equitable financial services and economic opportunities. 

The engineering team currently manages their codebases using **Apache Subversion (SVN)**. To improve collaboration, enhance developer workflows, and embrace modern open-source standards, the engineering organization has initiated a phased migration to **Git** and **GitHub**.

---

## Objective
As the initial step in this migration, your task is to establish a public, open-source repository on GitHub hosting the organization's reference script for calculating simple interest. 

Beyond simply uploading the code, you must establish an open-source standard for the team by implementing core governance documents, collaboration workflows, and licensing compliance.

---

## Project Requirements

### 1. Repository Setup & Version Control
* Initialize a local Git repository and connect it to a new public GitHub repository.
* Include a clean commit history demonstrating standard Git hygiene (`add`, `commit`, `push`).
* Configure an appropriate `.gitignore` file to ensure build artifacts and temporary files remain uncommitted.

### 2. Core Implementation
Host the reference script implementing the simple interest formula:

$$A = P(1 + rt)$$

Where:
* $P$ = Principal investment or loan balance
* $r$ = Annual interest rate (decimal form)
* $t$ = Time period (in years)
* $A$ = Total accumulated value ($P + I$, where $I = P \cdot r \cdot t$)

The script should accept user inputs, validate numerical boundaries, and print the resulting interest and total balance cleanly.

---

## Supporting Open-Source Documentation

To adhere to open-source software best practices, your repository must contain the following foundational governance files:

| File | Purpose | Key Contents |
| :--- | :--- | :--- |
| `README.md` | Primary landing page & user guide | Project overview, mission statement, prerequisites, installation steps, input/output usage examples, and contribution pointers. |
| `LICENSE` | Legal usage & distribution terms | Full legal text of the **Apache License 2.0**, granting broad usage rights, explicit patent grants, and trademark protection. |
| `CONTRIBUTING.md` | Developer onboarding & standards | Branch naming conventions, pull request procedures, coding standards, issue reporting templates, and testing expectations. |
| `CODE_OF_CONDUCT.md` | Community expectations & safety | Explicit ethical guidelines and enforcement procedures (e.g., standard Contributor Covenant) fostering an inclusive environment. |

---

## Phased Execution Plan

```
Step 1: Local Setup
 └── git init
 └── Add simple_interest script
 └── Add .gitignore

Step 2: Add Governance & Documentation
 ├── Create README.md
 ├── Add Apache 2.0 LICENSE
 ├── Add CONTRIBUTING.md
 └── Add CODE_OF_CONDUCT.md

Step 3: Staging & Committing
 ├── git add .
 └── git commit -m "feat: initial release with open-source governance"

Step 4: GitHub Remote Publication
 ├── git remote add origin <github-repo-url>
 ├── git branch -M main
 └── git push -u origin main
```

---

## Acceptance Criteria
- [ ] Repository is publicly accessible on GitHub.
- [ ] Contains the functional simple interest calculation script.
- [ ] `LICENSE` is explicitly configured with Apache License 2.0.
- [ ] `README.md` documents both the formula and clear step-by-step execution instructions.
- [ ] `CONTRIBUTING.md` outlines standard branch-and-PR contribution flows.
- [ ] `CODE_OF_CONDUCT.md` establishes a safe, professional community standard.
