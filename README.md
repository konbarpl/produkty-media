# produkty-media

Hosting zdjęć produktów do ofert marketplace (Erli i in.).

Struktura: jeden podfolder na model, w środku ponumerowane zdjęcia (`01.jpg`, `02.jpg`, ...).

Wzór raw-URL do PATCH `images` na Erli:

```
https://raw.githubusercontent.com/konbarpl/produkty-media/main/<model>/01.jpg
```

Repo publiczne celowo — Erli pobiera zdjęcia anonimowo, raz, i re-hostuje u siebie.

## Aplikacja „analiza sprzedazy” (Allegro REST API)

Ten adres jest stroną informacyjną aplikacji `analiza sprzedazy`, zarejestrowanej w Allegro Developer Portal i wskazywanej w nagłówku `User-Agent` zapytań do Allegro REST API.

Aplikacja służy wyłącznie właścicielowi konta sprzedawcy Super_Zakupy_PL do pracy na własnych danych tego konta:

- odczyt własnych ofert, zamówień i rozliczeń (billing, prowizje) do raportów sprzedaży,
- zmiany cen własnych ofert po zatwierdzeniu przez właściciela konta.

Nagłówek wysyłany w każdym zapytaniu: `User-Agent: analiza-sprzedazy/1.0 (+https://github.com/konbarpl/produkty-media)` (nazwa zarejestrowana w Allegro Developer Portal: „analiza sprzedazy”).

Aplikacja nie pobiera ofert innych sprzedawców i nie przenosi treści z Allegro na inne platformy. Kontakt: właściciel konta Super_Zakupy_PL przez wiadomości Allegro.
