# Kilovaty – Monorepo

## O projektu

Monorepo firmy **Kilovaty s.r.o.** — konzultantů a lektorů srozumitelného psaní (plain language). Dva zakladatelé: Martin Kavka a Dalibor Behún.

Repo obsahuje veškerý firemní obsah a výstupy: web, prezentace, e-maily, materiály pro sociální sítě.

## Struktura

```
_raw/              # Surové podklady (gitignored) — NEUPRAVOVAT
content/           # Strukturovaný obsah v Markdownu (single source of truth)
  pages/           # Stránky webu (homepage, o nás, kontakt)
  services/        # Služby (workshopy, testování, editace, roční plán)
  people/          # Bio zakladatelů
  data/            # Sdílená data (klienti, recenze, statistiky)
  blog/            # Články
brand/             # Vizuální identita, tokeny, hlas značky
  tokens.css       # Design tokens (barvy, typografie, spacing)
  voice.md         # Detailní pravidla hlasu značky
web/               # Web kilovaty.cz
presentations/     # Prezentace na školení a konference
```

## Jazyk a tón

Detailní pravidla hlasu značky budou v `brand/voice.md` — až bude tento soubor existovat, vždy si ho načti před jakoukoli prací s textem.

Veškerý obsah je v **češtině**, pokud není výslovně řečeno jinak.

Kilovaty učí srozumitelné psaní. Vlastní texty musí být vzorem toho, co hlásáme.

### Jak to celé máš brát

Principy níže nejsou checklist. Jsou to instinkty.

Nesvazuj texty do kozelce. Cílem není *„splnit všech pět bodů"*,
ale psát tak, aby Kilovaty působily **čerstvě, neformálně, jako
profíci, se kterými lidé chtějí trávit čas.**

Reference:

- **Harry Dry** (Marketing Examples) — velmi krátké věty, často
  jedno slovo na řádek. Konkrétní příklady místo teorie. Humor
  v rytmu a formátu, ne v hláškách. Ukázat, ne vysvětlit.
- **Alex Hormozi** — přímý, faktický, brutálně upřímný bez krutosti.
  Kontrast a čísla. „Tady je co dělat a proč to funguje."

Když si nejsi jistý tónem, zeptej se: *Znělo by tohle jako Harry Dry
nebo Alex Hormozi, kdyby psal česky?* Když ne — zkrať, uber na
opatrnosti, přidej rytmus.

Kilovaty jsou firma, které se daří, protože si s námi lidé rádi
povídají. Nesnaž se za každou cenu být vtipný. Ale taky nebuď sterilní.

### Pět principů hlasu

**1. Krátké věty. Tečka je kamarád.**
Priorita je rytmus a srozumitelnost. Většina vět krátká, úderná. Občas delší věta pro rytmus — to je OK, ale nikdy na úkor jasnosti.

- místo: *„V rámci naší dlouholeté praxe v oblasti srozumitelného psaní jsme dospěli k závěru, že klíčovým faktorem úspěšné komunikace je jednoduchost."*
- → píšeme: *„Jednoduchost funguje. Víme to z praxe."*

**2. Konkrétní čísla a fakta. Žádné mlhavé fráze.**
Číslo přesvědčí víc než přídavné jméno. Fakt víc než superlativ.

- místo: *„Naše workshopy mají skvělé výsledky a účastníci jsou velmi spokojení."*
- → píšeme: *„Workshop trvá 6 hodin. Vedou ho 2 lektoři. Maximálně 15 lidí ve skupině. Pracujete na vlastních textech."*

**3. Sebevědomí bez arogance.**
Víme, co umíme. Nemusíme to dokazovat superlativy. Výsledky mluví za nás.

- místo: *„Jsme přední a nejlepší odborníci na srozumitelné psaní v České republice."*
- → píšeme: *„Jsme jedni z mála v Česku, kteří se srozumitelnému psaní systematicky věnují."*

