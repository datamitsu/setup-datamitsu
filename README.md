# setup-datamitsu

GitHub Action that installs the [datamitsu](https://github.com/datamitsu/datamitsu)
CLI and runs it in CI.

> **This repository is auto-generated — do not edit by hand.**
> The action is built and published automatically from
> [`datamitsu/datamitsu`](https://github.com/datamitsu/datamitsu) (the
> `packaging/action` package) on every datamitsu release. Files committed here
> are overwritten on each publish. Open issues and pull requests in the
> [main repository](https://github.com/datamitsu/datamitsu/issues).

## Status

🚧 **Not yet released.** The first published version will appear here
automatically as an immutable tag (`vX.Y.Z`) matching the datamitsu CLI version
it installs.

## Usage (planned)

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: datamitsu/setup-datamitsu@v0.1.5 # installs datamitsu 0.1.5 (hashes baked in) and runs `datamitsu lint`
```

Each release tag pins one datamitsu version together with the SHA-256 hashes of
its release binaries, so a pinned tag is fully reproducible and integrity is
verified on download. Pin by full version or commit SHA (not a moving major tag)
and let Dependabot keep it current.

### Inputs (planned)

| Input  | Default | Description                                                                          |
| ------ | ------- | ------------------------------------------------------------------------------------ |
| `args` | `lint`  | Arguments passed to `datamitsu`. An empty string installs and initializes only (runs nothing). |

The action carries no configuration of its own: it reads the datamitsu config
already present in your repository.

## License

[MIT](LICENSE)
