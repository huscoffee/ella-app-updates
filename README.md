# La Macchini app updates

Public, download-only release channel for the La Macchini iOS and Android app.

This repository intentionally contains no application source code, credentials,
private signing keys, customer data, or machine data. Future release assets are
compiled web bundles encrypted for the La Macchini app. The client verifies its
native identity (`com.lamacchini.lm` on iOS or `com.lamacchini.app` on Android),
accepts assets only from this repository, and verifies their encrypted checksum.

`stable.json` is currently disabled. The first updater-capable native build must
be installed through TestFlight/App Store or the normal Android distribution
before an over-the-air web bundle can be used.

## Publication order

1. Build, test, encrypt, and review the candidate in the private app repository.
2. Create its immutable GitHub release tag and upload the encrypted ZIP.
3. Verify the public asset download and SHA-256 digest.
4. Publish the matching `stable.json` last.

Never upload an unencrypted ZIP or a private signing key.
