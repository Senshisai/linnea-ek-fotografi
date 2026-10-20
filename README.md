# Linnea Ek Fotografi

En responsiv och tillgänglig webbplats för Linnea Ek Fotografi, byggd utifrån uppgiftens mockup. Projektet är ett grupparbete i HTML, CSS/SCSS och tillgänglighet.

Webbplatsen innehåller fem sidor: Start, Portfolio, Om mig, Tjänster & priser och Kontakt.

## Gruppmedlemmar och ansvar

- Saya – Startsida.
- Flavius – Portfolio.
- Nathalie – Kontakt.
- Gemensamt – Om mig och Tjänster & priser.

## Länkar

- [Besök webbplatsen](https://senshisai.github.io/linnea-ek-fotografi/)
- [GitHub-repository](https://github.com/Senshisai/linnea-ek-fotografi)

## Sass / SCSS

Vi använder Sass med SCSS-syntax. Stylingen är uppdelad i mindre filer, så kallade partials, för att göra koden lättare att hitta och underhålla.

- `_variables.scss` – gemensamma färger och typsnitt.
- `_base.scss` – grundstilar, header, navigering och footer.
- `_home.scss` – startsidan.
- `_portfolio.scss` – Portfolio.
- `_om-mig.scss` – Om mig.
- `_tjanster.scss` – Tjänster & priser.
- `_contact.scss` – Kontakt.

Alla filer ligger i mappen `scss`. Filen `style.scss` samlar dem med `@use` och kompileras till `style.css`. Samtliga HTML-sidor använder den gemensamma CSS-filen.

Vi använder variabler för färger och typsnitt, nesting för att gruppera stilar och mixins för att återanvända kod.

## Kompilera Sass

Vi använder tillägget **Live Sass Compiler** i Visual Studio Code.

1. Öppna projektmappen i VS Code.
2. Installera tillägget Live Sass Compiler om det saknas.
3. Klicka på **Watch Sass** längst ner i VS Code.
4. Gör ändringar i SCSS-filerna och spara.

Tillägget omvandlar SCSS till CSS och uppdaterar `scss/style.css`. Webbläsaren använder CSS-filen för att visa sidornas utseende. Därför ändrar vi i SCSS-filerna och låter tillägget uppdatera CSS-filen.

## Responsivitet och tillgänglighet

Layouten är byggd med Flexbox och Grid. Vi arbetar mobile-first: grundstilarna gäller för mobil och anpassas till större skärmar med `min-width`-media queries.

Vi använder semantisk HTML, alt-texter för bilder och etiketter till formulärfält. Webbplatsen har testats med Lighthouse och HTML-validatorn.

## Samarbete med Git

Vi arbetar i egna branches och sammanför ändringarna till `main` genom pull requests. GitHub används för versionshantering och samarbete.