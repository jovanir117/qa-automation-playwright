# qa-automation-playwright

Study project: end-to-end test automation with **Playwright for Python** and pytest. I'm a QA Engineer (manual mobile and POS release testing, ISTQB CTFL) moving into test automation, and this repo is where the work is done in the open.

## Status

| Step | Topic | Status |
|---|---|---|
| 1 | Playwright basics: locators, assertions, auto-wait | in progress |
| 2 | Page Object Model, fixtures, trace viewer, GitHub Actions CI | planned |
| 3 | Same tests in Selenium, with a comparison | planned |
| 4 | Appium: Android mobile flows | planned |
| 5 | Load testing with k6 | planned |

Each step lands as its own commits and ends with something runnable, not just notes.

## Run it

```
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
playwright install chromium
pytest              # headless
pytest --headed     # watch the browser
```

## What's here today

- `tests/test_smoke.py`: two checks against the public Playwright docs site (page title, navigation to the install guide). They confirm the toolchain works; they are not a real test suite yet.
- `pytest.ini`: Chromium by default.

## Stack

Python 3.12, pytest 9, pytest-playwright 0.10 (Playwright 1.64), Chromium.
