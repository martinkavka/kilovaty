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
docs/              # Web kilovaty.cz (GitHub Pages servíruje z /docs, pojmenování je GH Pages konvence)
presentations/     # Prezentace na školení a konference
workshops/         # Materiály k offline workshopům (prezentace .pptx, handouty .docx, cvičení)
```

**Pozor na pojmenování `docs/`:** Je to vynucená konvence GitHub Pages, ne dokumentace. Když migrujeme na Cloudflare Pages (viz níže), složku přejmenujeme na `web/`.

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
- **Jediný CSS soubor:** `docs/style.css` — všechny komponenty a styly na jednom místě.
- **Design tokens** jsou definované přímo v `:root` v `style.css` (ne v externím souboru).
- **Fonty:**
  - Bricolage Grotesque — nadpisy (`--font-heading`)
  - Source Sans 3 — běžný text (`--font-body`)
- **Barvy:** `--bg: #FFFDF7`, `--bg-warm: #F5F0E6`, `--bg-dark: #1A1714`, `--accent: #C2410C`, `--ink: #1A1714`, `--ink-soft`, `--ink-mute`, `--ink-inverse: #FFFDF7`
- **Responzivní breakpoint:** 1024 px — gridy (services, stats, ba, quotes, pricing, blog) přepínají na 1 sloupec; services-header se centruje; ba-arrow přechází z absolute na static flow
- **Max-width:** Sekce `.s`, `.hero`, `.page-header` používají `padding-inline: max(56px, 50% - 720px)` pro omezení obsahu na ~1440px na širokých monitorech. Nav a footer mají `max-width` na inner wrapperu.
- **Logo:** 90px výška v navigaci
- **České uvozovky:** vždy „ (U+201E) a " (U+201C), nikdy ASCII ". **Pozor:** nikdy nepoužívat typografické uvozovky (U+201C/U+201D) v HTML atributech — jen rovné `"`. Typografické uvozovky v atributech rozbijí CSS třídy.
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
docs/
  index.html                      # Homepage
  o-nas.html                      # O nás + příběh + zakladatelé + služby nudge
  sluzby.html                     # Přehled služeb + roční program pricing + FAQ
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
  kontakt.html                    # Kontakt + Calendly + formulář
  kontakt-diky.html               # Thank-you po odeslání formuláře
  kurz.html                       # Lead magnet landing — mini-kurz 5 lekcí
  kurz-diky.html                  # Thank-you po přihlášení do kurzu
  style.css                       # Jediný CSS soubor
  assets/
    photos/                        # Fotky zakladatelů a recenzentů
    logo/                          # Loga Kilovaty
```

### Konverzní architektura

- **Každá stránka má CTA sekci** (tmavé pozadí, "Domluvit schůzku" → `kontakt.html#schuzka`).
- **Homepage:** Hero → Trusted logos → Before/After → Stats → Problem/Solution → Služby (3 karty + upsell roční program) → Testimonial → Mini-kurz (lead magnet) → Quotes → CTA.
- **Služby detail:** Popis → Pro koho → Co získáte (`.benefit-grid` dlaždice) → Jak to probíhá (`.timeline` vizuální časová osa) → Cena + `.roi-box` (návratnost) → Testimonial → Cross-sell (2 další služby) → CTA. Sticky CTA bar po 400px scrollu.
- **sluzby.html:** Přehled workshopů → další služby → roční program pricing → **FAQ sekce (8 otázek, native `<details>`)** → CTA.
- **testovani.html:** Má navíc `.package-box` s rozpisem „V ceně" pro interní a externí testování.
- **Blog:** "Akademie srozumitelnosti" — kuratovaný, bez dat. **Nahoře `.kurz-promo` widget** (lead magnet) → featured karty → tematické sekce → interlude (odkaz na workshop) → širší kontext. Každý článek má cílené article-cta (mapované na relevantní službu) + 2 related články.
- **O nás:** Příběh → Co děláme → Timeline → Zakladatelé → Quotes → Služby karty → CTA.
- **Kontakt:** Calendly widget s micro-proof (citát Janků) → **formulář „Raději napište" (Web3Forms)** → kontaktní údaje + fakturační údaje → CTA.
- **Lead magnet** (`kurz.html`): 5 lekcí srozumitelného psaní jako PDF. Formulář (Web3Forms) → `kurz-diky.html` → PDF se posílá mailem. Promo widget `.kurz-promo` na homepage (vlastní sekce) a na blog.html (nahoře, bg-warm).

### Formuláře a Web3Forms

Dva formuláře (`kontakt.html`, `kurz.html`) posílají přes **Web3Forms** (unlimited free tier). Oba mají:
- `action="https://api.web3forms.com/submit"`, method POST
- Hidden `access_key` — **placeholder `DOPLNIT-WEB3FORMS-KEY`**, musí se doplnit reálný klíč z web3forms.com
- Hidden `redirect` — URL thank-you stránky (aktuálně `martinkavka.github.io/kilovaty/...`, po migraci změnit na `kilovaty.cz/...`)
- Honeypot pole `botcheck` (schovaný checkbox)
- GDPR checkbox s odkazem na mail pro odhlášení
- Submit button plné šířky s šipkou

