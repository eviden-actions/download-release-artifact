# download-release-artifact

GitHub Action that downloads an artifact from a GitHub release (public or private)

[![Release](https://github.com/ATOS-Actions/download-release-artifact/actions/workflows/release.yml/badge.svg)](https://github.com/ATOS-Actions/download-release-artifact/actions/workflows/release.yml)

## Prerequisites

This action depends on `jq` and `curl` being installed.

## Usage

```
steps:
- uses: ATOS-Actions/download-release-artifact@v1
with:
    name: 'my-artifact-1.0.0.tgz'
    path: './artifacts'
    tag: 'v1.0.0'
```

### Inputs

|  Input  |                       Description                        | Required |
| :-----: | :------------------------------------------------------: | :------: |
| `name`  |                 The name of the artifact                 |   Yes    |
| `path`  |                  The destination folder                  |    No    |
|  `tag`  |                  The tag of the release                  |   Yes    |
| `token` | The Github token. If not provided it uses `GITHUB_TOKEN` |    No    |
