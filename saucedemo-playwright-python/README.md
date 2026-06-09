# SauceDemo Playwright Python

This project is a QA/QE portfolio automation demo for the SauceDemo web application:
https://www.saucedemo.com/

## Tech Stack

- Python
- Pytest
- Playwright
- pytest-playwright
- Page Object Model

## Folder Structure

```text
saucedemo-playwright-python/
├── pages/
│   ├── __init__.py
│   ├── login_page.py
│   ├── inventory_page.py
│   ├── cart_page.py
│   └── checkout_page.py
├── tests/
│   ├── __init__.py
│   ├── test_login.py
│   ├── test_cart.py
│   └── test_checkout.py
├── data/
│   ├── __init__.py
│   └── users.py
├── utils/
│   ├── __init__.py
│   └── config.py
├── pytest.ini
├── requirements.txt
└── README.md
```

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
playwright install
```

On Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
playwright install
```

## Run Tests

```bash
pytest
```

## Current Status

Scaffold only. Page object implementations and test assertions are pending.
