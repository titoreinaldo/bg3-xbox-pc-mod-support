# BG3 Mod Support for the Xbox App on PC

**Experimental package 0.2.3 · Microsoft package 1.8.907.0+ / engine build 7445165+**

Download the player package and complete corresponding source from the [0.2.3 release](https://github.com/titoreinaldo/bg3-xbox-pc-mod-support/releases/tag/v0.2.3). This release replaces the exact-version checks with minimum-version checks in the manager and Script Extender. The maintainer confirmed a successful game launch on Microsoft package 1.8.910.0 on 3 October 2026.

## Installation

1. Launch BG3 once through the Xbox app, open its in-game Mod Manager, then quit.
2. Extract **BG3-Xbox-Mod-Manager-0.2.3.zip** to a writable folder outside the game.
3. Open **App/BG3ModManager.exe**, then click **Set up**. Leave MCM checked to include it.
4. Launch BG3 normally. Look for **Script Extender v33 loaded** and **Mod Configuration Menu** in the main menu.

Keep the App files together and keep existing setup backups. If the game already has a setup record, preserve that record rather than replacing it with a fresh installation. The manager window still identifies experimental build 0.2.0; the package is 0.2.3.

To add mods, close BG3, choose **File > Import Mod**, move the desired mods to Active, and **Export Order to Game**. Preserve existing mods and follow each author's dependencies and load order.

## What it does

An unofficial Xbox compatibility build of BG3 Mod Manager, with a **Set up** button for the compatible Script Extender and optional Mod Configuration Menu (MCM). It detects the game and Xbox profile, preserves other mods and settings, and creates backups. **Undo setup** refuses to overwrite later changes. No commands or global .NET installation are required.

## Validation and limitations

Both changed components compiled successfully. The maintainer confirmed the game launches correctly on Microsoft package **1.8.910.0**. No additional automated tests or gameplay/save-load tests were run for 0.2.3. Accepting a newer version does not establish compatibility with every future engine change. See [release details](Developer/RELEASE-0.2.3.md).

The version gate accepts Microsoft package **1.8.907.0 or newer** and engine build **7445165 or newer**. Package identity, publisher and x64 architecture checks remain. Windows Xbox PC / Microsoft Store only; Xbox consoles, cloud gaming, Steam and GOG are outside this port's scope. Custom profile relocation is unsupported. Standard SE/manager automatic updates remain disabled.

Earlier releases included setup/restore fixtures, Lua/Osiris, gameplay and modded save/reload checks. Those are historical results, not fresh validation of this release. Full API coverage, multiplayer, achievements and long-session stability are not established. Keep pre-mod saves.

## Credits and corresponding source

- Norbyte: Script Extender, MIT with Commons Clause.
- LaughingLeader: BG3 Mod Manager, MIT.
- Volitio/AtilioA: Mod Configuration Menu, AGPLv3 plus component/font notices.
- Xbox integration and packaging: tito-reinaldo, with AI coding assistance.

This is not an official release or endorsement by those authors, Larian or Microsoft. Free distribution; no Donation Points. Component notices remain in **App/THIRD PARTY NOTICES.txt** and **LICENSE.txt**.

The [release](https://github.com/titoreinaldo/bg3-xbox-pc-mod-support/releases/tag/v0.2.3) includes full corresponding source and build instructions. GitHub's automatic Code/tag ZIPs are not the complete source package. See [BUILDING.md](BUILDING.md).

## Earlier releases

The 0.2.0 outer launcher was withdrawn after antivirus detections. It was removed in 0.2.1 and remains absent from 0.2.3. Package 0.2.2 added the full AGPLv3 license and copyright notices. Historical releases and their records remain available; do not use the withdrawn launcher or bypass security warnings. The [Nexus page](https://www.nexusmods.com/baldursgate3/mods/25204) is subject to Nexus scanning and moderation.

## Reports and contributions

Use the [bug report form](https://github.com/titoreinaldo/bg3-xbox-pc-mod-support/issues/new/choose) for problems and [CONTRIBUTING.md](CONTRIBUTING.md) for proposed fixes. Report security vulnerabilities through [SECURITY.md](SECURITY.md). See the [code of conduct](CODE_OF_CONDUCT.md).
