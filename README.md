# app-config

Holds one file, `servers.json`: the signed list of server addresses the IPO Hisab Kitab app may use.

- It contains no secrets: only public addresses and a signature.
- The app accepts it only if the signature checks out against the release key built into the app,
  and only if its version is newer than the one the app already has.
- Changing this file without the release private key has no effect on any phone.
