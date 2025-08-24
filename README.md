# `setup-orbit` action

[![Test](https://github.com/chaseruskin/setup-orbit/actions/workflows/test.yml/badge.svg?branch=trunk)](https://github.com/chaseruskin/setup-orbit/actions/workflows/test.yml)

This GitHub Action will install a release of [Orbit](https://github.com/chaseruskin/orbit), a package manager and build system for VHDL, Verilog, and SystemVerilog.

## Usage

### Examples

In most cases all you will need is the following in your workflow.

```yaml
- uses: chaseruskin/setup-orbit@v0
```

If you want a specific version of Orbit, you can specify this by passing the
`version` input.

```yaml
- uses: chaseruskin/setup-orbit@v0
  with:
    version: '0.26.0'
```

### Inputs

| Name           | Required | Description                                  | Type   | Default               |
| -------------- | -------- | -------------------------------------------- | ------ | --------------------- |
| `version`| no       | A valid semver specifier of the Orbit version to install                | string | null                  |

By default, the latest released version of Orbit will be installed.