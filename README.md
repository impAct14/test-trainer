\# Test Trainer



A personal QA/QE training workspace for improving manual testing, automation testing, CI/CD practice, and interview preparation.



This repository is designed to help me practice real QA workflows, organize testing materials, build automation demo projects, and demonstrate continuous learning while applying for QA/QE positions.



\## Purpose



The main goals of this repository are:



\* Practice manual test design and test case writing

\* Build automation testing projects using Python and Playwright

\* Improve test framework structure and maintainability

\* Practice CI/CD setup with GitHub Actions

\* Organize QA/QE interview preparation notes

\* Use external QA/QE reference materials as a submodule



\## Repository Structure



```text

test-trainer/

├── .github/

│   └── workflows/

│       └── ci.yml

│

├── qe-testing-kit/

│

├── manual-practice/

│

├── saucedemo-playwright-python/

│

├── interview-notes/

│

├── .gitmodules

└── README.md

```



\## Folder Overview



\### `.github/workflows/`



Contains GitHub Actions workflow files for CI validation.



Current workflow:



\* `ci.yml`: validates repository structure and checks that the `qe-testing-kit` submodule can be loaded correctly.



\### `qe-testing-kit/`



External QA/QE reference toolkit added as a Git submodule.



This folder is used as a reference for:



\* QA workflow improvement

\* Manual testing support

\* Automation testing ideas

\* Test planning

\* Prompt templates

\* Test case generation

\* Flaky test analysis

\* Automation review checklist



This folder should generally be treated as an external reference, not as the main project workspace.



\### `manual-practice/`



Planned folder for manual testing practice materials, such as:



\* Test scenarios

\* Test cases

\* Bug report samples

\* Regression checklist

\* Exploratory testing notes

\* Test design technique practice



\### `saucedemo-playwright-python/`



Planned automation demo project using:



\* Python

\* Pytest

\* Playwright

\* Page Object Model

\* Reusable locators

\* Test data management

\* Trace, screenshot, and report support



The target demo application will be SauceDemo.



Planned test scope:



\* Login

\* Invalid login

\* Product listing

\* Add to cart

\* Remove from cart

\* Checkout

\* Form validation

\* Logout



\### `interview-notes/`



Planned folder for QA/QE interview preparation, including:



\* Self-introduction

\* Project explanation

\* Manual testing questions

\* Automation testing questions

\* CI/CD explanation

\* Flaky test handling

\* Bug handling under deadline

\* English interview answers



\## CI/CD



This repository uses GitHub Actions for continuous integration.



Current CI workflow:



```text

Test Trainer CI

```



The workflow currently checks:



\* Repository structure

\* `.gitmodules` existence

\* `qe-testing-kit` submodule checkout

\* Submodule status



Future CI workflow will run Playwright Python automation tests when the `saucedemo-playwright-python` project is added.



\## Git Submodule



This repository uses `qe-testing-kit` as a Git submodule.



\### Clone this repository with submodules



```bash

git clone --recurse-submodules https://github.com/impAct14/test-trainer.git

```



\### If cloned without submodules



```bash

git submodule update --init --recursive

```



\### Update submodule to latest remote version



```bash

git submodule update --remote qe-testing-kit

git add qe-testing-kit

git commit -m "Update qe-testing-kit submodule"

```



\## Planned Roadmap



\### Phase 1: Repository Setup



\* \[x] Create `test-trainer` repository

\* \[x] Add `qe-testing-kit` as a Git submodule

\* \[x] Add basic GitHub Actions CI workflow

\* \[x] Protect main branch

\* \[ ] Add complete README

\* \[ ] Add `.gitignore`



\### Phase 2: Manual Testing Practice



\* \[ ] Create manual test scenario examples

\* \[ ] Create test case samples

\* \[ ] Create bug report samples

\* \[ ] Create regression checklist

\* \[ ] Practice test design techniques:



&#x20; \* Boundary Value Analysis

&#x20; \* Equivalence Partitioning

&#x20; \* Decision Table Testing

&#x20; \* Error Guessing



\### Phase 3: Automation Demo Project



\* \[ ] Create `saucedemo-playwright-python`

\* \[ ] Set up Python, Pytest, and Playwright

\* \[ ] Create Page Object Model structure

\* \[ ] Add login tests

\* \[ ] Add cart tests

\* \[ ] Add checkout tests

\* \[ ] Add negative test cases

\* \[ ] Add trace/screenshot support

\* \[ ] Add test report support



\### Phase 4: CI for Automation Tests



\* \[ ] Add GitHub Actions workflow for Playwright Python tests

\* \[ ] Run tests on pull requests

\* \[ ] Upload test artifacts on failure

\* \[ ] Document CI result and test execution



\## Branching Strategy



The `main` branch is protected.



Recommended workflow:



```bash

git checkout main

git pull



git checkout -b feature/add-new-content

```



After making changes:



```bash

git add .

git commit -m "Add new content"

git push -u origin feature/add-new-content

```



Then create a Pull Request from the feature branch into `main`.



\## Why This Repository Exists



This repository is part of my continuous improvement plan as a QA/QE.



It helps me practice not only automation coding, but also the complete testing mindset:



\* Understanding requirements

\* Designing test scenarios

\* Writing clear test cases

\* Identifying regression risks

\* Reporting bugs effectively

\* Choosing good automation candidates

\* Building maintainable automation frameworks

\* Running tests in CI/CD

\* Explaining testing decisions clearly in interviews



\## Tech Stack



Current and planned tools:



\* Git

\* GitHub

\* GitHub Actions

\* Python

\* Pytest

\* Playwright

\* Markdown

\* Manual test design techniques

\* QA/QE reference toolkit



\## Author



An Nguyen

GitHub: \[impAct14](https://github.com/impAct14)



