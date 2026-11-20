# Personal Finance Tracker

v1 and v2 implementations of a finance tracker application for CISC 594: Software Testing Principles and Techniques.

A standalone Python application for recording income and expenses, categorizing spending, and calculating account balances. The architecture prioritizes testability.

> **Current state: v0 baseline.** This code is imported unchanged (apart from this README) from a CISC 593 team project. See [Acknowledgements](#acknowledgements). v1 and v2 are developed in this repository.

## Documentation

- [Design Document](docs/design.md) — architecture, class diagrams, JSON schema, and design decisions

## Setup

### Prerequisites

- Python 3.8 or newer

### Installation

```bash
git clone <repo-url>
cd harrisburg-cisc-594-project
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

On Windows, activate the venv with `.venv\Scripts\activate` instead.

### Running the test suite

With the virtual environment activated:

```bash
# Run all unit tests
make test

# Run all unit tests with verbose output
make test-verbose

# Run tests for a single unit with verbose output
pytest src/domain/test_transaction.py -v
```

### Adding dependencies

With the venv activated:

```bash
pip install <package-name>
pip freeze > requirements.txt
```

Commit `requirements.txt` after adding dependencies.

## Acknowledgements

The v0 baseline (tag `v0.0.0`) was co-developed in CISC 593 (Software Verification & Validation), Harrisburg University, Late Spring 2026, in the repository `mustafa-siddiqui/personal-finance-tracker-project`. The original team:

| Team Member | Role |
|-------------|------|
| Mustafa Siddiqui | Backend Architect & Developer |
| Owais Adil Mohammed | Core Backend Developer |
| Anas Rais Lnu | Security & UI Specialist |
| Mohd Karim Siddiqui | Reporting & Analytics Developer |
