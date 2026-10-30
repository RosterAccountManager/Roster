# Roster

**Roster** is a multi-account Roblox manager for Windows. This repository hosts
the official **release downloads** and the **auto-update channel** for Roster.

- **Website / download:** https://accountroster.com
- **Latest release:** https://github.com/RosterAccountManager/Roster/releases/latest

## Is this the source code?

No. Roster is proprietary software and its source is **not** published. This
repository exists only to distribute release builds and to host
security advisories. Use of Roster is governed by the
[EULA](https://accountroster.com/legal).

## Verifying your download

Every release publishes a SHA-256 hash in its release notes. Verify the file
before installing:

```powershell
Get-FileHash Roster-Setup-<version>.exe -Algorithm SHA256
```

Updates are delivered via Velopack and are Ed25519-signed; the app refuses any
update whose signature does not verify against the public key built into the
binary at compile time.

> **SmartScreen:** Roster ships unsigned by design (no EV certificate). Windows
> may warn on first launch — choose **More info → Run anyway**. See the
> [Trust page](https://accountroster.com/trust) for why.

## Security

Found a vulnerability? See [SECURITY.md](./SECURITY.md).

## Trademark / affiliation

Roster is an independent project. Not affiliated with, endorsed by, or sponsored
by Roblox Corporation.
