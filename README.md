# AP Estates — apestates.pl

Strona firmowa AP Estates — pośrednictwo nieruchomości w Tajlandii (PL/EN).

## Stack
Jeden statyczny plik `index.html` (HTML/CSS/JS, bez zależności poza Google Fonts). Hosting: GitHub Pages + domena apestates.pl.

## Deploy
1. Push do brancha `main` — GitHub Pages publikuje automatycznie (Settings → Pages → Deploy from branch `main` / root).
2. Plik `CNAME` ustawia domenę apestates.pl.
3. W Settings → Pages włącz **Enforce HTTPS** (po propagacji DNS).

## Formularz
Załóż konto na formspree.io, utwórz formularz i podmień `YOUR_FORM_ID` w `index.html`.

## Security
- CSP (meta): skrypty tylko inline z tej strony, formularze tylko do formspree.io, brak iframe'ów i obiektów
- Referrer-Policy: strict-origin-when-cross-origin
- Honeypot antyspamowy w formularzu (`_gotcha`)
- Brak sekretów w repo, brak zależności JS z zewnątrz
