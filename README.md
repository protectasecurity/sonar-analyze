# Sonar Analyze GitHub Actions

Sonar Analyze GitHub Actions allows you to run SonarQube Analyze

## Example usage

```yaml
on: [push]

env:
  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: protectasecurity/sonar-analyze@v1
```

## Environment

- `GITHUB_TOKEN` **Required**
- `SONAR_TOKEN` **Required**

## Authors

- [Ronnie Ayala](https://github.com/ronnieacs)