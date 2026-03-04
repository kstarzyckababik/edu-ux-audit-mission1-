## Analiza dostępności – wsparcie audio

### Obserwacja

Pierwsza scena gry zawiera automatyczne wprowadzenie głosowe.
Kolejne sceny i polecenia tekstowe nie są czytane na głos.

Nie stwierdzono możliwości ręcznego uruchomienia audio dla dalszych instrukcji.

### Analiza

Jeżeli gra jest kierowana do uczniów klas 1-3:
- część użytkowników może mieć trudność z samodzielnym czytaniem poleceń,
- brak audio może obniżać dostępność poznawczą.

Dodatkowo:
- obecność audio w pierwszej scenie tworzy oczekiwanie spójności w kolejnych etapach.

### Potencjalne ryzyko

- obniżona dostępność dla młodszych uczniów,
- niespójność doświadczenia użytkownika,
- konieczność wsparcia nauczyciela przy korzystaniu z gry.

### Rekomendacja

- Dodanie opcji odsłuchu poleceń w każdej scenie
lub
- Jasne określenie minimalnej grupy wiekowej

### Priorytet

Średni

---

## Jakość renderowania tekstu

### Obserwacja
Tekst w grze sprawia wrażenie nieostrego / lekko rozmytego (scena salon -> popiersie -> uzuepełnienie munduru)
Problem występuje niezależnie od przeglądarki.

### Analiza
Możliwa przyczyna:
- skalowanie elementów (CSS transform / zoom),
- renderowanie w canvas o innej rozdzielczości niż ekran,
- brak optymalizacji pod wysokie DPI.

### Wpływ na użytkownika
- obniżona czytelność,
- zwiększone obciążenie wzroku,
- potencjalna bariera dla uczniów młodszych klas.

### Rekomendacja
- weryfikacja renderowania fontów w natywnej rozdzielczości,
- sprawdzenie skalowania interfejsu przy różnych DPI.

### Priorytet
Średni
