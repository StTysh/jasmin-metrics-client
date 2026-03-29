# jasmin-metrics-client

`jasmin-metrics-client` is a Python package intended to provide a reusable client for working with JASMIN metrics data backed by Elasticsearch-style sources.

## Current status

This repository is currently in an early scaffold stage. The packaging, quality tooling, and documentation structure are in place, but the client surface itself is still minimal and not yet implemented as a full library.

That means this repository is best treated as the foundation for a Python client package rather than a finished SDK.

## Stack

- Python 3.9 to 3.13
- Poetry
- Pydantic Settings
- STAC Pydantic
- Ruff
- Black
- isort
- mypy
- Bandit
- Xenon
- Coverage
- Sphinx

## Repository structure

```text
jasmin_metrics_client/            Package source
jasmin_metrics_client/tests/      Unit tests
docs/                             Documentation sources
pyproject.toml                    Packaging and tool configuration
.pre-commit-config.yaml           Local quality checks
```

## Development setup

### Install dependencies

```bash
poetry install
```

### Install pre-commit hooks

```bash
poetry run pre-commit install
```

## Common commands

```bash
poetry run python -m unittest discover jasmin_metrics_client/tests
poetry run mypy jasmin_metrics_client
poetry run ruff check .
poetry run black --check .
```

## Notes

- The package metadata and tooling are configured, but the library implementation is still skeletal.
- If you continue development here, the next step is to define the actual client API, request models, and metrics query workflows.
