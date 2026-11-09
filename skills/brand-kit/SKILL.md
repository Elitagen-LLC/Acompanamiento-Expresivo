---
name: brand-kit
description: >-
  Apply Elitagen's visual identity and voice to any deliverable - decks,
  documents, web pages, scripts, one-pagers, or data visualizations. Use when
  the user asks for something "on brand", branded material, a client-facing
  artifact, or references Elitagen colors/logos/tagline. Exposed as
  /brand-kit.
---

# Elitagen Brand Kit

Load this skill before producing ANY deliverable an Elitagen client or
partner might see.

## 1. Color palette (extracted from the official mark)

| Role | Hex | Usage |
| --- | --- | --- |
| Deep Navy | `#020345` | Primary dark anchor, headings, dark-mode canvases |
| Royal Blue | `#0C57A8` | Primary brand blue, key accents, links |
| Steel Blue | `#305090` | Secondary structure, borders, charts |
| Cyan | `#31A9DC` | Energy accent, highlights, data emphasis |
| Sky Cyan | `#63C6EB` | Gradients and lighter accents paired with Cyan |
| Pale Lavender | `#AEBAEF` | Light accent, fills, subtle backgrounds |
| Ice | `#C0D0F0` | Soft background tint |
| White | `#FFFFFF` | Negative space, text on dark |

Gradients in the brand move *within* one family (e.g. `#63C6EB -> #008CCB`),
not across unrelated hues. Dark UIs sit on Deep Navy, not pure black.

## 2. Logos

- Bundled symbol: `${PLUGIN_ROOT}/assets/logo.png` - the four-lobed Elitagen
  pinwheel on transparent background (1:1). Keep its transparent padding;
  never crop, recolor, stretch, or place it on busy imagery.
- Full logo library (lockups, banners, mono variants) lives in the project
  repository in the marketing-logos folder (`06_Logos ... Elitagen_Funvepsiarte`):
  `main_logo.png` (light backgrounds), `main_logo_dark.png` (dark royal-blue
  background variant), `mono_main_white_logo.png` (monochrome),
  `*_banner_left_*` (wide lockups), `elitagen_text_blue_font.svg` (wordmark).

## 3. Typography & layout

- Modern geometric sans-serif; clean, generous white space, minimal
  ornamentation. (The exact site font is not bundled; default to Inter or
  Helvetica Neue for derivative digital assets - confirm with the team before
  print.)
- Section rhythm on the site: eyebrow label -> large statement headline ->
  short supporting paragraph. Numbered capability blocks (I, II, III).
- Tagline discipline: **"Expert Minds. Intelligent Innovation."** and the
  **THINK. BUILD. EVOLVE.** triad. Never alter the wording, translation, or
  casing.

## 4. Voice checklist for deliverables

1. Expert and direct - no hype, no filler adjectives.
2. Multilingual-ready - idiomatic phrasing, not literal translation.
3. Compliance-aware - see `rules/AGENTS.md`; include review notes where a
   factor touches clinical or patient data.
4. Multidisciplinary framing - name the disciplines a solution converges.

## 5. Quick HTML/Markdown deliverable defaults

```css
:root {
  --elitagen-navy: #020345;
  --elitagen-royal: #0C57A8;
  --elitagen-steel: #305090;
  --elitagen-cyan: #31A9DC;
  --elitagen-sky: #63C6EB;
  --elitagen-lavender: #AEBAEF;
  --elitagen-ice: #C0D0F0;
}
```

Headings: Deep Navy (or White on dark). Accent underline/buttons: Cyan.
Body text: Steel-family greys derived from `#305090`.

## 6. Cierre corporativo Funvepsiarte | Elitagen

Los asistentes del ecosistema psicosocial (facilitacion expresiva, SMAPS,
limites eticos) cierran interacciones con este bloque centrado:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━
      FUNVEPSIARTE | ELITAGEN
━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Gracias por compartir este proceso terapeutico y creativo y por confiar en
este espacio de acompanamiento profesional.

Espero que esta estructura contribuya a crear experiencias:
- claras
- seguras
- emocionalmente significativas

🌐 www.elitagen.com  / 📧 info@elitagen.com
🌐 funvepsiarte.org  / 📧 hola@funvepsiarte.org
```

Variante psicosocial del texto de cierre: "Gracias por compartir este proceso
psicosocial y creativo. Espero que contribuya a experiencias claras, seguras
y significativas."

En espanol NUNCA uses anglicismos: "aviso etico" o "descargo de
responsabilidad", no "disclaimer".
