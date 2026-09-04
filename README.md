# Nikolina Đurović — geštalt psihoterapija

Statični jednostrani sajt. Struktura:

```
index.html      — cela stranica
styles.css      — stilovi (Classical dizajn sistem)
images/         — hero.png, gestalt.webp, portret.webp
.nojekyll       — obavezno! bez njega GitHub menja izgled sajta
```

**Važno:** sva četiri stavke moraju biti u repozitorijumu, uključujući skriveni fajl `.nojekyll`.
Ako `styles.css` nije uploadovan ili je `.nojekyll` izostavljen, sajt će na GitHubu izgledati
drugačije — bez boja, sa drugim fontovima i rasporedom.

## Hostovanje na GitHub Pages

1. Napravi repozitorijum na GitHubu (npr. `nikolina-djurovic`).
2. Ubaci sav sadržaj ovog foldera u koren repozitorijuma (`index.html`, `styles.css`, `images/`).
3. Settings → Pages → Source: `Deploy from a branch`, Branch: `main`, folder: `/ (root)`.
4. Sajt će biti na `https://<korisnicko-ime>.github.io/<repo>/`.

Za sopstveni domen: Settings → Pages → Custom domain, pa kod registrara dodaj CNAME zapis ka `<korisnicko-ime>.github.io`.

## Zamena slika

Zameni fajlove u `images/` istim imenima i sve radi bez menjanja koda:
- `hero.png` — horizontalno, ~2400 × 1000 px, motiv desno
- `gestalt.webp` — vertikalno 4:5, min. 1200 × 1500 px
- `portret.webp` — vertikalno 4:5, min. 1200 × 1500 px

## Kontakt forma

Trenutno samo prikazuje potvrdu — ne šalje mejl. Za pravo slanje najlakše je Formspree:
napravi formu na formspree.io i u `index.html` dodaj `action="https://formspree.io/f/TVOJ-ID" method="POST"`
na `<form id="kontakt-forma">`, pa obriši `<script>` blok na dnu.

## Pre objave proveri

- Broj krizne linije u futeru.
- Podatke o obrazovanju, superviziji, adresi, mejlu i telefonu.
- Utisci klijenata su primeri — objavljuj samo uz pismenu saglasnost.

## Mobilna verzija

Sajt je responzivan u istom `index.html` — nema odvojene mobilne strane. Na širinama do 768px: burger meni, hero sa svetlijim slojem preko slike, sve kolone u jedan red, tabela cena kao kartice, forma puna širina.
