[![Create Release][release-badge]][release-url]
[![Import Labels][import-labels-badge]][import-labels-url]
[![Sync Labels][sync-labels-badge]][sync-labels-url]
[![PR AutoLabeler][autolabeler-badge]][autolabeler-url]
[![Assigner][assigner-badge]][assigner-url]

Description

### Inputs
#### `pullRequestNumber`
PR number for commenting
Required.
Default: `${{ github.event.pull_request.number }}`

#### `ignore`
comma-separated list of packages names to ignore
Default: ""

#### `root`
rootDir to search package.json files
Default: `.`

#### `commentWhenClean`
Whether or not to comment when there are no deprecations
Default: `false`


### Example usage
```yaml
      - name: Check for deprecated packages
        uses: CumulusDS/deprecated-packages-action@v1
        with:
          commentWhenClean: true
```



[release-badge]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/release.yml/badge.svg
[release-url]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/release.yml
[import-labels-badge]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/labels_import.yml/badge.svg
[import-labels-url]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/labels_import.yml
[sync-labels-badge]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/labels_sync.yml/badge.svg
[sync-labels-url]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/labels_sync.yml
[autolabeler-badge]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/autolabeler.yml/badge.svg
[autolabeler-url]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/autolabeler.yml
[assigner-badge]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/assign.yml/badge.svg
[assigner-url]: https://github.com/CumulusDS/deprecated-packages-action/actions/workflows/assign.yml
