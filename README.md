# Odtwarzacz muzyki pod tagi NFC

Jedna strona, wiele tagów. Każdy tag NFC zapisujesz jako rekord **URL** z linkiem:

```
https://dtronics-pl.github.io/<repo>/?t=<klucz>
```

## Dodanie utworu
1. Wrzuć MP3 do `muzyka/` (najlepiej 128–192 kbps, nazwa bez spacji i polskich znaków).
2. W `index.html` dopisz wpis w `TRACKS`:
   ```js
   drugi: { title: "Tytuł", artist: "Wykonawca", src: "muzyka/drugi.mp3", cover: "", hue: 200 }
   ```
3. Tag: `…/?t=drugi`

Zmiana utworu pod istniejącym kluczem nie wymaga przepisywania tagu.

## Włączenie GitHub Pages
Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)` → Save.
Po ok. minucie strona działa pod `https://dtronics-pl.github.io/<repo>/`.

## Uwagi
- iPhone nie pozwala na autoodtwarzanie z dźwiękiem — potrzebne jedno dotknięcie ▶. Android czasem gra od razu.
- Repo jest publiczne: wrzucaj tylko muzykę własną lub z licencją pozwalającą na udostępnianie.
