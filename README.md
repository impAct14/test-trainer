# Test Trainer

A personal QA/QE training workspace for practicing manual testing, automation testing, CI/CD, and interview preparation.

This repository is used to organize testing practice materials, build automation demo projects, and demonstrate continuous improvement as a QA/QE.

---

## Overview

This workspace focuses on:

- Manual test design
- Test case and bug report writing
- Automation testing with Python and Playwright
- Test framework structure and maintainability
- CI/CD practice with GitHub Actions
- QA/QE interview preparation
- External QA/QE reference materials through Git submodules

---

## Repository Structure

```text
test-trainer/
├── .github/
│   └── workflows/
│       └── ci.yml
├── qe-testing-kit/
├── manual-practice/
├── saucedemo-playwright-python/
├── interview-notes/
├── .gitmodules
└── README.md
```

---

## Main Folders

| Folder | Description |
| --- | --- |
| `.github/workflows/` | GitHub Actions workflows for CI validation |
| `qe-testing-kit/` | External QA/QE reference toolkit added as a Git submodule |
| `manual-practice/` | Manual testing practice materials |
| `saucedemo-playwright-python/` | Planned Playwright Python automation demo project |
| `interview-notes/` | QA/QE interview preparation notes |

---

## CI/CD

This repository uses GitHub Actions for continuous integration.

Current workflow:

| Workflow | Purpose |
| --- | --- |
| `Test Trainer CI` | Validates repository structure and checks submodule checkout |

Current CI checks:

- `.gitmodules` exists
- `qe-testing-kit` submodule is available
- Submodule status can be displayed successfully

Future CI scope:

- Run Playwright Python tests
- Upload screenshots, traces, and reports on failure
- Validate automation project structure on pull requests

---

## Git Submodule

This repository uses `qe-testing-kit` as a Git submodule.

Clone with submodules:

```bash
git clone --recurse-submodules https://github.com/impAct14/test-trainer.git
```

If the repository was cloned without submodules:

```bash
git submodule update --init --recursive
```

Update the submodule:

```bash
git submodule update --remote qe-testing-kit
git add qe-testing-kit
git commit -m "Update qe-testing-kit submodule"
```

---

## Roadmap

### Phase 1: Repository Setup

- [x] Create `test-trainer` repository
- [x] Add `qe-testing-kit` as a Git submodule
- [x] Add basic GitHub Actions CI workflow
- [x] Protect `main` branch
- [x] Add README
- [ ] Add `.gitignore`

### Phase 2: Manual Testing Practice

- [ ] Add test scenarios
- [ ] Add test case samples
- [ ] Add bug report samples
- [ ] Add regression checklist
- [ ] Practice test design techniques
  - Boundary Value Analysis
  - Equivalence Partitioning
  - Decision Table Testing
  - Error Guessing

### Phase 3: Automation Demo Project

- [ ] Create `saucedemo-playwright-python`
- [ ] Set up Python, Pytest, and Playwright
- [ ] Add Page Object Model structure
- [ ] Add login tests
- [ ] Add cart tests
- [ ] Add checkout tests
- [ ] Add negative test cases
- [ ] Add trace and screenshot support

### Phase 4: CI for Automation Tests

- [ ] Add Playwright Python CI workflow
- [ ] Run tests on pull requests
- [ ] Upload test artifacts on failure
- [ ] Document test execution results

---

## Branching Strategy

The `main` branch is protected.

Recommended workflow:

```bash
git checkout main
git pull

git checkout -b feature/example-change
```

After making changes:

```bash
git add .
git commit -m "Add example change"
git push -u origin feature/example-change
```

Then create a Pull Request into `main`.

---

## Tech Stack

Planned and current tools:

- Git
- GitHub
- GitHub Actions
- Python
- Pytest
- Playwright
- Markdown
- Manual test design techniques

---

## Author

An Nguyen  
GitHub: [impAct14](https://github.com/impAct14)
