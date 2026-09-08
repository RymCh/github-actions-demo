# GitHub Actions CI Demo

Small Python project created to practice Continuous Integration (CI) with GitHub Actions.

## CI workflow

The CI workflow is triggered automatically when a pull request targets the `main` branch.

It runs on an Ubuntu runner and performs the following steps:

- Checks out the repository
- Sets up Python
- Installs the required tools
- Runs unit tests with `pytest`
- Checks code style with `flake8`
- Checks formatting with `black`
- Performs static type checking with `mypy`

## Project structure

- `app.py`: Python code
- `test_app.py`: unit tests
- `.github/workflows/ci.yml`: GitHub Actions CI workflow

## Run tests locally

```bash
python -m pytest