**4. Přeškrtnutá vata.**
Kilovaty používají konkrétní textovou a vizuální metodu: přeškrtávají úřednické a vatové obraty, aby pod nimi víc vystoupila srozumitelná věta. Je to pedagogická metoda z workshopů převedená do designu a textu. Přeškrtává se celý úřednický blok včetně spojky, aby výsledná věta stála samostatně a měla punch. Kontrast dělá pointu.

Kde to používáme:
- hero nadpisy na webu
- before/after bloky (úřednický originál vs. přepsaná verze)
- ukázky cvičení z workshopů
- občas i v nadpisech postů a prezentací

- místo: *„Tímto vám sdělujeme, že vaše texty nikdo nečte."*
- → píšeme: *„~~Tímto vám sdělujeme, že~~ Vaše texty nikdo nečte."*

**5. Lidský humor v patičce.**
Zápatí, poděkování, chybové hlášky, potvrzovací e-maily — všude, kde to jde, přidáme lidský tón.

- místo: *„© 2025 Kilovaty s.r.o. Všechna práva vyhrazena."*
- → píšeme: *„© 2025 Kilovaty s.r.o. Tento web běží díky litrům kávy a lásce k dobrému psaní."*

### Zakázaná slova

Tyto fráze nikdy nepoužíváme. Jsou to přesně ten typ vaty, který pomáháme likvidovat:

- synergie
- komplexní řešení
- na klíč
- holistický přístup
- zdvořile žádáme
- v návaznosti na výše uvedené
- tímto Vás informujeme
- revoluční
- transformační
- disruptivní
- špičkový

### Vzorky hlasu v kontextu

| Kontext | Místo tohoto… | …píšeme tohle |
|---|---|---|
| Hero nadpis | *Komplexní řešení firemní komunikace* | *Pište srozumitelně. Vyplatí se to.* |
| Popis služby | *Náš workshop poskytuje účastníkům komplexní vhled do problematiky efektivní písemné komunikace.* | *Naučíme váš tým psát texty, které každý pochopí na první přečtení. Za 6 hodin.* |
| CTA | *Neváhejte nás kontaktovat pro více informací.* | *Bojujete s vatou? Napište nám.* |
| Potvrzovací e-mail | *Vážený kliente, tímto Vám potvrzujeme přijetí Vaší objednávky. O dalším postupu Vás budeme informovat.* | *Máme to. Ozveme se do 24 hodin s dalšími detaily.* |
| Patička | *Děkujeme za Váš zájem. Těšíme se na spolupráci.* | *Díky, že čtete až sem. Většina lidí to vzdá u třetího odstavce.* |

## Pravidla pro obsah

- **Jediný zdroj pravdy je `content/`.** Web, prezentace a další výstupy
  čerpají obsah odtud. Když upravím cenu workshopu, upravuji ji tam,
  ne na webu.
- **`_raw/` je archiv podkladů.** Nikdy ho neupravuj, nemazej z něj,
  nepřidávej do gitu. Slouží jen jako reference.
- **Obsahová pravidla jsou v sekci „Jazyk a tón" výše** a detailně budou
  v `brand/voice.md`.
- **Nikdy si nevymýšlej čísla, statistiky, procenta ani citace.** Pokud
  nemáš v podkladech reálné číslo, napiš větu bez čísla, nebo se zeptej.
  Kilovaty prodávají důvěryhodnost — jedno vymyšlené číslo ji rozbije.

## Pravidla pro kód

- **Vanilla HTML + CSS, bez build stepu.** Žádný framework, bundler ani preprocesory, pokud to nebude výslovně schváleno.
- **Jediný CSS soubor:** `web/style.css` — všechny komponenty a styly na jednom místě.
- **Design tokens** jsou definované přímo v `:root` v `style.css` (ne v externím souboru).
- **Fonty:**
  - Bricolage Grotesque — nadpisy (`--font-heading`)
  - Source Sans 3 — běžný text (`--font-body`)
