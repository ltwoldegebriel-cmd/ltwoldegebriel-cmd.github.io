# assetlinks for Nineveh: Home Library (TWA)

This folder is the content for a NEW GitHub user-site repo named
ltwoldegebriel-cmd.github.io (not created yet). It will serve:

https://ltwoldegebriel-cmd.github.io/.well-known/assetlinks.json

Why: Android verifies a Trusted Web Activity by fetching
/.well-known/assetlinks.json at the ROOT of the origin. The app lives on a
GitHub Pages project site (/library-catalog/), which can only publish under
/library-catalog/. Only the user-site repo publishes at the domain root.

The .nojekyll file is required, or GitHub Pages (Jekyll) skips the
.well-known folder.

Note: creating the user-site repo does not affect the /library-catalog/
project site. Both keep working.

Current fingerprint (upload key):
A3:1B:AA:21:15:D3:34:89:44:9A:3F:AD:90:46:E8:1C:B6:36:27:15:DD:12:2A:E7:51:57:7F:E2:A8:65:54:89

After uploading to Play with Play App Signing, add the app signing key
SHA-256 from Play Console (Test and release > App integrity > App signing)
as a second entry in sha256_cert_fingerprints. Without it, the Play-installed
app shows a browser URL bar instead of running full screen.
