# Security Policy

BeamDisk connects Macs to storage over the network. It handles CHAP secrets and the data on the disks it connects, often on home, office and lab networks. We take security reports seriously.

## Reporting a vulnerability

**Do not file a public GitHub issue for security bugs.** Public disclosure before a fix is available puts other BeamDisk users at risk.

Please report vulnerabilities through:

1. **GitHub private security advisory**:
   [Open a draft advisory](https://github.com/3rdBitLabs/BeamDisk/security/advisories/new)

We will acknowledge receipt within 3 business days and aim to provide an initial assessment within 7 days.

## What to include

A useful report contains:

- A clear description of the issue and its impact.
- Affected BeamDisk version(s) and macOS version.
- The storage server or iSCSI target involved, if any, and its software version.
- Steps to reproduce, or a proof of concept.
- Any logs, packet captures or screenshots that help us reproduce it, with secrets removed.
- Whether you've shared this with anyone else.

## Scope

In scope:

- The BeamDisk app as distributed through the App Store and TestFlight.
- BeamDisk's handling of CHAP secrets and server details.
- BeamDisk's iSCSI implementation: anything a malicious or compromised target, or someone on the network, can make it do.
- Data integrity: anything that makes BeamDisk write the wrong data, or let two computers write one disk at once.

Out of scope:

- Vulnerabilities in storage servers, SANs or iSCSI target software. Report those to their vendors.
- General macOS vulnerabilities not introduced by BeamDisk.
- Issues that require physical access to an unlocked Mac.
- Social engineering, phishing, or attacks against BeamDisk users outside the app itself.

## Disclosure policy

- We follow coordinated disclosure. We'll work with you on a timeline to fix and release before public disclosure.
- Once a fix ships, we'll credit reporters in the release notes unless you'd prefer to remain anonymous.
- We do not currently run a paid bug bounty program.

## Hardening tips for users

A few practices worth keeping, whatever BeamDisk does:

- Keep iSCSI on a trusted network: a separate VLAN or a direct link to the server when you can. iSCSI is not meant to cross the internet.
- Use CHAP, or mutual CHAP so the server proves itself too, with a unique, long secret for each target.
- Allow only the initiator names that should reach each target on your server.
- Turn on CRC32C header and data digests if your network path is less than reliable and your target supports them.
- Keep macOS, BeamDisk and your storage server's software updated. Security fixes ship in updates.
