# Tag Check Action

GitHub Action that checks the version in the NPM package is not used as a tag.

```yaml

  - name: Check for version tag
    id: check-tag
    uses: clockwork-marketing-uk/actions-tag-check@1.0.0
    with:
        github-token: ${{ secrets.GITHUB_TOKEN }}
        branch-name: ${{ github.event.pull_request.head_branch }}

```

## Updates to the action

- Update the version in the [NPM package](package.json) as this is `NOT` automated in the repository.

- Amend the [Change Log](CHANGELOG.md)

