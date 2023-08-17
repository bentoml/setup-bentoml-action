## About

Boostrap BentoML and adjacent support tools for running BentoML on CI.

## Usage

```yaml
name: ci
on:
  push:
    branches:
      - 'main'
jobs:
  docker:
    runs-on: ubuntu-latest
    steps:
      - uses: bentoml/setup-bentoml-action@v1
        with:
          python-version: '3.10'
          bentoml-version: 'main'
          cache: 'pip'
```
