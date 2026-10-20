# Tillgänglighetsrapport – Linnea Ek Fotografi

## 1. Arbetsprocess och samarbete

Arbetet började med att skapa en grundstruktur, fördela uppgifterna och komma överens om hur samarbetet skulle fungera.

Varje gruppmedlem arbetade i sin egen branch på GitHub. Planen var att använda pull requests, granska varandras kod och sedan göra merge till main.

Samarbetet fungerade bra och problem som uppstod löstes genom diskussioner och gemensamma beslut.

## 2. Problem och lösningar

**SCSS-struktur**

Från början fanns en gemensam plan för SCSS-strukturen, men eftersom Sass var nytt för oss hade inte alla detaljer diskuterats tillräckligt noggrant.

Ibland glömdes understrecket (`_`) framför filnamnen för våra partials, vilket ledde till att extra CSS-filer skapades vid kompileringen.

När orsaken upptäcktes rättades filnamnen och strukturen. Nu samlas alla partials via `@use` i `style.scss` och kompileras till en gemensam `style.css`, precis som planerat.

**SEO och meta description**

Vid Lighthouse-testerna upptäcktes att saknade meta descriptions påverkade SEO-resultatet negativt.

Efter att meta descriptions lagts till på alla sidor förbättrades resultatet direkt vid nästa test.

**Kontrastproblem**

Ett kontrastproblem upptäcktes i samband med en bild. Genom att byta bilden kunde problemet lösas och kontrastkontrollen godkändes.

**Tangentbordsnavigation**

Vid testning med Tab upptäcktes att fokusmarkeringen på vissa knappar inte syntes tillräckligt tydligt.

Problemet diskuterades och en gemensam lösning togs fram. Koden delades inom gruppen och fokusmarkeringarna anpassades för bättre synlighet.

**Gemensam design**

Mot slutet upptäcktes att H1-rubrikerna hade lite olika utseende. Efter diskussion justerades stilarna för att skapa en mer enhetlig design.

Det blev också tydligt att fler gemensamma mixins från början hade underlättat arbetet. Eftersom projektet nästan var färdigt valde vi att justera stilarna direkt i stället för att ändra hela SCSS-strukturen.

## 3. Tester och resultat

Följande tester genomfördes enligt examinationsuppgiften:

- **Lighthouse:** 95–100 poäng i Performance, Accessibility, Best Practices och SEO enligt de slutliga testerna.
- **W3C HTML Validator:** Inga fel vid slutkontrollen.
- **Responsivitet:** Webbplatsen byggdes enligt mobile-first-principen och testades på mobil, surfplatta och dator. Ingen oönskad horisontell scrollning upptäcktes.
- **Zoom:** Webbplatsen testades vid 200 % och 400 % zoom. Text och innehåll var fortsatt synliga och läsbara, och webbplatsen gick att använda.
- **Tangentbordsnavigation:** Alla sidor testades med Tab och fokusmarkeringarna kontrollerades.
- **Skärmläsare:** Innehåll, navigation och bildbeskrivningar testades och fungerade på ett begripligt sätt.
- **Kontrast:** Kontrasten kontrollerades och upptäckta problem åtgärdades.

Vi har även arbetat med följande WCAG 2.2-kriterier:

- **1.1.1 Non-text Content:** Beskrivande alt-texter för bilder.
- **1.4.3 Contrast (Minimum):** Tillräcklig kontrast mellan text och bakgrund.
- **2.1.1 Keyboard:** Webbplatsen ska gå att använda med tangentbord.
- **2.4.7 Focus Visible:** Tydliga fokusmarkeringar vid tangentbordsnavigation.

## 4. Reflektion och slutsats

Samarbetet har fungerat bra och projektet har gett värdefull erfarenhet av Sass, tillgänglighet och GitHub.

En viktig lärdom är att planera den gemensamma SCSS-strukturen mer detaljerat från början och använda fler gemensamma mixins och variabler.

Under arbetet hände det också några gånger att ändringar mergades utan pull request, vilket avvek från både uppgiftens krav och vår överenskomna arbetsprocess. För att undvika detta i framtiden vill vi använda branch protection rules på GitHub, så att pull requests krävs innan ändringar kan mergas till main.

Granskning och kommentarer på varandras pull requests är också något som kan förbättras till nästa grupparbete.

Projektet har varit lärorikt. De problem vi upptäckte hanterades längs vägen, och de slutliga testerna gav goda resultat.