- **Barvy:** `--bg: #FFFDF7`, `--bg-warm: #F5F0E6`, `--bg-dark: #1A1714`, `--accent: #C2410C`, `--ink: #1A1714`, `--ink-soft`, `--ink-mute`, `--ink-inverse: #FFFDF7`
- **Responzivní breakpoint:** 1024 px — gridy (services, stats, ba, quotes, pricing, blog) přepínají na 1 sloupec; services-header se centruje; ba-arrow přechází z absolute na static flow
- **České uvozovky:** vždy „ (U+201E) a " (U+201C), nikdy ASCII "
- **Přístupnost:**
  - Kontrastní poměr minimálně 4.5:1
  - Sémantické HTML (správné heading levels, landmarky, `<button>` místo `<div onclick>`)
  - Viditelné focus stavy na všech interaktivních prvcích
  - Skip-to-content link na každé stránce
  - Alt texty na všech obrázcích
  - Mobilní hamburger menu s `aria-expanded`

## Web kilovaty.cz — stav a architektura

Web je **z velké části hotový** (duben 2026). Všechny stránky existují a jsou konverzně optimalizované.

### Struktura souborů

```
web/
  index.html                      # Homepage
  o-nas.html                      # O nás + příběh + zakladatelé + služby nudge
  sluzby.html                     # Přehled služeb + roční program pricing
  sluzby/
    jak-psat.html                  # Workshop hlavní (bestseller)
    psani-s-ai.html                # Workshop AI
    emaily.html                    # Workshop e-maily
    testovani.html                 # Testování srozumitelnosti
    editace.html                   # Editace textů (s before/after ukázkou)
    konzultace.html                # Konzultace
    srozumitelna-organizace.html   # Roční program (3 cenové varianty)
  blog.html                       # Blog index (Akademie srozumitelnosti)
  blog/
    01-naklady.html … 13-digitalizace.html  # 13 článků
  kontakt.html                    # Kontakt + Calendly widget
  style.css                       # Jediný CSS soubor
  assets/
    photos/                        # Fotky zakladatelů a recenzentů
    logo/                          # Loga Kilovaty
```

### Konverzní architektura

- **Každá stránka má CTA sekci** (tmavé pozadí, "Domluvit schůzku" → `kontakt.html#schuzka`).
- **Homepage:** Hero → Stats → Problem/Solution → Before/After → Služby (3 karty + upsell roční program) → Testimonial → Quotes → CTA.
- **Služby detail:** Popis → Pro koho → Co získáte → Jak to probíhá (4 kroky) → Cena → Testimonial → Cross-sell (2 další služby) → CTA. Sticky CTA bar po 400px scrollu.
- **Blog:** "Akademie srozumitelnosti" — kuratovaný, bez dat. Featured karty → tematické sekce → interlude (odkaz na workshop) → širší kontext. Každý článek má cílené article-cta (mapované na relevantní službu) + 2 related články.
- **O nás:** Příběh → Co děláme → Timeline → Zakladatelé → Quotes → Služby karty → CTA.
- **Kontakt:** Calendly widget s micro-proof (citát Janků) + kontaktní údaje + fakturační údaje.

### Testimonials — mapování na stránky

6 recenzí rozmístěných po webu, každá na relevantním místě:
- **Reedová** (Centrum pro regionální rozvoj) → homepage featured testimonial, testovani.html, srozumitelna-organizace.html
- **Janků** (Ústavní soud) → homepage quotes, sluzby.html featured, emaily.html, kontakt.html micro-proof
- **Syručková** (SUZ MV) → homepage quotes, jak-psat.html
- **Bendová** (marketing) → homepage quotes, psani-s-ai.html
- **Svatoňová** → editace.html
- **Precek** → konzultace.html

### Blog article-CTA mapování

Každý blogpost má cílené CTA směřující na relevantní službu:
- Technické články (03, 04, 06, 07, 12) → workshop jak-psat.html
- Testování (02, 05) → testovani.html
- E-maily (09) → emaily.html
- Jazyk (08, 10) → editace.html
- Konceptuální (01, 11, 13) → kontakt.html#schuzka

### Vizuální vzory (CSS komponenty)

