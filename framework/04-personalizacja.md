# 04 — Personalizacja outreachu z AI

## Dlaczego personalizacja?

| Typ emaila | Open rate | Reply rate |
|------------|-----------|------------|
| Generyczny cold email | 15-25% | 1-3% |
| Personalizowany (imię + firma) | 25-35% | 3-5% |
| **Deep personalizacja (AI)** | **35-50%** | **8-15%** |

Różnica między 2% a 12% reply rate to różnica między porażką a sukcesem kampanii.

## Czym jest "deep personalizacja"?

To nie tylko `{imię}` i `{firma}` w szablonie. To:
- Referencja do konkretnego postu/artykułu osoby
- Komentarz o aktualnej sytuacji firmy
- Propozycja rozwiązania konkretnego problemu
- Ton dopasowany do branży i stanowiska

## Pipeline personalizacji AI

```
1. Zbierz dane o firmie i osobie
   ↓
2. AI analizuje kontekst (strona, LinkedIn, posty)
   ↓
3. AI identyfikuje "hook" (punkt zaczepienia)
   ↓
4. AI generuje spersonalizowaną wiadomość
   ↓
5. Człowiek weryfikuje i wysyła
```

### Krok 1: Zbieranie danych

AI automatycznie zbiera z publicznych źródeł:

**O firmie:**
- Branża, rozmiar, lokalizacja
- Główne produkty/usługi
- Ostatnie wiadomości (press releases, blog)
- Technologie (BuiltWith, Wappalyzer)
- Rekrutacje (sygnał wzrostu)

**O osobie:**
- Stanowisko, ścieżka kariery
- Ostatnie posty na LinkedIn
- Artykuły, wystąpienia
- Wspólne kontakty

### Krok 2: Identyfikacja hooka

"Hook" to powód, dla którego piszesz TERAZ do TEJ osoby. AI wybiera najlepszy:

| Typ hooka | Przykład | Siła |
|-----------|---------|------|
| **Trigger event** | "Gratulacje z okazji nowej rundy finansowania" | Bardzo wysoka |
| **Wspólny kontakt** | "Poznaliśmy się na konferencji X" | Wysoka |
| **Content hook** | "Przeczytałem Pana artykuł o..." | Wysoka |
| **Problem hook** | "Widzę, że szukacie marketing managera — mogę pomóc" | Średnia-wysoka |
| **Branża hook** | "Pracuję z firmami z branży X i zauważyłem trend..." | Średnia |
| **Komplement** | "Imponujący wzrost Waszej firmy w ostatnim roku" | Średnia |

### Krok 3: Generowanie wiadomości

Prompt dla AI:

```
Na podstawie poniższych danych napisz spersonalizowany cold email:

DANE FIRMY:
{firma_dane}

DANE OSOBY:
{osoba_dane}

HOOK:
{wybrany_hook}

NASZA OFERTA:
{opis_oferty}

ZASADY:
- Max 100 słów
- Ton: profesjonalny, ale ludzki
- Jeden konkretny CTA (spotkanie 15 min)
- Język polski, forma Pan/Pani
- Bez agresywnej sprzedaży
- Bez generycznych frazesów ("Mam nadzieję, że ta wiadomość zastaje Pana w dobrym zdrowiu")
```

### Krok 4: Weryfikacja człowiekiem

AI generuje draft — człowiek sprawdza:
- [ ] Czy fakty są poprawne? (AI może halucynować)
- [ ] Czy ton jest odpowiedni?
- [ ] Czy CTA jest jasny?
- [ ] Czy nie jest zbyt agresywny?

## Personalizacja na LinkedIn

### Connection request (max 300 znaków)

```
Dzień dobry [IMIĘ], przeczytałem Pana post o [TEMAT] — bardzo trafne spostrzeżenia.
Pracuję z firmami z branży [BRANŻA] nad [PROBLEM]. Chętnie się połączę.
```

### Pierwszy message po akceptacji

```
Dziękuję za połączenie! Nie chcę zabierać czasu — w skrócie:
pomagam firmom takim jak [FIRMA] z [KONKRETNY PROBLEM].
Niedawno pomogliśmy [PODOBNA FIRMA] osiągnąć [WYNIK].
Czy warto porozmawiać 15 minut? Jeśli nie — bez problemu, miłego dnia.
```

## Personalizacja emaila — przykłady

### Dobry email (deep personalizacja)

```
Temat: Re: Pana post o automatyzacji — pomysł

Dzień dobry Panie Marku,

Przeczytałem Pana post na LinkedIn o wyzwaniach z automatyzacją procesów
w e-commerce. Trafne spostrzeżenie o kosztach ręcznej obsługi zwrotów.

Pracuję z firmami e-commerce (m.in. [PRZYKŁAD]) nad automatyzacją właśnie
tego procesu. Typowo zmniejszamy czas obsługi zwrotu z 15 do 2 minut.

Czy warto porozmawiać 15 minut w tym tygodniu? Chętnie pokażę, 
jak to wygląda w praktyce.

Pozdrawiam,
[IMIĘ]
```

### Zły email (generyczny)

```
Temat: Oferta współpracy

Szanowny Panie,

Mam nadzieję, że ta wiadomość zastaje Pana w dobrym zdrowiu.
Jestem przedstawicielem firmy XYZ, lidera w branży automatyzacji.
Oferujemy innowacyjne rozwiązania dla firm takich jak Pana.
Nasze rozwiązanie pozwala zaoszczędzić czas i pieniądze.
Czy moglibyśmy umówić się na spotkanie?

Z poważaniem,
[IMIĘ]
```

## Personalizacja w skali

### Problem skali
- Deep personalizacja: 10 min / email
- Potrzebujesz: 50-100 emaili / tydzień
- = 8-16h tygodniowo na same emaile

### Rozwiązanie: AI batch processing
1. Lista 50 firm → AI enrichment (5 min)
2. AI generuje 50 drafts (10 min)
3. Człowiek weryfikuje i edytuje (2h)
4. Wynik: 50 spersonalizowanych emaili w ~2.5h (zamiast 8h)

## Anty-wzorce (czego unikać)

- ❌ "Chciałbym przedstawić naszą firmę..." — nikogo to nie obchodzi
- ❌ "Jako lider branży..." — każdy tak pisze
- ❌ Email >200 słów — nikt nie czyta long cold emails
- ❌ Wiele CTA ("spotkanie, demo, lub przeczytaj nasz blog") — jedno CTA
- ❌ Załączniki — trafiają do spamu
- ❌ Fałszywe "Re:" w temacie — nieetyczne, obniża zaufanie

## Co dalej?

→ [05 — Follow-up](05-follow-up.md)
