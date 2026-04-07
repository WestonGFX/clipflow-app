# ClipFlow

<div align="center">
  <img src="docs/screenshots/main-ready/desktop-hero-carbonfox-kanagawa.png" width="760" alt="ClipFlow desktop hero showing the main window and tray workflow on macOS" />
</div>

<div align="center">
  <img src="public/logo4.png" width="120" alt="ClipFlow logo" />
  <h2>Fast Clipboard Recall For macOS</h2>
  <p>
    ClipFlow is a dense, local-first clipboard manager for people who want fast search,
    tray-first utility, and a serious desktop workflow instead of a bloated dashboard.
  </p>
</div>

## Why ClipFlow

ClipFlow is built around a few simple ideas:

- local-first history instead of cloud dependency
- fast recall instead of ornamental UI
- one main window for depth and one tray surface for speed
- practical privacy, diagnostics, and recovery controls

It is designed to feel like a real Mac utility you can trust all day, not a novelty layer on top of your clipboard.

## Beta Download

The latest beta builds live in:

- [Releases](https://github.com/WestonGFX/clipflow-app/releases)

For most people, the right download is:

- the `.dmg`

Use the zipped `.app` only as a fallback if the DMG route gives you trouble.

Install notes, trust caveats, upgrade guidance, and migration steps live in:

- [docs/install-and-upgrade.md](docs/install-and-upgrade.md)
- [docs/release-assets.md](docs/release-assets.md)

If the current beta build is not yet Developer ID signed and notarized, the install guide includes the local-open workaround and explains what that means.

## Product Gallery

### Density Range

<table>
  <tr>
    <td align="center" width="33.3%">
      <strong>Comfortable · Dawnfox</strong><br />
      <img src="docs/screenshots/main-ready/main-light-comfortable-dawnfox.png" width="280" alt="ClipFlow main window in Dawnfox with comfortable density" />
    </td>
    <td align="center" width="33.3%">
      <strong>Default · Kanagawa Dragon</strong><br />
      <img src="docs/screenshots/main-ready/main-dark-default-kanagawa-dragon.png" width="280" alt="ClipFlow main window in Kanagawa Dragon with default density" />
    </td>
    <td align="center" width="33.3%">
      <strong>Dense · Carbonfox</strong><br />
      <img src="docs/screenshots/main-ready/main-dark-dense-carbonfox.png" width="280" alt="ClipFlow main window in Carbonfox with dense density" />
    </td>
  </tr>
</table>

### More Surfaces

<table>
  <tr>
    <td align="center" width="50%">
      <strong>Tray · Night Owl</strong><br />
      <img src="docs/screenshots/main-ready/tray-dark-night-owl.png" width="220" alt="ClipFlow tray window in Night Owl" />
    </td>
    <td align="center" width="50%">
      <strong>Settings · Kanagawa Dragon</strong><br />
      <img src="docs/screenshots/main-ready/settings-dark-kanagawa-dragon.png" width="320" alt="ClipFlow settings view in Kanagawa Dragon" />
    </td>
  </tr>
</table>

## What The Beta Already Covers

- fast local search over clipboard history
- tray workflow and quick recall
- dense main window with multiple density modes
- pins, favorites, snippets, tags, and filtering
- diagnostics, recovery, export, and reset tooling
- local-only storage in the app support directory

## Planned Next

The public roadmap stays intentionally short. Detailed feature planning stays in the private development repo, but these are the current highest-priority future directions:

1. Stronger importers so switching from other clipboard tools feels less painful.
2. More useful transforms that clean up copied text without silently rewriting history.
3. Better local smart actions for links, dates, code, and reusable snippets.
4. Auto-update once signing and notarization are fully stable.
5. A future Windows version after the Mac app is stronger and the parity path is clear.
6. Smarter local-only retrieval features only if they can stay fast, private, and trustworthy.

If you want to influence the order, use feature requests and roadmap feedback issues in this repo rather than treating the README as a live poll.

- [Roadmap feedback and voting thread](https://github.com/WestonGFX/clipflow-app/issues/1)

## Feedback

Use GitHub Issues in this repo for:

- beta bugs
- install or trust problems
- feature requests
- screenshot and UX feedback

Start here:

- [Report a bug](https://github.com/WestonGFX/clipflow-app/issues/new?template=bug_report.yml)
- [Report an install or trust problem](https://github.com/WestonGFX/clipflow-app/issues/new?template=install_trust_issue.yml)
- [Request a feature](https://github.com/WestonGFX/clipflow-app/issues/new?template=feature_request.yml)
- [Share screenshot or UX feedback](https://github.com/WestonGFX/clipflow-app/issues/new?template=screenshot_ux_feedback.yml)

## Source And Development

This public repo is the beta/download surface. The private source repo remains separate.

If you are reviewing ClipFlow as a product, use this repo.
If you have direct access to the private engineering repo, use that one for code, release engineering, and implementation details.
