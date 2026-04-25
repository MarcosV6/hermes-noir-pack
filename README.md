# 🌌 Hermes Noir Pack

> **Three premium dashboard themes for Hermes Agent.** Deep space aesthetics, advanced CSS animations, and meticulous attention to detail. Built for the hackathon. Built to win.

---

## ✨ The Collection

### 🌊 Aurora — The Command Center
*Deep indigo canvas, electric cyan data streams, amber alerts*

A cockpit-style command center with animated grid overlay, corner brackets, and pulsing ambient glow. Every element feels alive — cards breathe, tabs pulse, and the background grid shifts with a subtle rhythm. Built for operators who need their dashboard to feel like a mission control.

**Key Features:**
- Cockpit layout with 260px sidebar rail for telemetry
- Animated grid overlay with breathing opacity
- Corner brackets on all cards with hover glow
- Custom Orbitron + Space Grotesk typography
- Cyan data stream animations on primary text
- Custom scrollbar with cyan accent

### 🖤 Obsidian — The Luxury Theme
*Pure volcanic black meets molten gold*

Premium, luxurious, and effortlessly elegant. No noise, no grit — just clean surfaces with warm amber accents that feel expensive. Smooth curves, subtle elevation, and a gold shimmer that moves across the background like light on obsidian glass.

**Key Features:**
- Ultra-premium color palette with gold accents
- Smooth card elevation with gold top-border on hover
- Playfair Display serif for headings, DM Sans for body
- Backdrop blur effects on header
- Minimal, elegant scrollbar
- Soft gold shimmer animation

### 💜 Zenith — The Minimalist
*Space black meets cosmic violet*

Ultra-minimal with cosmic violet accents. Breathing animations on cards, floating particle effects in the background, and monospace typography throughout. The most restrained theme in the pack — but every pixel serves a purpose.

**Key Features:**
- Floating particle field animation
- Breathing glow effect on card hover
- Ultra-compact layout with sharp edges
- Space Grotesk + IBM Plex Mono typography
- Subtle grid overlay
- Almost-invisible scrollbar

---

## 🎯 Philosophy

**Great themes aren't just color swaps.** They're complete design systems with:
- **Typography with intent** — every font choice serves readability and mood
- **Animation with purpose** — nothing decorative, everything functional
- **Depth through layering** — gradients, shadows, and glows create spatial hierarchy
- **Consistency across every surface** — cards, headers, tabs, badges, scrollbars

These themes use every feature the Hermes dashboard theme system supports: custom palettes, typography, layout variants, component styles, color overrides, assets, and raw CSS.

---

## 📦 Installation

```bash
# Clone the repo
git clone https://github.com/MarcosV6/hermes-noir-pack.git
cd hermes-noir-pack

# Install all three themes
cp *.yaml ~/.hermes/dashboard-themes/

# Restart your dashboard
hermes dashboard --restart

# Switch themes: open dashboard → palette icon in header → choose Aurora, Obsidian, or Zenith
```

**Or install a single theme:**
```bash
# Aurora only
cp aurora.yaml ~/.hermes/dashboard-themes/

# Obsidian only
cp obsidian.yaml ~/.hermes/dashboard-themes/

# Zenith only
cp zenith.yaml ~/.hermes/dashboard-themes/
```

---

## 🎨 Color Maps

### Aurora
| Variable | Hex | Role |
|----------|-----|------|
| `--color-primary` | `#3fd3ff` | Electric cyan — interactive elements, data streams |
| `--color-accent` | `#ffce3a` | Amber — warnings, highlights, alerts |
| `--color-card` | `rgba(10, 22, 40, 0.88)` | Deep indigo surface |
| `--color-border` | `rgba(63, 211, 255, 0.12)` | Hairline cyan separators |

### Obsidian
| Variable | Hex | Role |
|----------|-----|------|
| `--color-primary` | `#d4a853` | Warm gold — interactive elements |
| `--color-accent` | `#e8c878` | Light gold — highlights |
| `--color-card` | `rgba(12, 12, 12, 0.9)` | Volcanic black surface |
| `--color-border` | `rgba(212, 168, 83, 0.08)` | Subtle gold separators |

### Zenith
| Variable | Hex | Role |
|----------|-----|------|
| `--color-primary` | `#a78bfa` | Cosmic violet — interactive elements |
| `--color-accent` | `#c4b5fd` | Light violet — highlights |
| `--color-card` | `rgba(6, 6, 10, 0.9)` | Space black surface |
| `--color-border` | `rgba(167, 139, 250, 0.06)` | Barely-visible violet separators |

---

## 🔧 Technical Details

Each theme YAML file includes:
- **Palette** — 3-layer color system (background, midground, foreground) + warm glow + noise
- **Typography** — Google Fonts loading, custom font stacks, sizing, spacing
- **Layout** — Border radius, density, layout variant (cockpit/default)
- **Assets** — Custom gradient backgrounds, radial glows
- **Component Styles** — Card shapes (clip-path), backgrounds, shadows, borders
- **Color Overrides** — Full shadcn/ui token customization
- **Custom CSS** — Advanced animations, hover effects, scrollbars, selection colors

**Total CSS per theme:** 150-250 lines of production-quality styles
**Animation performance:** All animations use `transform` and `opacity` for GPU acceleration
**Browser support:** Modern browsers with CSS custom properties and backdrop-filter

---

## 🏆 Hackathon Submission

This pack demonstrates mastery of the Hermes dashboard theme system:
- ✅ All 7 YAML configuration sections used
- ✅ 3 distinct design languages (command center, luxury, minimalist)
- ✅ Advanced CSS animations (grid, particles, breathing, shimmer)
- ✅ Custom typography with Google Fonts integration
- ✅ Cockpit layout variant implementation
- ✅ Component-level styling (cards, headers, tabs, badges)
- ✅ Complete color system overrides
- ✅ Production-quality README with installation guide

---

## 📸 Previews

### Aurora
*Command center with animated grid and corner brackets*

### Obsidian
*Premium luxury with gold accents and smooth curves*

### Zenith
*Ultra-minimal with violet particles and breathing effects*

---

## 📝 Customization

Edit any YAML file directly. Key knobs:
- `palette.*` — Base colors and effects
- `typography.*` — Fonts and spacing
- `layout.*` — Radius, density, variant
- `componentStyles.*` — Card shapes, shadows, borders
- `colorOverrides.*` — Individual token colors
- `customCSS` — Add your own animations or effects

After editing, restart dashboard:
```bash
hermes dashboard --restart
```

---

## 📄 License

MIT © 2026 Marcos Vallejo

---

*"A dashboard should be a place you want to look at."* — Hermes Noir Pack
