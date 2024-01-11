# composite-workflow-trigger

[![tests](https://img.shields.io/github/actions/workflow/status/toonvd/workflow-trigger/triggered.yaml?style=for-the-badge&label=tests)](https://github.com/toonvd/workflow-trigger/actions/workflows/triggered.yaml)

## Why?
I decided to make this workflow dispatcher because current workflow mechanics are flawed.

- `workflow_run`:
  - loses `ref` from the third nest on
  - maximum nesting of `4`
- `workflow_call`:
  - does not really trigger the workflow separately:
    - no badges
    - sloppy summary

## Requirements
`bash` and `jq`, `jq` is available by default in a lot of `Linux` runners

## Installation
```yaml 
- name: composite-workflow-trigger        
  uses: toonvd/composite-workflow-trigger@v0.0.2
```
## Usage
Please check the [workflows](https://github.com/toonvd/workflow-trigger/tree/main/.github/workflows).

Summary:
 - the trigger needs the `file` to trigger, the `ref` and the `GITHUB_TOKEN` to [work](https://github.com/toonvd/workflow-trigger/blob/main/.github/workflows/main.yaml#L12)