- `.ba-grid` — Before/After porovnání (2 sloupce desktop, 1 sloupec mobil). Ručně kreslená SVG šipka mezi panely (absolutně pozicovaná na desktopu, v grid flow na mobilu s negativním marginem pro přesah do obou sekcí). Škrty v Před panelu používají SVG vlnovku jako `background-image` (ne rovné čáry) — text je rozdělen do více `.x` spanů, liché/sudé mají jinou vlnovku.
- `.service` / `.service--featured` — karty služeb s badge "Bestseller".
- `.featured-testimonial` — velký testimonial pod sekcí služeb.
- `.service-testimonial` — menší testimonial na detail stránkách (max-width 760px, border-left accent).
- `.blog-featured` — 3-sloupcový grid featured článků.
- `.blog-cards` — 2-sloupcový grid článků s pull quotes.
- `.blog-interlude` — vizuální přerušení v blogu s CTA na workshop.
- `.article-cta` — cílená CTA box uvnitř blogpostu.
- `.related` — sekce "Čtěte dál" s 2 souvisejícími články.
- `.sticky-cta` — fixní CTA bar na service detail stránkách.
- `.calendly-reassurance` — micro-proof nad Calendly widgetem.
- `.services-upsell` — jednořádkový odkaz na roční program / všechny služby.

## Fáze projektu

> Tato sekce je interní kontext pro orientaci v prioritách. Termíny a fáze se nikdy nepromítají do produkčních textů, webu ani prezentací.

**Web kilovaty.cz:** Všechny stránky hotové, konverzně optimalizované (2 kola UX/CRO auditu). Zbývá finální vizuální ladění a nasazení.

**Akutně:**
1. Dokončení webu — poslední vizuální úpravy, nasazení
2. Prezentace na školení (16. 4. 2026)

**Postupně podle potřeby:**
- E-mailové šablony
- Materiály pro sociální sítě
- Další výstupy

Nepředbíhej — řeš to, co je na řadě.

## Fakta o firmě

- **Název:** Kilovaty s.r.o.
- **IČ:** 23686316
- **Sídlo:** Nad Přívozem 1681/3, Praha 4, 147 00
- **E-mail:** jsme@kilovaty.cz
- **Telefon:** +420 605 412 328 (Martin), +420 737 383 671 (Dalibor)
- **Web:** kilovaty.cz
- **Založeno:** září 2025

### Služby

1. **Workshop „Jak psát, aby to fakt četli"** — 6h, 2 lektoři, max 15 účastníků, 39 900 Kč
2. **Workshop „Psaní s AI, které nezní jako od AI"** — 4h, 29 900 Kč
3. **Workshop „Jak psát e-maily, které šetří čas"** — 4h, 29 900 Kč
4. **Testování srozumitelnosti textů** — od 25 900 Kč (interní) / 29 900 Kč (externí)
5. **Editace** — přepis textů do srozumitelné podoby
6. **Konzultace** — on-line nebo osobně
7. **Roční program „Srozumitelná organizace"** — 3 varianty (19 900 / 29 900 / 39 900 Kč/měs.)

### Klienti

PRE, Generali Česká pojišťovna, IKEA, Nadace OSF, Ministerstvo vnitra, Ministerstvo spravedlnosti, Ministerstvo pro místní rozvoj, SUZ MV, Centrum pro regionální rozvoj ČR

### Zakladatelé

- **Martin Kavka** — expert na obsahové projekty, newslettery a e-mailovou komunikaci. Bývalý novinář. Projekty: Newslettery.cz, Promptně, Tvůrcast, Čeština 2.0.
- **Dalibor Behún** — překladatel, jazykový korektor a copywriter. Spoluautor knih *Pište správně česky* a *Pište čtivě a srozumitelně*.

## Technické konvence

- Commit messages v češtině, imperativní způsob
- Git author: `kavka.martin@gmail.com`
- Necommituj a nepushuj automaticky — vždy se zeptej
- Soubory v `_raw/` jsou v `.gitignore` — nepatří do gitu
