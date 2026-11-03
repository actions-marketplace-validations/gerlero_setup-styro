# setup-styro

[![CI](https://github.com/gerlero/setup-styro/actions/workflows/ci.yml/badge.svg)](https://github.com/gerlero/setup-styro/actions/workflows/ci.yml)
[![Release](https://github.com/gerlero/setup-styro/actions/workflows/release.yml/badge.svg)](https://github.com/gerlero/setup-styro/actions/workflows/release.yml)

Installs a specific version of [**styro**](https://github.com/gerlero/styro) in the GitHub Actions environment.

## Usage

```yaml
steps:
- uses: actions/checkout@v7
- uses: gerlero/setup-openfoam@v1
  with:
    openfoam-version: 2606
- uses: gerlero/setup-styro@v1
- run: styro install solids4foam
```

## Inputs

### `styro-version`

Version of **styro** to install. E.g.:

```yaml
- uses: gerlero/setup-styro@v1
  with:
    styro-version: 0.1.39
```

If not specified, the action will install the latest version of **styro**.
