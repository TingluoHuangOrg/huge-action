# huge-action

A hello-world style GitHub Action that is intentionally large (~100MB) for testing purposes.

## Usage

```yaml
- uses: TingluoHuangOrg/huge-action@main
  with:
    name: 'GitHub'
```

### Inputs

| Name   | Description   | Required | Default |
|--------|---------------|----------|---------|
| `name` | Who to greet  | No       | `World` |

### Outputs

| Name       | Description          |
|------------|----------------------|
| `greeting` | The greeting message |

## Why is this repo so large?

This repository contains ~100MB of random binary data (`data/*.bin`) tracked via
Git LFS. The large size is intentional and is used for testing scenarios that
involve downloading or caching large GitHub Actions.