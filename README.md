# 🦉 OLicense

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OLicense** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OLicense audits the open-source licenses in a project. It identifies license texts by phrase fingerprint, scans a source tree for SPDX-License-Identifier tags, LICENSE files and package-manifest license fields, and checks whether those inbound licenses are compatible with your project's outbound license. It ships with all 740 SPDX license identifiers built in.

---

## ✨ Features

- Identifies a license from its full text with a confidence score
- Validates SPDX ids and expressions (AND / OR / WITH / +), including deprecation and OSI/FSF status
- Scans source trees: SPDX tags, LICENSE files and manifests (package.json, Cargo.toml, pyproject, composer, pom.xml, gemspec, setup.cfg)
- Compatibility matrix and inbound → outbound checks with copyleft findings
- Extracts copyright lines, lists per-license obligations and generates a NOTICES file
- Reports in TXT / JSON / Markdown / CSV / SARIF; CLI exits with code 3 on conflicts

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OLicense                                   # interactive menu
./OLicense --scan ./myproject --project MIT --notices NOTICES
./OLicense --identify LICENSE
./OLicense --validate "Apache-2.0 OR MIT"
./OLicense --compat GPL-3.0-only MIT
```

Run `./OLicense --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
