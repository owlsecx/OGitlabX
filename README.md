# 🦉 OGitlabX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OGitlabX** — GitLab Self-Managed / Omnibus Config Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OGitlabX — GitLab Self-Managed / Omnibus Config Auditor. It provides stdlib Ruby-literal parser for gitlab.rb (hashes, arrays, symbols, heredocs, ENV references), YAML-lite for gitlab.yml / LDAP heredocs, TOML-lite for Runner; `gitlab-ctl show-config` JSON / text export import. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- Stdlib Ruby-literal parser for gitlab.rb (hashes, arrays, symbols, heredocs, ENV references), YAML-lite for gitlab.yml / LDAP heredocs, TOML-lite for Runner
- `gitlab-ctl show-config` JSON / text export import
- External URLs, HTTPS redirect, Let's Encrypt, NGINX TLS protocols / ciphers / HSTS, rendered gitlab-http
- Sign-up, 2FA, group creation, OmniAuth SSO, SAML, OIDC, LDAP certificate verification & encryption
- Plaintext SMTP / DB / Redis / S3 / GCS secrets, gitlab-secrets.json permission checks (never read)
- Registry, Puma, Workhorse, Gitaly, Pages, Mattermost, Prometheus / Grafana, PostgreSQL & Redis in gitlab.rb

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OGitlabX                                     # interactive menu
./OGitlabX --scan -r /path/to/root
./OGitlabX --demo
./OGitlabX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*

---

## 🔍 Verification & Transparency

This tool is closed-source. These files let you see exactly what is inside it,
without the source:

- [`SBOM.cdx.json`](SBOM.cdx.json) — CycloneDX inventory: SHA-256 of this
  binary, bundled CPython version, and every bundled library with its exact
  version and license. Feed it to Grype, Trivy or Dependency-Track to audit
  our dependencies for CVEs yourself.
- [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) — the full license text
  of every third-party component, extracted from this binary.

**No telemetry, no analytics, no licence check-in.** This tool does not phone
home. Verify that claim yourself:

```bash
sudo strace -f -e trace=network ./OGitlabX --help   # watch every network call
firejail --net=none ./OGitlabX --help               # deny the network entirely
```

Release signing, GPL compliance and vulnerability reporting:
[**TRUST.md**](https://github.com/owlsecx/owl-os/blob/main/TRUST.md)
