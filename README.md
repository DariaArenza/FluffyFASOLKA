# Fasolka – wersja online 1.0.0

Wspinaczkowa gra platformowa o myszce Fasolce. Biomy: **Lawendowa wieża** i **Wiśniowy ogród**.

## Co jest w paczce

| Plik | Do czego służy |
|---|---|
| `index.html` | cała gra |
| `manifest.webmanifest` | pozwala dodać grę do ekranu telefonu jak aplikację |
| `sw.js` | gra działa też bez internetu po pierwszym otwarciu |
| `icons/` | ikona gry (telefon, karta przeglądarki) |
| `render.yaml` | ustawienia dla Render |

## Wrzucenie na GitHub (tak jak OCTOCHAOS)

1. Na GitHubie: **New repository** → nazwa np. `fasolka` → **Create repository**.
2. Kliknij **uploading an existing file** (albo **Add file → Upload files**).
3. Przeciągnij **zawartość** folderu (`index.html`, `manifest.webmanifest`, `sw.js`, `render.yaml`, `README.md` i cały folder `icons`) – nie sam folder `fasolka-online`.
4. **Commit changes**.

## Uruchomienie na Render

1. Render → **New +** → **Static Site**.
2. Wybierz repozytorium `fasolka`.
3. Ustawienia:
   - **Branch:** `main`
   - **Build Command:** zostaw puste
   - **Publish Directory:** `.`
4. **Create Static Site**. Po minucie gra będzie pod adresem typu `https://fasolka.onrender.com`.

Strona statyczna na Render jest darmowa i nie usypia się jak serwer gry – otwiera się od razu.

## Aktualizacja gry

1. Wgraj nowy `index.html` na GitHub (**Add file → Upload files**, nadpisze stary).
2. W pliku `sw.js` zmień numer wersji w linijce `const VERSION = 'fasolka-1.0.0';` (np. na `1.0.1`) i też go wgraj.
3. Render sam opublikuje nową wersję.

## Na telefonie jak aplikacja

- **Android (Chrome):** menu ⋮ → **Dodaj do ekranu głównego**.
- **iPhone (Safari):** przycisk udostępniania → **Do ekranu początkowego**.

Zapis postępu, rekordy i czapeczki są przechowywane w przeglądarce każdego gracza.
