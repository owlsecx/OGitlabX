# 🦉 OGitlabX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OGitlabX** — GitLab Self-Managed / Omnibus Config Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

GitLab self-managed / Omnibus configuration security auditor

---

## ✨ Features

- Stdlib Ruby-literal parser for gitlab.rb (hashes, arrays, symbols, heredocs, ENV references), YAML-lite for gitlab.yml / LDAP heredocs, TOML-lite for Runner
- `gitlab-ctl show-config` JSON / text export import
- External URLs, HTTPS redirect, Let's Encrypt, NGINX TLS protocols / ciphers / HSTS, rendered gitlab-http
- Sign-up, 2FA, group creation, OmniAuth SSO, SAML, OIDC, LDAP certificate verification & encryption
- Plaintext SMTP / DB / Redis / S3 / GCS secrets, gitlab-secrets.json permission checks (never read)
- Registry, Puma, Workhorse, Gitaly, Pages, Mattermost, Prometheus / Grafana, PostgreSQL & Redis in gitlab.rb
- Geo secondary TLS, backups, version end-of-life
- Runner privileged / docker.sock / shell executor
- Secrets masked everywhere; --root discovery; CWE + MITRE
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Self-test --demo, CI gates --fail-on / --min-severity

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OGitlabX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
