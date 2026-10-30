# Contributing to BeamDisk

Thanks for your interest in helping out. BeamDisk is made by a small team, and the most useful contributions are usually not code.

## About this repository

This repository is the **community hub** for BeamDisk. It does not contain BeamDisk's source code: BeamDisk is proprietary, made by [3rd Bit Labs](https://3rdbitlabs.com).

## Ways you can help

### Report bugs

[Open a bug report](https://github.com/3rdBitLabs/BeamDisk/issues/new/choose) using the issue form. It asks for the versions, your setup and BeamDisk's messages, which we need to reproduce the problem. The more specific you are, the faster we can fix it.

For security bugs, see [SECURITY.md](SECURITY.md). Do not file public issues for vulnerabilities.

### Request features

[Open a feature request](https://github.com/3rdBitLabs/BeamDisk/issues/new/choose). Lead with the problem you're trying to solve, not the implementation. Concrete use cases are far more persuasive than abstract wishes.

Search existing issues first. If your idea is already filed, add a thumbs-up or a comment with your use case rather than opening a duplicate.

### Share Test Speed results

If you've measured BeamDisk on your own server and network, post your results in the [Benchmarks discussion category](https://github.com/3rdBitLabs/BeamDisk/discussions). Use the template so posts can be compared. Real-world numbers help other people choose their storage and network.

### Report how BeamDisk works with your target

BeamDisk is tested with TrueNAS and Linux LIO / targetcli. If you use it with another storage server, SAN or iSCSI target, tell us how it went in [Discussions](https://github.com/3rdBitLabs/BeamDisk/discussions), working or not. If you make storage, [get in touch](https://beamdisk.app/contact/?category=vendor) about qualifying BeamDisk with your targets.

### Help other users

[Discussions](https://github.com/3rdBitLabs/BeamDisk/discussions) is where users ask questions and trade tips. If you've solved a problem yourself, posting your solution there saves the next person hours.

### Improve the documentation

The docs live at [beamdisk.app/docs](https://beamdisk.app/docs/). If something is unclear, missing or wrong, open an issue here describing the gap and we'll fix the docs.

## Issue and discussion etiquette

- **Search first.** Most questions have been asked before.
- **One issue per bug.** Don't bundle unrelated problems into one report.
- **Keep secrets out.** Never post CHAP secrets. Consider replacing server addresses and target names with placeholders.
- **Be patient.** BeamDisk is maintained by a small team. We'll get to your issue.
- **Be kind.** See the [Code of Conduct](CODE_OF_CONDUCT.md).

## Triage labels

Maintainers use a small label set to triage:

- `bug` / `enhancement` - what kind of issue it is.
- `needs-info` - waiting on the reporter for more detail.
- `confirmed` - we've reproduced it.
- `target-specific` - it happens only with a particular storage server or target.
- `wontfix` - we've decided not to act on it (with a comment explaining why).

If your issue gets `needs-info`, please respond. Issues with no response after 30 days may be closed.
