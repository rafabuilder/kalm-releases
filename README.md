# Kalm releases

Release builds of Kalm and the Sparkle update feed. The source code lives in a separate private repository.

- Downloads and changelog: [Releases](https://github.com/rafabuilder/kalm-releases/releases)
- Update feed: `https://rafabuilder.github.io/kalm-releases/appcast.xml`

## Publishing a version

1. Build, sign and notarise `Kalm.dmg`.
2. Put it in a folder with the earlier DMGs and run Sparkle's `generate_appcast <folder> --download-url-prefix https://github.com/rafabuilder/kalm-releases/releases/download/v<version>/`. It signs each update with the private key in the login Keychain.
3. Create a GitHub release `v<version>` with the DMG attached and the release notes.
4. Commit the new `appcast.xml` here.
