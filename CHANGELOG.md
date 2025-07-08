# Changelog

All notable changes to this project will be documented in this file.  
This project adheres to [Github] https://github.com/SahrulGunawan-ID/busybox.

## [1.0.0] – 2025-07-08

### 🔧 Added
- Compatibility patch for BusyBox `check-lxdialog.sh` script to support GCC 12+ and newer.
- Replaced legacy `main()` function signature with `int main() { return 0; }` to conform to modern C standards.

### 🧪 Verified
- Confirmed compatibility with:
  - BusyBox version 1.37.0
  - GCC versions 12, 13, and 14
  - ARM64 environments and modular builder setups
