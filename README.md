# Hoofware Remediation Lab

A disposable public repository for testing Hoofware's dependency-vulnerability detection and remediation workflow.

## Intentional test fixture

This repository intentionally pins **minimist 1.2.5**, which is affected by **CVE-2021-44906** (prototype pollution). The vulnerable dependency is included only as a scanner test fixture; this repository contains no application secrets or production code.

- Expected advisory: CVE-2021-44906
- Vulnerable version: minimist 1.2.5
- First fixed version: 1.2.6
- Expected ecosystem: npm
- Lockfile: package-lock.json

Do not use this dependency version in a real application. Do not deploy this repository as a service. Keep the vulnerable pin until the initial Hoofware scan has recorded the finding, then test the remediation workflow.
