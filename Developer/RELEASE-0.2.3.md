## Changes

- Accept Microsoft Store package **1.8.907.0 or newer** and engine build **7445165 or newer**, instead of requiring exact versions.
- Update both the Script Extender and manager checks, including the bundled DLL integrity hash.
- Keep Microsoft package identity, publisher, architecture and existing engine mapping checks.

## Validation

The manager and Script Extender were rebuilt successfully. The maintainer confirmed that the updated game launches correctly on Microsoft package **1.8.910.0** on 3 October 2026. No additional automated tests or gameplay/save-load tests were run for this release. Later builds pass the version gate; this does not establish compatibility with every future engine change.

## Downloads

- **BG3-Xbox-Mod-Manager-0.2.3.zip**: player package. Extract it outside the game folder and open `App/BG3ModManager.exe`.
- **BG3-Xbox-PC-Corresponding-Source-0.2.3.zip**: complete corresponding sources, licenses and build instructions.
- **SHA256SUMS-0.2.3.txt**: archive and changed-binary checksums.

The manager window still identifies experimental build 0.2.0; the package version is 0.2.3. Keep your existing setup backups. The withdrawn outer launcher is not included.

Norbyte's Script Extender, LaughingLeader's manager, Volitio/AtilioA's MCM and other components retain their existing licenses. Experimental Windows x64 Xbox PC / Microsoft Store release.
