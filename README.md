# Blisko

Niezależny prototyp ogólnopolskiej wyszukiwarki placówek opieki dla seniorów.

Obejmuje wyszukiwanie, filtry usług i ceny, sortowanie, dostępność, zapisane
placówki, responsywną listę oraz schematyczną mapę Polski. Dane są demonstracyjne.
Model danych jest przygotowany do rozszerzenia o kolejne kraje.

Profil placówki (`detail.html`) zawiera galerię, pełny opis, usługi, warianty
pokoi i cen, interaktywny kalendarz dostępności oraz formularz kontaktowy.

## Uruchomienie

Nie wymaga instalowania zależności. Otwórz `index.html` w przeglądarce albo uruchom lokalny serwer HTTP, np.:

```powershell
cd outputs/Blisko
python -m http.server 8080
```

Następnie przejdź na `http://localhost:8080`.

## Struktura

- `index.html` — widok aplikacji
- `styles.css` — pełna warstwa wizualna i responsywność
- `app.js` — interakcje

Projekt nie zawiera zależności ani odwołań do Flexo.

## Model biznesowy

Darmowy wpis podstawowy oraz abonamenty Partner i Pro dla placówek. Portal nie
pobiera prowizji od przyjęcia seniora; płatna promocja jest zawsze oznaczona i
nie wpływa na weryfikację ani organiczne dopasowanie.

Strefa B2B jest oddzielona od wyszukiwarki dla rodzin: `partners.html` zawiera
ofertę, plany i rejestrację, a `dashboard.html` przedstawia panel placówki.
