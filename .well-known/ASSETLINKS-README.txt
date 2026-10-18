assetlinks.json — Android App Links for https://stepsstreak.com/i/<code> (package ai.stepstreak.app).

The fingerprint listed now is the UPLOAD key (android/keystore/upload.jks). Builds installed from
Google Play are re-signed with Play's APP SIGNING key, so App Links only verify for Play installs
after you ADD that key's SHA-256 as a second entry in "sha256_cert_fingerprints":
  Play Console > StepStreak > Test and release > Setup > App signing > "App signing key certificate" > SHA-256.
Keep the upload-key entry too (it covers locally signed release builds).

GitHub Pages serves dotfolders only when .nojekyll exists at the repo root (it does if this site uses it;
otherwise add an empty .nojekyll). Check: curl -s https://stepsstreak.com/.well-known/assetlinks.json
