# scoop-bucket

A [Scoop](https://scoop.sh) bucket for [gistui](https://github.com/akunzai/gistui) — a terminal UI for managing GitHub Gists.

## Install

```powershell
scoop bucket add akunzai https://github.com/akunzai/scoop-bucket
scoop install gistui
```

`gistui` shells out to the [GitHub CLI](https://cli.github.com) (`gh`) at runtime; Scoop
installs it automatically as a dependency. Run `gh auth login` once before using gistui.

## Update

```powershell
scoop update gistui
```

## Maintenance

Manifests track upstream releases automatically through `checkver` / `autoupdate`, driven by
the scheduled [Excavator](.github/workflows/excavator.yml) workflow. The
[CI](.github/workflows/ci.yml) workflow validates the manifest JSON on every change.
