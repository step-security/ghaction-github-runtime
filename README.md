[![GitHub release](https://img.shields.io/github/release/step-security/ghaction-github-runtime.svg?style=flat-square)](https://github.com/step-security/ghaction-github-runtime/releases/latest)
[![GitHub marketplace](https://img.shields.io/badge/marketplace-github--runtime-blue?logo=github&style=flat-square)](https://github.com/marketplace/actions/github-runtime)

## About

GitHub Action to expose GitHub runtime to the workflow

___

* [Usage](#usage)
* [License](#license)

## Usage

```yaml
name: build

on:
  push:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      -
        name: Expose GitHub Runtime
        uses: step-security/ghaction-github-runtime@v3
      -
        name: Env
        run: |
          # ACTIONS_RUNTIME_TOKEN, ACTIONS_RUNTIME_URL should be exposed
          env|sort
```

## License

MIT. See `LICENSE` for more details.
