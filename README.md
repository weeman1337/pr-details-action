# pr-details-action
A Github Action for finding details about a PR relating to the workflow run

## Example for running from a `workflow_run` reacting to a `pull_request` workflow.

```yaml
steps:
  - id: details
    uses: matrix-org/pr-details-action@v1
    with:
      owner: ${{ github.event.workflow_run.head_repository.owner.login }}
      branch: ${{ github.event.workflow_run.head_branch }}
```
