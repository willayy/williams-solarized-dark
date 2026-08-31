# Repository Guidelines & Release Instructions

## Versioning & Releases

- **Always update `version` in [package.json](file:///Users/williamnorland/Documents/Source-Code/williams-solarized-dark/package.json)** when preparing a new release or publishing updates.
- Use Semantic Versioning (SemVer: `MAJOR.MINOR.PATCH`).
- Ensure the git tag matches the version in [package.json](file:///Users/williamnorland/Documents/Source-Code/williams-solarized-dark/package.json) prefixed with `v` (e.g. `v0.1.1` for version `0.1.1`).
- Pushing a version tag (`v*`) triggers the GitHub Actions workflow in [.github/workflows/publish.yml](file:///Users/williamnorland/Documents/Source-Code/williams-solarized-dark/.github/workflows/publish.yml) to package the extension and create a GitHub Release with the `.vsix` binary asset.
