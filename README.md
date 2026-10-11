# PocketBase ARMv6 Build Repository

Unofficial builds for Raspberry Pi 1, Zero, and Zero W.

[![Build PocketBase](https://github.com/ikhwan-qp/pocketbase-armv6/actions/workflows/build.yaml/badge.svg?style=flat-square)](https://github.com/ikhwan-qp/pocketbase-armv6/actions/workflows/build.yaml)
[![Check Latest Version](https://github.com/ikhwan-qp/pocketbase-armv6/actions/workflows/check.yaml/badge.svg?style=flat-square)](https://github.com/ikhwan-qp/pocketbase-armv6/actions/workflows/check.yaml)
[![Release](https://img.shields.io/github/v/release/ikhwan-qp/pocketbase-armv6?include_prereleases&sort=semver&style=flat-square)](https://github.com/ikhwan-qp/pocketbase-armv6/releases/latest)

## 📌 About This Repository

This repository **ONLY PROVIDES BINARIES FOR ARMv6 DEVICES AND DOES NOT ALTER SOURCE CODE** for the PocketBase repo. 

Since official PocketBase releases do not target ARMv6 (such as older Raspberry Pi models), this repository automates the compilation process to provide ready-to-use binaries. For software bugs, feature requests, or core issues regarding PocketBase, please visit the [PocketBase repository](https://github.com/pocketbase/pocketbase).

---

## 🚀 Quick Start / Installation on Raspberry Pi

1. Go to the **[Releases](../../releases)** page and download the latest `.tar.gz` file for ARMv6, or download it via terminal:
   ```bash
   # Example (replace <VERSION> with the actual version, e.g., v0.40.5)
   wget https://github.com/ikhwan-qp/pocketbase-armv6/releases/latest/download/pocketbase_<VERSION>_linux_armv6.tar.gz
   ```

   

2. Extract the archive:
   ```bash
   tar -xzf pocketbase_*_linux_armv6.tar.gz
   ```

3. Run PocketBase:
   ```bash
   ./pocketbase serve
   ```

---

## 🔒 Security & Verification

All release binaries are built transparently using GitHub Actions. You can verify the build provenance and integrity using GitHub CLI:

   ```bash
   gh attestation verify pocketbase_<VERSION>_linux_armv6.tar.gz -R ikhwan-qp/pocketbase-armv6
   ```
