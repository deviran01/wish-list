# Development

## Environments

```shell
pipenv install
```

## Necessary Packages

- `Django`: ...
- `pytest`: A Python testing framework that provides features such as fixtures, parametrization, plugins, and more. It
  can
  be used to write and run tests for various types of applications and libraries.
- `pytest-html`: A plugin for pytest that generates a HTML report for test results. It supports various options and
  features, such as customizing the report title, output format, and report structure.
- `pytest-xdist`: A plugin for pytest that extends its test execution modes with new ones, such as distributing tests
  across multiple CPUs to speed up test execution or looping on failures until they pass or a certain number of failures
  is reached.
- `assertpy`: A simple assertion library for unit testing in Python with a fluent API. It supports both Python 2 and 3,
  and works best with a python test runner like pytest or Nose. It allows you to write assertions in a concise and
  readable way using methods like assert_that or assert_equal_to.
- `pytest-cov`: A plugin for pytest that integrates coverage.py into the test process. It calculates code coverage
  statistics based on the source code files executed by the tests, and reports them in various formats such as HTML,
  JSON, or XML.
- `python-json-logger`: A Python logging library that emits JSON log messages instead of plain text ones. This can be
  useful for logging infrastructure such as ELK (Elasticsearch Logstash Kibana) or Cloudwatch (AWS) that can easily
  index and search JSON log data.
- `pre-commit`: A framework for managing and maintaining multi-language pre-commit hooks. Pre-commit hooks are scripts
  that run before committing changes to a repository, and can perform tasks such as linting code quality, formatting
  code style, running tests, etc. Pre-commit can help you keep your code consistent and reliable across different
  languages and tools.
- `pylint`: A static code analysis tool for the Python programming language that identifies errors in Python code and
  helps programmers enforce good coding styles according to PEP 8 (the official Python style guide). Pylint can also
  check other aspects of the code quality such as complexity, readability, security issues, etc., depending on the
  configuration options used by the user or by default settings provided by Pylint itself or by other tools such as
  flake8 or black.

```shell
pipenv install Django pytest pytest-html pytest-xdist python-json-logger assertpy
```

## Linter

- `pre-commit`: A multi-language package manager for pre-commit hooks that manages the installation and execution of any
  hook written in any language before every commit³.

### Install

```shell
pipenv install pre-commit
```

### Check Version

```shell
pre-commit --version
```

### Create Simple Config

```shell
pre-commit sample-config
```

#### Recommended Hooks

```text
https://github.com/pre-commit/pre-commit-hooks
https://github.com/Lucas-C/pre-commit-hooks-safety
https://github.com/PyCQA/bandit
pylint
https://github.com/psf/black
https://github.com/pre-commit/mirrors-mypy
```

### Create pylint Config (It's necessary for pre-commit config)

```shell
pylint --generate-rcfile >.pylintrc
```

### Run (Execute)

```shell
pre-commit run
```

## Docker

## Tests
