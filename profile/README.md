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
├── falcon-system-service    ← Node.js backend — Steam API, GPU stats, game launch
├── falcon-hw-profiles       ← gaming hardware profiles, driver scripts
└── falcon-site              ← Landing page and documentation
```

---

## Hardware Compatibility

| Brand | Model | GPU | Status |
|---|---|---|---|
| Laptop | 15/16" gaming laptop (10th–12th gen Intel) | RTX 3050 | 🚧 In Development |
| Laptop | Budget gaming laptop (10th–12th gen Intel) | RTX 3050 | 🚧 In Development |
| Laptop | Mid-range gaming laptop (11th–12th gen Intel) | RTX 3060/3070 | 🚧 In Development |
| Laptop | Entry gaming laptop 15/16" | RTX 3050/3060 | 🚧 In Development |
| Laptop | General-purpose laptop (Intel) | RTX 3050 | 🚧 In Development |
| Laptop | High-end gaming laptop 15/16" | RTX 3060–3080 | 🚧 In Development |
| Laptop | XPS 15 | RTX 3050 Ti | 🚧 In Development |

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
