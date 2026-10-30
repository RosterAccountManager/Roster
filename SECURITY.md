# Security policy

Roster handles `.ROBLOSECURITY` cookies. A cookie compromise lets an attacker take over the affected Roblox account. We take vulnerability reports seriously and ship fixes quickly.

---

## Reporting a vulnerability

**Preferred:** open a [GitHub Security Advisory](https://github.com/RosterAccountManager/Roster/security/advisories/new) on the repository. Advisories are private by default and let us coordinate a fix and disclosure with you.

**Alternative:** email the security contact listed on the project website's Trust page. Please include:

- A clear description of the issue and the impact.
- Steps to reproduce, or a proof-of-concept.
- The Roster version (Settings → About) and the Windows build.
- Whether you would like public credit on disclosure.

Please do **not** open a public GitHub issue for a vulnerability until a fix has shipped.

---

## What is in scope

- The Roster desktop application (`Roster.App.exe`) and any binary it ships.
- The auto-update channel and the manifest signing chain (Velopack / Ed25519).
- The licence activation + refresh flow (`api.accountroster.com`).
- The cookie vault format and its KDF / encryption path.
- The installer (`Roster-Setup-<version>.exe`).
- The project website (the marketing/download pages), to the extent a flaw there could ship a tampered binary.

## What is **not** in scope

- Roblox itself. Roster does not control the Roblox client, web API, or server-side behaviour. Report Roblox bugs to Roblox.
- Issues that require physical access to an already-unlocked Windows session.
- Self-XSS or social engineering of the local user.
- Denial of service from running the application without sufficient resources.
- Vulnerabilities in transitive dependencies that we cannot exploit through our code paths. (Report these upstream; we'll bump versions as fixes land.)

---

## Response targets

- **Acknowledgement:** within 3 business days of receipt.
- **Triage and severity assignment:** within 7 business days.
- **Fix shipped:** depends on severity. Critical issues (remote cookie disclosure, remote code execution, update-channel takeover) target a fix within 14 days of triage. Lower severities target the next regular release.
- **Public disclosure:** coordinated with the reporter. We aim to publish a GitHub Security Advisory within 90 days of the initial report, or sooner with reporter agreement once a fix has shipped.

---

## Safe harbour

We will not pursue civil or criminal action against researchers who:

- Make a good-faith effort to avoid privacy violations, destruction of data, and interruption or degradation of services.
- Only interact with accounts they own or have explicit permission to test with.
- Do not exploit a vulnerability beyond what is necessary to confirm its existence.
- Give us reasonable time to fix the issue before public disclosure.

---

## Credit

With the reporter's consent, we publish credit in the GitHub Security Advisory and in the release notes for the version that fixes the issue.
