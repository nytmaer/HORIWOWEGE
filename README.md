# 🔫 HORIWOWEGE

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://nytmaer.github.io/HORIWOWEGE/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Meta Horizon Worlds](https://img.shields.io/badge/Meta-Horizon%20Worlds-blue)](https://www.meta.com/horizon-worlds/)

**HORI**zon **WO**rlds **WE**apon **GE**nerator — A web-based tool for creating Meta Horizon Worlds compatible weapon configurations. Built for the Chop 'N Pop: Graveyard Bash weapon system.

**🚀 Live Demo: [nytmaer.github.io/HORIWOWEGE/](https://nytmaer.github.io/HORIWOWEGE/)**

## ✨ Features

- **🎯 Guided Generator**: Step-by-step weapon configuration with smart defaults
- **⚡ Shorthand Randomizer**: Quick weapon generation using simple keywords
- **📋 Complete Output**: TypeScript configs, entity hierarchies, and deployment guides
- **🎲 Random Variations**: Auto-generates weapon variants (MkII, Elite, Tactical, etc.)
- **📱 Responsive Design**: Works on desktop and mobile

## 🎮 Supported Weapon Types

| Type | Description | Special Mechanics |
|------|-------------|-------------------|
| `pistol` | Standard sidearm | Balanced stats |
| `revolver` | High power, slow reload | Heavy recoil |
| `smg` | Rapid fire, low damage | Full-auto |
| `rifle` | Balanced automatic | Versatile |
| `sniper` | Long range, high damage | Single-shot |
| `shotgun` | Spread shot | 8 pellets |
| `rocketlauncher` | Explosive projectile | Area damage |
| `laser` | Hitscan energy weapon | No recoil |
| `machinegun` | Heavy suppressive fire | 100 round capacity |

## 🚀 Quick Start

### Guided Mode
1. Select weapon type (auto-fills realistic defaults)
2. Adjust stats: fire rate, recoil, ammo capacity, damage
3. Click "Generate" → Copy TypeScript config

### Shorthand Mode
Generates 1-3 random variants per type with ±20% stat variation.

rocketlauncher
machinegun, pistol
shotgun, sniper, laser

## 📋 Output Includes

- **TypeScript Configuration** (`GunCore.ts` ready)
- **Entity Hierarchy** (matching ZombieGun3000 structure)
- **Script Dependencies** (all required imports)
- **Projectile Hit Handler** (`NPCAgent.ts` template)
- **Deployment Checklist** (step-by-step setup)

## 🛠️ Horizon Worlds Integration

Based on the official weapon system from **Chop 'N Pop: Graveyard Bash**:

- Uses `GunCore.ts` and `GunProjectile.ts` (Local execution mode)
- Compatible with `ProjectileLauncher` gizmo
- Supports crosshairs for 2D screens (Web/Mobile)
- Integrates with `Events.projectileHit` system

### Required Scripts

GunCore.ts          → Attach to weapon reference object
GunProjectile.ts    → Attach to ProjectileLauncher gizmo
AnimUtils.ts        → Animation utilities
Events.ts           → Event system
HapticFeedback.ts   → Controller haptics
StageHand.ts        → Stage management
Throttler.ts        → Rate limiting


## 🏗️ Entity Structure
WeaponName (Reference Object)
├── GunCore.ts (Script - Local Mode)
├── HackyGrabCube (Grab points)
├── WeaponModel (Asset Bundle)
├── MuzzleFlash (VFX)
├── ProjectileLauncher (Gizmo)
│   └── GunProjectile.ts (Script - Local Mode)
├── AmmoText (Text Gizmo)
├── WeaponPickup (Sound)
├── WeaponFire (Sound)
├── WeaponReload (Sound)
├── WeaponDryFire (Sound)
├── WeaponShellDrop (Sound)
└── WeaponPickup (Sound)

🤝 Contributing
Fork the repository
Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

See CONTRIBUTING.md for detailed guidelines.

📄 License
Distributed under the MIT License. See LICENSE for more information.

🙏 Acknowledgments
Based on Meta Horizon Worlds documentation
Chop 'N Pop: Graveyard Bash weapon system reference
Meta Horizon Worlds creator community
Made with 💜 for VR creators by nytmaer
HORIWOWEGE = HORIzon WOrlds WEapon GEnerator


