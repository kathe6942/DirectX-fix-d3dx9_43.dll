# 🎮 DirectX-fix-d3dx9_43.dll

> A small Windows utility to diagnose and fix game crashes caused by **inpoutx64.sys** driver conflicts

[![Windows](https://img.shields.io/badge/Platform-Windows-blue?logo=windows)](https://www.microsoft.com/windows)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-success)]()
[![Donwload](https://img.shields.io/badge/donwload-success)]()

---

## 🚨 The Problem

After the Windows 11 **KB5121003** update, many users experienced sudden game crashes with:
- **EXCEPTION_ACCESS_VIOLATION** errors
- Anti-cheat blocking messages
- Unexpected crashes without clear cause

**Root cause:** The driver **inpoutx64.sys** can conflict with certain hardware and software configurations.

---

## ✨ What It Checks

This tool automatically diagnoses:

- ✅ Windows version and installed updates
- ✅ Whether **inpoutx64.sys** is installed
- ✅ Which service loads the driver
- ✅ If the driver is currently running

**What it does NOT do:**
- ❌ Replace DirectX files
- ❌ Copy DLLs into game folders
- ❌ Automatically delete drivers

---

## 🚀 Quick Start

### Before running it

Close the game first.

If you have RGB, motherboard or hardware-monitoring software running, close that too. Some of these programs install inpoutx64.sys as part of their hardware access.

Run the tool as Administrator if Windows doesn't allow it to read or change the driver configuration.

---

# What to do if the driver is found

Don't delete the .sys file manually.

The safer approach is to identify the application that installed it and either update that application or temporarily disable its driver. That also makes it possible to restore the setup later if it turns out not to be the cause.

---

# If the crash isn't fixed

Then inpoutx64.sys probably wasn't the problem.

Check the GPU driver, verify the game files, remove unstable overclocks, and look at the game's crash log. Anti-cheat software can also produce very similar symptoms.

This project only targets the driver conflict described above.
