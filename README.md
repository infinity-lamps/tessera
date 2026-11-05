# Tessera infinity lamps

*A piece of the galaxy, in a box.*

This is the public home of the Tessera infinity lamp: the firmware updates the
lamps install themselves, the user guides, and the 3D print files for
replacement parts.

Code is MIT licensed. Documentation and 3D models are CC BY-SA 4.0.

**Start here: [infinity-lamps.github.io/tessera](https://infinity-lamps.github.io/tessera/)**

---

## What is in this repository

| Where | What it holds |
|---|---|
| [`guides/`](guides/) | User guides. Each one reads online as a `.md` file and comes as a `.pdf` to print |
| [`3d-print-files/`](3d-print-files/) | STEP files for printing replacement parts, one folder per lamp, with print settings in its [README](3d-print-files/README.md) |
| [Releases](https://github.com/infinity-lamps/tessera/releases) | Every firmware version, with checksums |
| `gh-pages` branch | The website above, and the files the lamps check for updates |

The firmware is published here as ready-built releases.

## Installing the firmware on a new board

Open the [website](https://infinity-lamps.github.io/tessera/#install) in
Chrome, Edge, Opera or Brave on a desktop computer, plug the board in with a
USB data cable, and press **Connect and install**. Nothing else needs
installing.

## Updating a lamp

Lamps on your WiFi check for updates themselves. To check by hand, open the
lamp's page, then **Advanced settings**, **Firmware and updates**, **Check for
updates**. Your settings, palettes and custom effects are kept.

The address every lamp reads for updates, and which does not change:

```
https://infinity-lamps.github.io/tessera/firmware/manifest.json
```

No internet on the lamp? Download the two `.bin` files from
[Releases](https://github.com/infinity-lamps/tessera/releases) and upload them
under **Firmware and updates**. Check them against the release's `SHA256SUMS`
first if you want to be sure they arrived intact.

## Guides

| Guide | For |
|---|---|
| Quick Start | Every lamp: from plugging it in to controlling it from your phone |
| User Guide | Every lamp: every control, and what to try when something looks wrong |
| Kit Build Guide | Kit builders: frame, wiring, panels and first power-up |

Guides appear in [`guides/`](guides/) as they are published. The
[website](https://infinity-lamps.github.io/tessera/#guides) shows which are
ready.

## Printing a replacement part

Find the folder for your lamp's edge length and shape in
[`3d-print-files/`](3d-print-files/), and read its
[print settings](3d-print-files/README.md) first. Print one of each part and
check the fit before printing a full set.

## Licences

- **Firmware and other code:** [MIT](LICENSE).
- **Guides, images and 3D print files:** [CC BY-SA 4.0](LICENSE-CONTENT). You
  can share and adapt them, with credit, under the same terms.

## Problems and questions

[Open an issue](https://github.com/infinity-lamps/tessera/issues) and say
which lamp you have (the edge length and shape from the label underneath) and
which firmware version it runs (shown under **Firmware and updates**).

---

Made by Ryan in Scotland.
