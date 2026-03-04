# Audyt funkcjonalno-techniczny gry edukacyjnej  
„Wizyta u dziadka - zwiedzamy dworek Marszałka Józefa Piłsudskiego”

[GRA](https://niepodlegla.men.gov.pl/niepodlegla/mission1/)

## 1. Cel opracowania

Celem niniejszego opracowania było przeprowadzenie analizy funkcjonalnej, technicznej oraz heurystycznej gry edukacyjnej przeznaczonej dla uczniów klas I-III szkoły podstawowej.

Analiza została wykonana jako symulacja odbioru produktu edukacyjnego przed jego publikacją lub wdrożeniem na platformie publicznej.

---

## 2. Zakres analizy

Analiza obejmowała:

- weryfikację poprawności działania gry w środowisku przeglądarkowym,
- ocenę zgodności funkcjonalnej mechaniki gry z jej celem edukacyjnym,
- analizę user flow i kryteriów ukończenia poszczególnych scen,
- ocenę dostępności cyfrowej (m.in. kontrast, czytelność tekstu, wsparcie audio),
- identyfikację potencjalnych ryzyk technicznych i dydaktycznych,
- sformułowanie rekomendacji usprawnień.

---

## 3. Środowisko testowe

Testy przeprowadzono w następującej konfiguracji:

- system operacyjny: Linux, iOS
- przeglądarki: Mozilla Firefox, Google Chrome, Safari
- wersja gry: przeglądarkowa (desktop)

---

## 4. Ustalenia z analizy

### 4.1. Kompatybilność przeglądarkowa

W przeglądarce Mozilla Firefox i Safari zaobserwowano problem polegający na nieskończonym ładowaniu gry po wybraniu opcji „Wejdź”.  
Problem nie występuje w przeglądarce Google Chrome.

Zdarzenie może wskazywać na brak pełnej optymalizacji pod kątem kompatybilności przeglądarkowej.

---

### 4.2. Kryteria ukończenia sceny

Zaobserwowano możliwość ukończenia sceny i uzyskania wyniku 100% bez interakcji ze wszystkimi dostępnymi elementami edukacyjnymi (np. przeglądaniem albumu).

Może to prowadzić do:

- pominięcia części treści merytorycznych,
- niespójności między zakresem materiału a systemem zaliczenia.

---

### 4.3. Czytelność i jakość renderowania tekstu

W wybranych scenach tekst sprawia wrażenie nieostrego, co może wpływać na komfort czytania.

W kontekście użytkowników młodszych klas czytelność tekstu stanowi istotny element dostępności i jakości dydaktycznej.

---

### 4.4. Dostępność

Pozytywnie oceniono:

- możliwość zmiany kontrastu,
- odpowiednią wielkość tekstu,
- brak presji czasowej,
- intuicyjną nawigację.

Wątpliwości budzi brak pełnego wsparcia audio w części scen, co może mieć znaczenie w przypadku uczniów z niższymi kompetencjami czytelniczymi.

---

## 5. Rekomendacje

1. Zweryfikować działanie gry w przeglądarce Mozilla Firefox.  
2. Doprecyzować kryteria ukończenia sceny lub wyraźnie oznaczyć elementy opcjonalne.  
3. Zweryfikować jakość renderowania tekstu w różnych konfiguracjach rozdzielczości.  
4. Rozważyć rozszerzenie wsparcia audio dla wszystkich poleceń i treści kluczowych.  

---

## 6. Charakter opracowania

Opracowanie ma charakter analityczny i demonstracyjny.  
Celem projektu było zaprezentowanie sposobu prowadzenia analizy funkcjonalno-technicznej produktu edukacyjnego w kontekście odbioru jakościowego.
