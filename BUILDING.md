# Build instructions

Download **BG3-Xbox-PC-Corresponding-Source-0.2.3.zip** from the [0.2.3 release](https://github.com/titoreinaldo/bg3-xbox-pc-mod-support/releases/tag/v0.2.3) and follow its **BUILDING.md**. It contains the complete modified sources, build helpers, dependency records and existing setup fixtures.

The repository and GitHub's automatic source ZIPs do not contain the complete component sources. [Minimum-Version-0.2.3.patch](Developer/Minimum-Version-0.2.3.patch) records the code changes relative to the 0.2.2 corresponding-source archive. [RELEASE-0.2.3.json](Developer/RELEASE-0.2.3.json) records the changed binary hashes and validation scope.

Build the native DLL first, then set its SHA256 in `Source/BG3ModManager/src/GUI/Util/XboxPcSetup.cs` before building the manager. Native binaries can differ across compiler versions and timestamps, so this hash must match the DLL being packaged. The release used .NET SDK 8.0.425 and portable MSVC 14.51.36231 (compiler 19.51.36260), Windows SDK 10.0.26100.0.

The current package starts `App/BG3ModManager.exe` directly. The old installer and its tests remain in the [v0.1.0 history](https://github.com/titoreinaldo/bg3-xbox-pc-mod-support/tree/v0.1.0).
