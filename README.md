# produkty-media

Hosting zdjęć produktów do ofert marketplace (Erli i in.).

Struktura: jeden podfolder na model, w środku ponumerowane zdjęcia (`01.jpg`, `02.jpg`, ...).

Wzór raw-URL do PATCH `images` na Erli:

```
https://raw.githubusercontent.com/konbarpl/produkty-media/main/<model>/01.jpg
```

Repo publiczne celowo — Erli pobiera zdjęcia anonimowo, raz, i re-hostuje u siebie.
