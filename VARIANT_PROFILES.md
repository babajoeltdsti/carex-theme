# Carex Variant Profiles

## Purpose

This file helps you pick the right Carex setup based on your environment, display type, and workflow.

## Core Profiles

### Carex Dark

- Best for: all-around daily dark theme use
- Pair with: Carex File Icons + Carex Product Icons
- Recommended for: TypeScript, Python, backend work, long sessions

### Carex Light

- Best for: bright rooms and daytime coding
- Pair with: Carex File Icons + Carex Product Icons
- Recommended for: docs, dashboards, product work, general office use

### Carex OLED

- Best for: OLED panels and users who want near-true black surfaces
- Pair with: reduced screen brightness and smooth cursor animations
- Recommended for: low-light setups and battery-sensitive laptop use

### Carex Dusk

- Best for: warmer dark-theme preference
- Pair with: medium contrast editor settings
- Recommended for: reading-heavy sessions and late-night work

### Carex Dawn

- Best for: soft light-theme preference
- Pair with: slightly larger line height and muted icon themes
- Recommended for: writing, review sessions, and documentation

### Carex Neon

- Best for: screenshots, social sharing, and high-energy setups
- Pair with: bracket pair colorization enabled
- Recommended for: frontend demo work and visual punch

## Accessibility Profiles

### Carex High Contrast Dark

- Best for: maximum contrast on dark backgrounds
- Recommended for: strong separation between tokens and UI regions

### Carex High Contrast Light

- Best for: bright environments with strong text separation
- Recommended for: high-clarity daytime use

### Carex Deuteranopia Friendly

- Best for: users who benefit from blue-orange-purple differentiation
- Recommended for: language-heavy workflows with many semantic categories

### Carex Protanopia Friendly

- Best for: users who prefer cyan-gold-lilac separation
- Recommended for: strong readability without red-led contrast dependence

### Carex Low Distraction

- Best for: quiet, muted focus work
- Recommended for: writing, refactors, long maintenance sessions

## Suggested Settings

```json
{
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.renderLineHighlight": "all",
  "editor.minimap.enabled": true,
  "workbench.iconTheme": "carex-file-icons",
  "workbench.productIconTheme": "carex-product-icons"
}
```