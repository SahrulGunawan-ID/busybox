# Contributing Guidelines

Welcome, and thank you for considering a contribution to this BusyBox GCC compatibility project.

This repository provides a manual patch for ensuring BusyBox builds correctly on modern GCC toolchains, especially for builders like Thunder Linux. All contributions should prioritize simplicity, compatibility, and modular integration.

---

## 📁 Repository Scope

- ✅ GCC compatibility for BusyBox builds
- ✅ Manual scripts and patches for `check-lxdialog.sh`
- ✅ Markdown-based documentation only
- ❌ No CI/CD integrations, automated tests, or deployment workflows

---

## 🔧 How to Contribute

1. **Create a New Branch**
   - Work in your own local fork or repository
   - Choose meaningful branch names, such as `fix-main-syntax` or `doc-update-usage`

2. **Make Your Changes**
   - Follow semantic formatting in shell scripts and markdown files
   - Update related `.md` files if applicable
   - Avoid toolchain hardcoding—favor portability across builder environments

3. **Test Everything**
   - Use GCC 12+ or higher
   - Validate patched `check-lxdialog.sh` using a working BusyBox source
   - Run builds manually via `make menuconfig && make`

4. **Submit a Pull Request**
   - Describe the change clearly
   - Reference any affected versions, environments, or error messages
   - Keep documentation modular and consistent with the tone of this project

---

## 📜 Contribution Rules

- All patches must comply with **GPLv2** (same license as BusyBox)
- Binary submissions are not accepted
- Large additions must be modular and justified
- Formatting should follow the style used across existing files

---

## 🧙 Builder Philosophy

This project supports modular builder environments, rootfs stealth configurations, and static toolchain strategies. Contributions should respect:

- Portability across ARM64, x86_64, and rootless shells
- Compatibility with minimal Linux environments
- Manual build processes that avoid CI/CD or centralized deployment

---

For help, ideas, or patch discussions, feel free to open an issue labeled `[@SahrulGunawanID]`. Thank you for strengthening the builder ecosystem!
