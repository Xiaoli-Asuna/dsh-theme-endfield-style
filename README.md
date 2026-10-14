# dsh-theme-endfield-style

English | [中文](README.zh.md)

A theme in the style of *Arknights: Endfield* for the [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) web UI.
Unofficial fan work, not affiliated with or endorsed by the game's publisher.


| Light | Dark |
|---|---|
| ![light](assets/screenshot-light.png) | ![dark](assets/screenshot-dark.png) |

## What it changes

- Fluorescent-yellow sidebar header and a signal rail on the right edge.
- A masthead with a large `DEEPFIELD` background word and procedurally drawn contour lines.
- Engineering grey-white and graphite-black palettes that follow the built-in light / dark / system setting.
- Small corner radii, thin lines, and a shortcut to the built-in Appearance settings in the sidebar.

All artwork is generated in code. There are no image files from the game, no network requests, and no animation loop.

## Install

```sh
dsh plugin --profile web add dsh-theme-endfield-style
```

Or install it from the Themes tab of [dsh-market](https://github.com/dsh-market/dsh-market). Refresh the page afterwards.

If the package is not on npm yet, install from GitHub:

```sh
dsh plugin --profile web add github:Xiaoli-Asuna/dsh-theme-endfield-style
```

## Uninstall

```sh
dsh plugin --profile web remove dsh-theme-endfield-style
```

The theme only adds a `<style>` tag, a few decorative elements, and a `data-endfield-theme` attribute on `<html>`. Removing the plugin removes all of them.

## Compatibility

Selectors use DSH's hashed component class names (for example `.hHd-Xa_root`). They were verified against DSH `0.1.5-rc.3`. A newer DSH may rename them, and parts of the theme may stop applying until the selectors are updated. Please open an issue with your DSH version if that happens.

## Build

```sh
npm install
npm run build   # regenerates lib/client.js from src/client.ts and src/styles.css
```

## License

MIT. The theme is a visual homage; "Arknights: Endfield" and related names belong to their respective owners.