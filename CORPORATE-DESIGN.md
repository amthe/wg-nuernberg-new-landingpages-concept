# WG Nürnberg — Corporate Design Referenz

## Logo

Graues Sprechblasen-Logo mit weißem "wg" Schriftzug.
Datei: `data/wg-nuernberg/logo.svg` (auch als `logo.png`)
Immer verlinkt zu: https://www.wg-nuernberg.de
Daneben Text: "WG Nürnberg"

Das Logo wird als **inline SVG** eingebettet (kein externer Link):
```svg
<svg xmlns="http://www.w3.org/2000/svg" width="40" height="40" viewBox="0 0 180 180"><path fill="#535353" d="M108 34c-3-3-7-5-10-5H34c-3 0-7 2-10 5s-5 7-5 11v44l1 8c1 6 5 10 9 12s8 1 12 1c0 6 0 12-2 18 4-7 9-13 14-18h45c7 0 13-5 14-12l1-7V46c0-5-2-9-5-12z"/><path fill="#535353" d="M99 45c2-2 5-3 7-3h44c3 0 6 1 7 3 2 2 4 5 4 8v30l-1 7c0 3-3 6-6 8h-8c-1 5 0 9 1 13l-10-13h-31c-4 0-9-3-10-8v-5-32c0-3 1-6 3-8z"/><path fill="#FFF" d="M32 81l3-7 3-8 3-8 2-9 1-1v-2l1-2h4l1 1 1 1v6l-3 7-3 8-3 7-2 7-1 1v5l-1 2v2l1 2 1 1h1l3-1 5-5 5-6 5-7 5-9 3-8 1-1h2l2 1 1 2v1l-1 2-1 3-1 3-1 4v12l1 3v2l1 2 2 1 2-1 3-3 3-4 2-5 3-6 2-5 2-6 1-5 1-4v-4l1-3 1-4 1-2 1-1 1-1 1-1 2 1 1 3v4l-1 5-1 4-1 5-3 9-4 10-5 8-4 7-2 2-3 2-3 1-2 1q-3 0-5-2l-3-4-2-6v-7l-4 6-4 5-3 3-4 3-4 3-4 1-4-1-2-2-2-3v-4-6l1-5zM140 71l-1 1h-2l-3 1-3 1-2 1-1 1h-1-1l-1 1-1-1h-1l-1-2v-1l1-2 2-1 2-1h3l1-1h2l3-1 3-1 2-1 2 1 2 1 1 1v4l-3 7-5 6-6 5-7 3h-1l-2 1h-7-1v-1l-4-2-3-3-1-3-1-4 1-5 2-6 3-5 4-5 5-5 5-3 3-2 3-2 4-1 3-1h3l2 2 2 1v5l-1 1h1-1-2l-2-1-1-1-1-1h-1l-5 2-6 4-6 5-4 5-4 6-1 6 1 4 3 3 2 1 3 1 2-1 3-1 3-1 2-2q4-2 6-5l4-7v-1z"/></svg>
```

---

## Farben

| Rolle | Farbe | Hex |
|---|---|---|
| **Primary** (Buttons, Links, Akzente, Sektionen) | Lila/Blau-Violett | `#5755d9` |
| Primary Hover | etwas dunkler | `#4b48d6` |
| Primary Active | nochmal dunkler | `#3634d2` |
| **Secondary Background** | helles Flieder | `#f1f1fc` |
| **Success** (NUR WhatsApp-Button!) | Grün | `#32b643` |
| **Warning** | Gelb | `#ffb700` |
| **Error / Accent** | Orange | `#e85600` |
| **Text** | Dunkelgrau | `#3b4351` |
| **Muted Text** | Mittelgrau | `#66758c` |
| **Dark Sections** (Footer, dunkle Sektionen) | Dunkel | `#303742` |
| **Borders** | Hellgrau | `#dadee4` |
| **Light Background** | Fast-Weiß | `#f7f8f9` |
| **Hintergrund** | Weiß | `#fff` |

### ⚠️ Wichtig: Grün sparsam!
Grün (#32b643) darf **NUR** für den WhatsApp-CTA-Button verwendet werden. Alle anderen Akzente, Buttons, Überschriften, Borders, Banner → Primary Lila (#5755d9).

---

## Typografie

**Keine Google Fonts!** System-Font-Stack:
```
-apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", sans-serif
```

---

## Layout-Stil

- **Hintergrund:** Weiß mit subtiler SVG-Geometrie (hellgrauer Streifen-Pattern)
- **Container:** max-width 1200px, zentriert
- **Grid:** Flexbox/Columns (col-4, col-6 etc.)
- **Cards:** Weiße Karten mit 1px Border (#dadee4), leichter Schatten
- **Buttons:** `.btn` mit Primary-Farbe, `.btn-success` nur für WhatsApp
- **Genereller Stil:** Schlicht, clean, keine fancy Animationen, kein Parallax
- **Responsive:** Mobile-first, Breakpoint bei 768px
- **Standalone:** Alles inline im `<style>` Tag, kein CDN

---

## Kontaktdaten (immer gleich)

- **Firma:** WG Nürnberg
- **Adresse:** Vordere Sterngasse 2a, 90402 Nürnberg
- **Telefon:** 0911-2355810
- **E-Mail:** info@wg-nuernberg.de
- **Website:** https://www.wg-nuernberg.de
- **WhatsApp:** https://wa.me/499112355810

---

## Seitenstruktur (Standard)

1. **Header:** Logo (links) + CTA-Button (rechts)
2. **Hero:** Tag, Überschrift, Untertitel, Buttons, Hero-Card mit Stats
3. **Adressleiste:** Lila Hintergrund mit Adresse + Kontakt
4. **Inhaltssektionen:** Abwechselnd weiß / grau / dunkel / farbig
5. **CTA-Sektion:** Farbiger Hintergrund (Lila), zentriert
6. **Kontakt:** Formular + Kontaktinfos + WhatsApp-Button
7. **Footer:** Dunkel (#303742), Firmeninfo + Links
