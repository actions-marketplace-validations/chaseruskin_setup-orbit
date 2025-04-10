# `setup-orbit` action

[![Test](https://github.com/chaseruskin/setup-orbit/actions/workflows/test.yml/badge.svg?branch=trunk)](https://github.com/chaseruskin/setup-orbit/actions/workflows/test.yml)

This GitHub Action will install a release of [Orbit](https://github.com/chaseruskin/orbit), an agile package manager and extensible build tool for hardware description languages (HDLs).

## Usage

### Examples

In most cases all you will need is the following in your workflow.

```yaml
- uses: chaseruskin/setup-orbit@v0
```

If you want a specific version of `orbit`, you can specify this by passing the
`orbit-version` input.

```yaml
- uses: chaseruskin/setup-orbit@v0
  with:
    orbit-version: '0.24.0'
```

### Inputs

| Name           | Required | Description                                  | Type   | Default               |
| -------------- | -------- | -------------------------------------------- | ------ | --------------------- |
| `orbit-version`| no       | A valid semver specification.                | string | null                  |

By default, the latest version of `orbit` will be installed.