Thank-you stránky (`kontakt-diky.html`, `kurz-diky.html`) mají `noindex` meta a navádějí na další krok (blog, workshop, druhý magnet).

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
- `.benefit-grid` / `.benefit-tile` — 2-sloupcový grid dlaždic (1 sloupec mobil). Warm pozadí, accent border-left. Používá se na všech service detail stránkách pro „Co získáte" / „Proč se vyplatí" / „Co měříme".
- `.timeline` / `.timeline-step` / `.timeline-num` / `.timeline-content` — vizuální časová osa se svislou čárou a accent kolečky s čísly. Používá se na všech service detail stránkách pro „Jak to probíhá". Pozor: uvnitř `.content` je potřeba override `.content ol.timeline` kvůli specificitě.
- `.roi-box` — accent-light pozadí, border-left, eyebrow „VRÁTÍ SE VÁM TO" / „PROČ SE TO VYPLATÍ" + krátká kalkulace návratnosti. Na každé service detail stránce před cenou.
- `.package-box` — warm pozadí, border-left, cena + seznam „V ceně" s checkmarkem. Používá se na testovani.html pro rozpis interního/externího balíčku.
- `.faq-list` / `.faq-item` — native HTML5 `<details>`/`<summary>` accordion, žádný JS. Plusko/mínusko indikátor. Používá se na sluzby.html.
- `.contact-form-wrap` / `.contact-form` / `.form-field` / `.form-check` — styling formuláře. Card container s padding + rounded, labely display:block nad inputy, input 100% width, focus accent border. `.form-row` je 2-sloupcový grid pro dvojice polí.
- `.kurz-promo` — lead magnet widget (strong + span + button). Default pozadí `var(--bg)` (krémová), border-left accent. Na homepage ve vlastní sekci, na blogu inline override na `var(--bg-warm)`.
- `.diky-hero` — centrovaný hero pro thank-you stránky (větší H1, krátký podtitul, 2 button akce).

## Nasazení a deploy

**Aktuální stav:** GitHub Pages, servíruje z `docs/` na branchi `main`. URL: `https://martinkavka.github.io/kilovaty/`. Deploy trvá 2–5 minut po pushi.

**Plánovaná migrace → Cloudflare Pages** (až si Martin a Dalibor odsouhlasí finální verzi webu):
1. Cloudflare dashboard → Pages → Connect to Git → repo `martinkavka/kilovaty`
2. Build settings: framework None, output directory `docs/`
3. Připojit doménu `kilovaty.cz` (Cloudflare DNS to zvládne bez čekání)
4. Po migraci: přejmenovat `docs/` na `web/` (konvence GH Pages tam už nebude potřeba) a aktualizovat output directory v Cloudflare
5. **Aktualizovat redirect URL** ve formech `kontakt.html` a `kurz.html` z `https://martinkavka.github.io/kilovaty/...` na `https://kilovaty.cz/...`

**Proč Cloudflare, ne Vercel:** Martin už má Cloudflare účet a další weby, unlimited bandwidth ve free tieru (Vercel 100 GB), global CDN rychlejší než GH Pages.

**Commit a push:** Neprováděj automaticky. Stage explicitně jen to, co se opravdu změnilo — složky jako `workshops/` nebo `_raw/` nikdy nestage do webových commitů.

## Fáze projektu

> Tato sekce je interní kontext pro orientaci v prioritách. Termíny a fáze se nikdy nepromítají do produkčních textů, webu ani prezentací.

**Web kilovaty.cz:** Všech 28 stránek hotových, konverzně optimalizované (3 kola UX/CRO auditu). Nasazeno na GitHub Pages (martinkavka.github.io/kilovaty/). Dalibor kontroluje na velkém monitoru.

**Čeká na dokončení (blokuje live provoz formulářů):**
1. **Web3Forms access-key** — registrace na web3forms.com, doplnit do `kontakt.html` a `kurz.html` (placeholder `DOPLNIT-WEB3FORMS-KEY`)
2. **PDF mini-kurzu** — vytvořit z `_raw/email-kurz-lead-magnet.docx` (5 lekcí), nahrát někam (drive/autoresponder), nastavit ve Web3Forms autoresponder s linkem

**Akutně:**
1. Prezentace na školení (16. 4. 2026)
2. Dokončení bodů výše, ať formuláře funkčně sbírají leady

**Po odsouhlasení webu:**
- Migrace na Cloudflare Pages (viz oddíl „Nasazení a deploy")
- Přejmenovat `docs/` → `web/`
- Připojit doménu `kilovaty.cz`

**Postupně podle potřeby:**
- Případové studie (1–2 s měřitelnými výsledky od PRE nebo CRR)
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
