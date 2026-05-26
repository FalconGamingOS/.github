<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Rajdhani&weight=700&size=42&duration=3000&pause=1000&color=00AAFF&center=true&vCenter=true&width=600&height=80&lines=FALCONOS;BUILT+FOR+GAMING;BUILT+IN+PAKISTAN" alt="FalconOS"/>

**Ubuntu-based console-style gaming OS for NVIDIA RTX 30xx systems.**
Boot in 15 seconds. No bloat. No desktop. Just games.

[![Status](https://img.shields.io/badge/status-in_development-00aaff?style=flat-square&labelColor=0d0d1a)](https://github.com/FalconGamingOS)
[![License](https://img.shields.io/badge/license-GPL_v3-ff6a00?style=flat-square&labelColor=0d0d1a)](https://github.com/FalconGamingOS/falcon-os-build/blob/main/LICENSE)
[![OS](https://img.shields.io/badge/base-Ubuntu_24.04-00aaff?style=flat-square&labelColor=0d0d1a)](https://ubuntu.com)
[![GPU](https://img.shields.io/badge/GPU-NVIDIA_RTX_30xx-76b900?style=flat-square&labelColor=0d0d1a)](https://github.com/FalconGamingOS/falcon-hw-profiles)
[![Made in](https://img.shields.io/badge/made_in-Pakistan-009900?style=flat-square&labelColor=0d0d1a)](https://github.com/FalconGamingOS)

---

</div>

## What is FalconOS?

FalconOS is an **Ubuntu 24.04-based gaming operating system** that boots directly into a console-style launcher — think PS5 meets Linux. No desktop to manage. No Windows bloat. Just your games, ready in 15 seconds.

Built specifically for **gaming laptops and desktops** with **NVIDIA RTX 30xx GPUs**, FalconOS auto-installs drivers, pre-configures Steam + Proton, and delivers a gaming experience that beats Windows on the same hardware.

> Built in Pakistan. For Pakistani gamers. And everyone else.

---

## Key Features

| Feature | Details |
|---|---|
| **Auto GPU setup** | NVIDIA 550 drivers install on first boot, Secure Boot signed, survive kernel updates |
| **Console UI** | PS5-style full-screen launcher via Gamescope — controller + keyboard navigation |
| **Proton + DXVK** | Run Windows games natively. DX9 → DX12. DLSS 2.x on RTX hardware |
| **Liquorix kernel** | Low-latency gaming kernel with NVMe tuning and optimised scheduler |
| **Broad wifi support** | Pre-baked Realtek/Intel/Broadcom wifi firmware — works out of the box |
| **Desktop mode** | One tap to KDE Plasma. One tap back to Gaming Mode |
| **15s boot** | From power button to game launcher — no waiting |
| **Zero background updates** | Updates never interrupt your session |

---

## Minimum Requirements

```
CPU      Intel Core i5 10th gen+
RAM      16 GB DDR4/DDR5
Storage  NVMe M.2  (any capacity)
GPU      NVIDIA RTX 30xx  (Ampere)
```

---

## Repositories

```
FalconGamingOS/
├── falcon-os-build          ← ISO pipeline, kernel, Calamares installer
├── falcon-launcher          ← React console UI (PS5-style game grid)
├── falcon-system-service    ← Python FastAPI backend — Steam API, GPU stats, game launch
├── falcon-hw-profiles       ← gaming hardware profiles, driver scripts
└── falcon-site              ← Landing page and documentation
```

---

## Development Cycles

FalconOS follows a 10-cycle model. Each cycle has one measurable deliverable and a clear definition of done. A cycle does not start until the previous one ships.

| Cycle | Name | Deliverable | Definition of Done | Duration | Status |
|---|---|---|---|---|---|
| **C1** | Build Pipeline | Working Cubic + QEMU pipeline | Bootable ISO built and tested in QEMU in under 10 minutes | Week 1–2 | 🔵 Current |
| **C2** | Base Hardening | Stripped, tuned Ubuntu base | Boots under 15s. Idle RAM under 400MB. Liquorix running | Week 3–4 | ⬜ Planned |
| **C3** | GPU Automation | Auto GPU driver install service | Driver installs with zero user input. Secure Boot signed. Survives kernel update | Week 5–6 | ⬜ Planned |
| **C4** | Gaming Stack | Full gaming layer baked into ISO | Steam launches. Proton-GE selectable. One Windows game runs via Proton | Week 7–8 | ⬜ Planned |
| **C5** | Console UI | Gamescope session + React launcher | Boots into full-screen launcher. Games launch one-tap. Controller navigates UI | Week 9–12 | ⬜ Planned |
| **C6** | Installer | Calamares + first boot wizard | Non-technical user installs in under 5 minutes. GPU setup runs automatically | Week 13–15 | ⬜ Planned |
| **C7** | Hardware Testing | Verified on real machines | Tested on 2+ physical machines. Top 10 issues fixed. Test suite green | Week 16–17 | ⬜ Planned |
| **C8** | Update System | Safe OTA updates with rollback | Timeshift snapshots before every update. Never interrupts gaming. Rollback in one command | Week 18–19 | ⬜ Planned |
| **C9** | Beta Release | v0.1-beta public ISO | Published on GitHub Releases with SHA256. Install guide live. 100+ downloads | Week 20–22 | ⬜ Planned |
| **C10** | v1.0 | Stable v1.0 release | All P1/P2 bugs resolved. Covered by at least one Linux publication. v1.1 roadmap published | Week 23–24 | ⬜ Planned |

---

## Roadmap

- [x] GitHub org + repositories setup
- [x] Project architecture defined
- [ ] `falcon-os-build` — base ISO hardening
- [ ] NVIDIA 550 auto-install service
- [ ] Gaming stack (Steam, Proton-GE, Lutris)
- [ ] Gamescope session + auto-login
- [ ] `falcon-launcher` — React console UI
- [ ] `falcon-system-service` — backend daemon
- [ ] Calamares installer
- [ ] First boot wizard
- [ ] v0.1-beta public release

---

## Known Limitations

- ❌ Valorant, PUBG (kernel-level anti-cheat — not fixable)
- ❌ AMD GPU support (v1.1 target)
- ❌ 32-bit app support

---

## Contributing

The best place to contribute right now is **[falcon-hw-profiles](https://github.com/FalconGamingOS/falcon-hw-profiles)** — submit a profile for your machine and help expand hardware support.

1. Fork `falcon-hw-profiles`
2. Add a folder under `laptop/` or `laptop/` with your model name
3. Include a `profile.json` (wifi chip, known issues) and `tweaks.sh`
4. Open a PR

---

## Website

**[falcongamingos.github.io](https://falcongamingos.github.io)**

---

<div align="center">

*GPL v3.0 — Open Source — Built in Pakistan*

</div>
