# what-changes

This action checks for changes of between 2 prs based on Merge Pull Request commit, and returns formatted output

# Usage

See [action.yml](action.yml)

## Basic

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: classfunc/what-changes@v1
    id: 'changes-table'
    with:
      output-type: 'md'
  - name: Print Output
    run: echo "${{ steps.changes-table.outputs.value }}"
```

# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
