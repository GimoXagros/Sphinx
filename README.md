# Sphinx V0.4.6

Bandai WonderSwan(Color/Crystal) System On a Chip emulator for GBA/NDS.

## This fork and integration

This repository is the GimoXagros fork of [FluBBaOfWard/Sphinx](https://github.com/FluBBaOfWard/Sphinx). `V0.4.6` is the core version in `Version.h`. This fork supplies source code rather than a standalone application and has no GitHub Release binaries.

The custom [NitroSwan](https://github.com/GimoXagros/NitroSwan) build pins `source/Sphinx` to a specific commit, which can differ from this repository's `main`. For a published build, use its release tag and recursive submodule checkout, as described in the [development guide](https://github.com/GimoXagros/NitroSwan/blob/main/Docs/DevelopmentGuide.md). Retain the alignment and reset requirements below when integrating the core.

Make sure RAM is aligned to 16 bytes, the sound mixer is dependant on this.
After reset also call wsvSetCartOk.

## Projects that use this code

* <https://github.com/FluBBaOfWard/NitroSwan>
* <https://github.com/FluBBaOfWard/SwanGBA>

## Credits

Fredrik Ahlström

<https://bsky.app/profile/therealflubba.bsky.social>

<https://www.github.com/FluBBaOfWard>

X/Twitter @TheRealFluBBa
