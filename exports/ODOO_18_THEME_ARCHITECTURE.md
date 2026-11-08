# EIGENKERN - Odoo 17 / 18 Website Theme & Snippet Architecture

## Recommended Base Template & Technical Rationale (2-3 Sentences for Contest Brief)
We recommend building this design on Odoo's official **`theme_default` (Odoo 17/18 Blank Starter Theme)** layered directly onto Odoo's native **Bootstrap 5.3 SCSS token system (`$o-color-palettes`, `$o-theme-font-configs`)** rather than modifying a bloated commercial theme. This guarantees 100% compatibility with the Odoo Website Builder drag-and-drop editor (`data-snippet`), native mobile grid responsiveness, and zero external requests by serving `Plus Jakarta Sans` and `IBM Plex Mono` as local `.woff2` files from `/theme_eigenkern/static/src/fonts/` for strict German DSGVO compliance. All custom blocks (including the *Wächter* Shadow-Copy diagram and the 3-Ways comparison matrix) are structured as modular XML `<template>` building blocks (`s_eigenkern_hero`, `s_eigenkern_waechter`, `s_eigenkern_drei_wege`) so the EIGENKERN team can edit all German copy and links directly in the Odoo visual editor.

## Color Palette & WCAG Contrast Tokens (`primary_variables.scss`)
- `$eigenkern-ink`: `#0F172A` (Anthracite Slate - WCAG AAA 16.4:1 on `#F6F8FA`)
- `$eigenkern-surface`: `#F6F8FA` (Architectural Alabaster)
- `$eigenkern-card`: `#FFFFFF` (Pure Crisp Surface)
- `$eigenkern-cobalt`: `#0047BA` (Sovereign German Engineering Cobalt - WCAG AA 7.8:1)
- `$eigenkern-emerald`: `#0D7A5F` (Local Hardware / DSGVO Security Status - WCAG AA 5.2:1)
