---
title: Poznámky pro stavbu webu
description: Audit přístupnosti a UX/konverze z moodboard fáze. Opravit před/při stavbě webu.
---

# Poznámky pro stavbu webu

Z auditu moodboardu (duben 2026). Opravit při stavbě webu.

## Přístupnost

### Kontrasty (WCAG AA minimum 4.5:1)

- **Škrtnutý text** — dekorativní, ale i tak by měl být čitelný. Aktuální `ink-mute` (40% opacity) dává jen 2.5:1. Zvednout na min. 55–60% nebo řešit jinak.
- **Before/after „before" text** — stejný problém. Musí být čitelný, i když vizuálně ustupuje.
- **CTA podtext na tmavém pozadí** — `rgba(255,253,247,0.45)` = 4.4:1. Těsně pod AA. Zvednout na 0.55+.
- **CTA e-mail na tmavém pozadí** — `rgba(255,253,247,0.25)` = 2.2:1. Výrazně pod. Zvednout na 0.55+.
- **Accent (#C2410C) na bg-warm** — 4.6:1. Projde AA, ale je těsné. Zvážit tmavší variantu accentu pro warm sekce.

### Chybějící prvky

- **Focus stavy** — `:focus-visible` na všechny interaktivní prvky (odkazy, tlačítka, formuláře). Viditelný outline, ne jen `outline: none`.
- **Skip-to-content link** — skrytý odkaz na začátku stránky pro klávesovou navigaci.
- **Mobilní menu** — hamburger tlačítko, menu se schová ale není čím ho otevřít.
- **Alt texty** — na všechny obrázky (loga klientů, fotky zakladatelů).
- **Sémantické HTML** — správné heading levels (h1→h2→h3), landmarky (`<main>`, `<nav>`, `<footer>`), `<button>` místo `<div onclick>`.
- **Aria labels** — na ikonová tlačítka a dekorativní prvky.

## UX / Konverze

### CTA strategie

- **Sjednotit CTA** — „Domluvit schůzku" / „Chci workshop" / „Vybrat termín" jsou tři různé formulace pro jednu akci. Vybrat jednu hlavní a jednu sekundární.
- **Kontakt viditelný bez scrollu** — telefon nebo e-mail v nav nebo hero. Klient, který chce rychle zavolat, nesmí scrollovat na konec.
- **Služby potřebují CTA** — každá karta služby by měla mít vlastní tlačítko/odkaz na další krok.

### Social proof

- **Jedna citace blíž k CTA** — ne až na konci stránky. Ideálně vedle nebo pod službami.
- **Loga klientů** — textová jména působí slabě. Loga (i jednobarevná) posílí důvěryhodnost.

### Navigace

- **Nav hover** — musí být vizuálně odlišný od výchozího stavu. Aktuálně je hover = default.
- **Ghost button v hero** („Co děláme") — musí být jasné, kam vede. Anchor link dolů? Jiná stránka?
