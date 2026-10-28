# Our Little Universe — dla Myszki

Autorska, statyczna strona na pierwszy miesiąc związku. HTML + CSS + vanilla JavaScript; bez backendu, kont, bibliotek płatnych ani kluczy API.

## Pliki

- `index.html` — struktura strony i wszystkie sekcje
- `styles.css` — styl, responsywność i animacje
- `app.js` — licznik, koperty, karty, list, marzenia, wiadomości, ukryta niespodzianka, quiz i finał
- `config.js` — teksty, data i personalizacja

## Uruchomienie lokalne

Najprościej otworzyć `index.html` w przeglądarce. Do testów bardziej podobnych do hostingu można uruchomić serwer statyczny:

```bash
python -m http.server 8080
```

Następnie wejdź na `http://localhost:8080`.

## Personalizacja

Otwórz `config.js`. Najważniejsze ustawienia:

```js
nickname: "Myszko",
relationshipStart: "2026-10-01",
signature: "z całego serca, ja",
```

W tym samym pliku zmienisz treść listu, sekretnych kopert, 10 kart, marzeń, wiadomości „Otwórz, gdy…”, pytań quizu i finału.

Ważne: teksty są przykładowe. Przed wysłaniem linku przeczytaj je i popraw tak, aby brzmiały jak Ty i pasowały do Waszej relacji.

## Darmowy hosting

### GitHub Pages
1. Utwórz nowe repozytorium na GitHubie.
2. Wgraj wszystkie cztery pliki do głównego katalogu repozytorium.
3. Otwórz **Settings → Pages**.
4. Wybierz publikację z gałęzi `main`, folder `/ (root)`, a następnie zapisz.
5. Po zakończeniu wdrożenia GitHub pokaże publiczny adres strony.

### Cloudflare Pages
Możesz też utworzyć projekt Pages z repozytorium GitHub. To strona statyczna, więc nie potrzebuje komendy build ani backendu.

## Prywatność

Strona nie wysyła wiadomości ani zaznaczonych marzeń na serwer. Zaznaczenia marzeń są przechowywane lokalnie w przeglądarce osoby, która otworzy stronę. Publiczny link może jednak otworzyć każda osoba, która go otrzyma; nie traktuj go jako zabezpieczenia hasłem. Nie umieszczaj w nim danych, których nie chcesz publicznie udostępniać.

## Uwaga o liczniku

Licznik używa daty `2026-10-01` i lokalnego czasu urządzenia. Liczy od lokalnej północy tego dnia. Daty miesięcznych rocznic mogą przypadać na różne długości miesięcy; pasek postępu pokazuje postęp względem pierwszego miesiąca.
