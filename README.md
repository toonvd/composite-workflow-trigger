# Workflow-Trigger
[![tests](https://img.shields.io/github/actions/workflow/status/toonvd/workflow-trigger/triggered.yaml?style=for-the-badge&label=tests)]([https://github.com/toonvd/workflow-trigger/actions/workflows/triggered.yaml](https://github.com/toonvd/workflow-trigger/actions/workflows/triggered.yaml)https://github.com/toonvd/workflow-trigger/actions/workflows/triggered.yaml)

Triggers a workflow using the API because the current workflow_run / workflow_call system is flawed:

- workflow_run: loses ref from the third nest on
- workflow_call: does not really trigger the workflow separately, no badges, bad overview etc.

Usage is at your own risk.