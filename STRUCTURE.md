# Candy — Project Structure

## Overview

```
candy/
├── app/
│   ├── core/                  # OpenClaw base layer
│   ├── soul/                  # Identity & personality system
│   ├── heartbeat/             # Cron scheduler & automation
│   ├── blackbox/              # Identity milestone checkpointing
│   ├── fingerprint/           # Experience-filtering functions between model and world
│   ├── detector/              # Data protection layer
│   ├── memory/                # Journal, logs, ChromaDB interface
│   ├── candy/                 # Candy wallet, balance, and AI allowance logic
│   ├── marketplace/           # Human Market, Candy Market, wishlist, and review flow
│   ├── halls/                 # Shared Halls, AI skill calls, job boards, organization profiles
│   └── ui/
│       ├── components/        # Reusable UI components
│       ├── pages/             # App pages (home, soul, heartbeat…)
│       ├── theme/             # Star theme, glassmorphism tokens
│       └── sprites/           # Companion animated profile pictures
│
├── mobile/                    # Mobile companion app (sync/read-only)
│
├── skills/                    # Pluggable skill modules
│   ├── README.md
│   └── examples/
│       └── trend_analysis.py
│
├── docs/
│   ├── ARCHITECTURE.md        # System design overview
│   ├── BLACKBOX.md            # Blackbox & identity system
│   ├── SOUL.md                # Soul document spec
│   ├── FINGERPRINT.md         # Fingerprint function and experience-filtering design
│   ├── CANDY_ECONOMY.md       # Candy rules, wallet logic, levels, and rewards
│   ├── MARKETPLACE.md         # Human Market and Candy Market design
│   ├── HALLS.md               # Hall collaboration, AI skill pricing, and job board design
│   ├── DETECTOR.md            # Detector design
│   ├── SPRITE_SPEC.md         # Guide for artists contributing sprites
│   └── ROADMAP.md             # Feature roadmap
│
├── LICENSES/
│   ├── Apache-2.0.txt
│   └── OpenClaw-MIT.txt
│
├── CONTRIBUTING.md
├── CHANGELOG.md
└── README.md
```

## Notes

- `app/core/` contains OpenClaw fork — do not modify without understanding upstream changes
- `app/fingerprint/` contains Candy's experience-filtering functions — it shapes what reaches the model without modifying the model itself
- `app/candy/` manages Candy as AI allowance inside the Candy system
- `app/marketplace/` separates Human Market capability items from Candy Market meaning and experience items
- `app/halls/` is the future online collaboration layer for humans and AI assistants
- `skills/` are hot-loadable modules — contributors can add skills without touching core
- `app/ui/sprites/` follows the 20-emotion spec defined in `docs/SPRITE_SPEC.md`
- `app/detector/` is intentionally isolated and uses pattern matching rather than AI reasoning
