# 02 — Źródła leadów

## Przegląd źródeł

| Źródło | Typ danych | Koszt | Jakość | Wolumen |
|--------|-----------|-------|--------|---------|
| **Google Maps** | Firmy lokalne | Niski | Wysoka | Średni |
| **Strony firmowe** | Dane kontaktowe | Niski | Wysoka | Niski |
| **LinkedIn** | Osoby decyzyjne | Średni-wysoki | Bardzo wysoka | Wysoki |
| **Bazy firm (KRS/CEIDG)** | Dane rejestrowe | Niski | Średnia | Bardzo wysoki |
| **Eventy/konferencje** | Uczestnicy | Średni | Bardzo wysoka | Niski |
| **Social media** | Sygnały intencji | Niski | Zmienna | Wysoki |
| **Narzędzia dedykowane** | Enriched data | Wysoki | Wysoka | Wysoki |

## 1. Google Maps

### Co możesz pozyskać
- Nazwa firmy, adres, telefon, strona www
- Godziny otwarcia, kategoria
- Oceny i recenzje (sygnał jakości)
- Zdjęcia (sygnał aktywności)

### Jak wykorzystać z AI
1. Zdefiniuj zapytanie (np. "gabinety stomatologiczne Kraków")
2. Pobierz dane (Google Maps API lub narzędzia jak DataForSEO)
3. AI filtruje: czy firma pasuje do ICP?
4. AI znajduje email ze strony www
5. AI personalizuje wiadomość na podstawie recenzji/opisu

### Wskazówki
- Szukaj firm z **niskimi ocenami** (potrzebują pomocy)
- Szukaj firm **bez strony www** (potencjał na usługi digital)
- Filtruj po liczbie recenzji (więcej = większa firma)

### RODO
- Dane firmowe z Google Maps są **publiczne** — można używać w B2B
- Dane kontaktowe **osób** (nie firm) wymagają podstawy prawnej
- Zawsze umożliw rezygnację z kontaktu

## 2. Strony firmowe

### Web scraping z AI
1. Znajdź listę firm (z Google Maps, branżowych katalogów, konferencji)
2. AI czyta stronę firmową i wyciąga:
   - Opis działalności
   - Technologie (co widać w kodzie strony)
   - Zespół / osoby decyzyjne
   - Dane kontaktowe (email, telefon, formularz)
3. AI ocenia dopasowanie do ICP

### Sygnały ze strony www
| Sygnał | Co oznacza | Wartość dla scoringu |
|--------|-----------|---------------------|
| Strona przestarzała | Potrzebuje modernizacji | Wysoka (usługi web) |
| Brak SSL | Niska świadomość tech | Średnia |
| Blog aktywny | Inwestuje w marketing | Wysoka |
| Zakładka "Kariera" | Firma rośnie | Wysoka |
| Nowe produkty/usługi | Okres inwestycji | Bardzo wysoka |

## 3. LinkedIn

### Strategie pozyskiwania
- **Sales Navigator** — zaawansowane filtry, listy leadów
- **Obserwowanie firm** — zmiany w zespole, posty, aktywność
- **Grupy branżowe** — uczestnictwo, identyfikacja aktywnych osób
- **Posty i komentarze** — sygnały intencji (ktoś pyta o rozwiązanie = lead)

### AI w LinkedIn prospectingu
- Analiza profilu → dopasowanie do ICP
- Generowanie spersonalizowanego connection request
- Monitorowanie postów ICP → automatyczny alert "ten lead jest gorący"
- Analiza sieci kontaktów → warm intro opportunities

### Limity i zasady
- LinkedIn ma limity: ~100 connection requests/tydzień
- Nie spamuj InMail — 1 wiadomość, max 1 follow-up
- Personalizuj connection request (referencja do postu/firmy)

## 4. Bazy publiczne (KRS/CEIDG)

### KRS (Krajowy Rejestr Sądowy)
- Dane rejestrowe spółek
- Zarząd, kapitał, przedmiot działalności
- Dostęp: [ems.ms.gov.pl](https://ems.ms.gov.pl)

### CEIDG (Centralna Ewidencja Działalności Gospodarczej)
- Jednoosobowe działalności gospodarcze
- Dane: nazwa, PKD, adres, data rozpoczęcia
- Dostęp: [ceidg.gov.pl](https://ceidg.gov.pl)

### Jak wykorzystać
1. Filtruj po kodach PKD (branża)
2. Filtruj po dacie rejestracji (nowe firmy = potrzebują usług)
3. Filtruj po lokalizacji
4. Enrichment: znajdź stronę www, email, telefon

## 5. Eventy i konferencje

### Przed eventem
- Lista prelegentów → research → przygotuj spersonalizowane intro
- Lista sponsorów → potencjalni partnerzy
- Lista uczestników (jeśli publiczna)

### W trakcie
- Skanowanie wizytówek → CRM
- Notatki z rozmów → AI podsumowanie + scoring

### Po evencie
- Follow-up w ciągu 48h
- "Miło było Pana poznać na [EVENT]. Rozmawialiśmy o [TEMAT]..."
- AI generuje spersonalizowany email na podstawie notatek

## 6. Social media (monitoring intencji)

### Sygnały intencji
Ktoś publicznie szuka rozwiązania = gorący lead:

- **Facebook grupy**: "Szukam firmy, która zrobi mi stronę www"
- **Twitter/X**: "Czy ktoś poleci narzędzie do CRM?"
- **Reddit**: "Potrzebuję pomocy z automatyzacją marketingu"

### AI monitoring
1. Zdefiniuj frazy kluczowe (problem, którego szukają Twoi klienci)
2. AI monitoruje social media
3. Alert: nowy post pasujący do ICP
4. AI przygotuje wersję roboczą odpowiedzi

## 7. Pipeline łączony

Najskuteczniejszy pipeline łączy kilka źródeł:

```
Google Maps (lista firm)
        ↓
Web scraping (enrichment)
        ↓
Hunter.io (email)
        ↓
LinkedIn (osoba decyzyjna)
        ↓
AI scoring (dopasowanie do ICP)
        ↓
AI personalizacja (email + LI)
        ↓
Outreach sekwencja
```

## Co dalej?

→ [03 — Scoring AI](03-scoring-ai.md)
