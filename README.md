# Xerinfuscator — Next-Gen .NET Obfuscator

[![Release](https://img.shields.io/badge/release-v1.0.0-blue)](https://xerinfuscator.great-site.net)
[![License](https://img.shields.io/badge/license-Proprietary-red)]

**Xerinfuscator** is a production-ready, high-performance .NET obfuscator designed to raise the bar on reverse-engineering resistance. It combines multiple protection layers — code virtualization, string & integer encryption, anti-debug/anti-dumping, control-flow obfuscation, proxying and more — to make analysis and tampering expensive and time consuming.

---

## Table of Contents

* [Key Features](#key-features)
* [Limitations & Notes](#limitations--notes)
* [Compatibility](#compatibility)
* [Changelog Highlights](#changelog-highlights)
* [Pricing & Plans](#pricing--plans)
* [Legal & Responsible Use](#legal--responsible-use)
* [Support & Contact](#support--contact)

---

## Key Features

* **Code Virtualization (VM)** — convert IL into custom bytecode executed by a VM runtime to hide program logic.
* **String Encryption** — compress & encrypt strings with runtime decryption and caching for performance.
* **Integer & Constant Protection** — protect numeric constants (including switch-case handling) using optimized transforms.
* **Control-Flow Obfuscation & Code Mutation** — reorder and replace IL with semantically equivalent but harder-to-analyze sequences.
* **Symbols Renaming** — rename types/methods/fields/parameters to unreadable identifiers (including options for Unicode/glyph names).
* **Reference / Delegate Proxying** — replace direct calls with encrypted/reflective proxies and delegate tables.
* **Anti-Debugging / Anti-Dumping / Anti-Tamper** — runtime checks to block debuggers, memory dumps, and unauthorized modifications.
* **Resources & Imports Protection** — encrypt embedded resources and hide/secure native imports.
* **Project System & Presets** — save/load protection profiles to reproduce the same settings across builds.

---

## Limitations & Notes

* Some advanced protections (VM, anti-tamper, native packing) may be incompatible with specific assembly types, e.g. C++/CLI binaries, strongly-signed assemblies, or assemblies that must be patched after protection. Always test protected assemblies thoroughly.
* Virtualization and heavy obfuscation may increase binary size and affect startup time or JIT behavior in certain environments — profile critical paths.
* Obfuscation raises the cost of reverse engineering but does not make it impossible. Consider obfuscation as part of a defense-in-depth strategy.

---

## Compatibility

* **Platforms:** Windows, Linux (feature behavior may vary depending on runtime & native wrappers).
* **Frameworks:** Broad .NET support (modern .NET Core / .NET 5–10 and .NET Framework families). Validate target frameworks when using advanced features.
* **Application Types:** Console apps, WinForms, WPF, ASP.NET apps, class libraries, services — subject to the limitations above.

---

## Changelog Highlights

* Improved integer encryption and switch-case handling to reduce runtime overhead.
* VM runtime fixes: better compatibility with embedded dependency loaders (Costura/ILMerge-like scenarios) and improved performance for hot paths.

---

## Pricing & Plans

Pricing and plans are maintained on the official site. For commercial / enterprise licensing and custom builds, contact the team.

---

## Legal & Responsible Use

Xerinfuscator is intended to protect legitimate software IP. The tool should not be used to hide malware, exfiltrate data, or violate third-party licenses. Users must comply with applicable laws and the tool's terms of service.

---

## Support & Contact

* Website: [https://xerinfuscator.great-site.net/](https://xerinfuscator.great-site.net/)
* Email: [xerinfuscator@gmail.com](mailto:xerinfuscator@gmail.com)
* Community: Discord & Telegram (links available on the site footer)

---
