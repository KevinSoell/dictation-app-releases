# Security

## Reporting a problem

Please report security problems privately through GitHub:
**https://github.com/KevinSoell/dictation-app-releases/security/advisories/new**
("Report a vulnerability"). Do not open a public issue and do not include other
people's data. You will get an answer there; please give a reasonable time to fix
it before telling others.

Helpful: the app version (Settings → General), macOS version, what you did, what
happened, and why it is a security problem.

## Scope

- Dictation App for macOS as downloaded from
  `github.com/KevinSoell/dictation-app-releases` (DMG and automatic updates).
- The update feed and release files in that repository.

Out of scope: problems that need an attacker who already controls your Mac,
reports about third-party services (GitHub, Hugging Face), and social engineering.

## How the app is protected (short)

- Speech recognition runs on your Mac; no audio, text or settings are sent anywhere.
- Updates are accepted only with a valid EdDSA (Ed25519) signature from the
  developer's key; the update feed itself is signed too.
- The app is signed and uses the macOS hardened runtime; it asks only for the
  microphone and Accessibility (to type the recognized text).
