# AI Ledger service list

The published list of AI services that the AI Ledger iPhone app recognises. The app downloads one file from here, checks its signature, and uses it in place of the list built into the app.

- `catalog.signed` is the file the app downloads. Its first line holds a key ID and an Ed25519 signature; the rest is the JSON document the signature covers.
- `catalog.json` is the same document as plain text, for reading.

The app only accepts a list signed by a key it trusts, with a higher version number than the one it already has. Anything else is ignored.

The file is public and holds only the names of AI services and the domains they use. The app sends nothing about its user when it fetches it.

No list has been published yet.
