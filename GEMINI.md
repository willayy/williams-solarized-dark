# Repository Guidelines & Release Instructions

## Versioning & Releases

- **Always update `version` in [package.json](file:///Users/williamnorland/Documents/Source-Code/williams-solarized-dark/package.json)** when preparing a new release or publishing updates.
- Use Semantic Versioning (SemVer: `MAJOR.MINOR.PATCH`).
- Ensure the git tag matches the version in [package.json](file:///Users/williamnorland/Documents/Source-Code/williams-solarized-dark/package.json) prefixed with `v` (e.g. `v0.1.1` for version `0.1.1`).
- Pushing a version tag (`v*`) triggers the GitHub Actions workflow in [.github/workflows/publish.yml](file:///Users/williamnorland/Documents/Source-Code/williams-solarized-dark/.github/workflows/publish.yml) to package the extension and create a GitHub Release with the `.vsix` binary asset.

## Theme Palette Consistency

All application themes (`themes/vscode/`, `themes/antigravity/`, `themes/ghostty/`, and `plugin.json`)
must maintain identical color palettes:

- **Background**: `#002B36` (Solarized base03)
- **Foreground / Text**: `#839496` (Solarized base0)
- **Primary / Button**: `#268BD2` (Solarized blue) with `#FFFFFF` text
- **Cursor**: `#D30102` (custom red accent)
- **Selection**: `#244952`
- **Comments**: `#62C262` (custom bright green)
- **Numbers / Constants**: `#2AA198` (Solarized cyan)
- **Strings**: `#2AA198` (Solarized cyan)
- **Keywords**: `#859900` (Solarized green)
- **Functions**: `#268BD2` (Solarized blue)
- **Classes / Types**: `#FF9900` (custom amber)
- **Regex / Errors**: `#C70000` (custom deep red)
- **Punctuation**: `#FFFFFF`

When modifying any color in one application theme, always propagate the update across all other
application themes simultaneously.
