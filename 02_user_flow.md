# Analiza User Flow – Gra „Wizyta u dziadka”

## Środowisko testowe

- Linux + Firefox

---

## Etap 1 – Wejście do gry

### Scenariusz:
1. Użytkownik klika przycisk „Wejdź”.
2. Rozpoczyna się ekran ładowania.

### Oczekiwany rezultat:
Gra powinna przejść do pierwszej sceny / wprowadzenia po zakończeniu ładowania.

### Rzeczywisty rezultat:
Gra ładuje się bez końca (brak przejścia do kolejnego ekranu).

Problem został odtworzony:
- na systemie Linux (Firefox)
- na urządzeniu mobilnym (iOS + Safari)

### Dodatkowa obserwacja:
Pomimo nieskończonego ładowania, użytkownik może ręcznie przejść do innych sekcji (np. hol, jadalnia, inne pomieszczenia).

---

## Analiza problemu

Możliwe przyczyny:
- błąd w mechanizmie inicjalizacji sceny startowej,
- problem z asynchronicznym ładowaniem zasobów,
- brak timeoutu lub obsługi błędu po stronie aplikacji,
- problem kompatybilności przeglądarki (potwierdzone w teście poniżej)

---

## Wpływ na użytkownika

- dezorientacja,
- brak jasnej informacji, czy gra działa,
- potencjalne porzucenie gry przez ucznia.

Dla użytkownika może to oznaczać:
- frustrację,
- utratę motywacji,
- przekonanie, że „gra nie działa”.

---

## Priorytet: WYSOKI

Błąd blokuje naturalny przepływ wejścia do gry.


---


## TEST - Problem kompatybilności przeglądarki

### Opis
Gra nie przechodzi z ekranu ładowania po kliknięciu „Wejdź” w przeglądarce Firefox (Linux).

### Środowiska testowe

- Linux + Firefox -> błąd (nieskończone ładowanie)
- iOS + Safari -> błąd (nieskończone ładowanie)
- Linux + Google Chrome -> działa poprawnie

### Oczekiwany rezultat
Gra powinna działać poprawnie we wszystkich wspieranych przeglądarkach.

### Rzeczywisty rezultat
W Firefox i Safari gra nie inicjalizuje poprawnie pierwszej sceny.

### Wpływ
- Możliwe porzucenie produktu.
- Ryzyko wykluczenia cyfrowego (np. szkoły korzystające z domyślnego Firefox).

### Priorytet
Wysoki

### Kategoria
Błąd funkcjonalno-techniczny / kompatybilność przeglądarki


---
