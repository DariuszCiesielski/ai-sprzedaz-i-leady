# 03 — AI Lead Scoring

## Czym jest lead scoring?

Punktacja leadów (lead scoring) to system oceny potencjalnych klientów. Zamiast traktować wszystkich jednakowo, priorytetyzujesz tych, którzy najprawdopodobniej kupią.

## Tradycyjny vs AI scoring

| Aspekt | Tradycyjny | AI Scoring |
|--------|-----------|------------|
| **Kryteria** | Ręcznie zdefiniowane reguły | Automatycznie wykryte wzorce |
| **Dane** | Firmografia (branża, rozmiar) | Firmografia + behawioralne + kontekst |
| **Aktualizacja** | Manualna (raz na kwartał) | Ciągła (real-time) |
| **Precyzja** | ~40-60% | ~70-85% |
| **Bias** | Wysoki (intuicja handlowca) | Niższy (dane) |

## Model scoringowy: 3 wymiary

### Wymiar 1: Dopasowanie do ICP (0-40 pkt)

Jak bardzo firma pasuje do Twojego idealnego klienta.

| Kryterium | Pkt | Przykład |
|-----------|-----|---------|
| Branża (dokładne dopasowanie) | 10 | E-commerce → 10 pkt |
| Branża (pokrewna) | 5 | Retail → 5 pkt |
| Wielkość firmy (idealny zakres) | 10 | 10-50 pracowników → 10 pkt |
| Lokalizacja (target region) | 5 | Polska → 5 pkt |
| Technologie (kompatybilne) | 10 | Używa Shopify → 10 pkt |
| Budżet (szacowany) | 5 | Widoczne inwestycje w marketing → 5 pkt |

### Wymiar 2: Sygnały intencji (0-35 pkt)

Czy firma aktywnie szuka rozwiązania?

| Sygnał | Pkt | Jak wykryć |
|--------|-----|-----------|
| Odwiedził stronę | 5 | Analytics |
| Pobrał lead magnet | 10 | Formularz |
| Pytanie na social media | 15 | Monitoring AI |
| Szukał na Google (intent keyword) | 10 | Google Ads data |
| Wypełnił formularz kontaktowy | 20 | CRM |
| Zmiana w firmie (nowy CEO, funding) | 10 | Monitoring LinkedIn |
| Rekrutuje na stanowisko pokrewne | 10 | Job boards |

### Wymiar 3: Gotowość do zakupu (0-25 pkt)

Czy decydent jest dostępny i gotowy?

| Sygnał | Pkt |
|--------|-----|
| Zidentyfikowany decydent | 10 |
| Decydent aktywny na LinkedIn | 5 |
| Firma w fazie wzrostu | 5 |
| Brak długoterminowego kontraktu z konkurencją | 5 |
| Budżetowanie (Q1 lub Q4) | 5 |

### Łączna punktacja

| Score | Kategoria | Akcja |
|-------|-----------|-------|
| **80-100** | 🔥 Gorący | Natychmiast kontaktuj — handlowiec dzwoni w 24h |
| **60-79** | 🟡 Ciepły | Outreach spersonalizowany email + follow-up |
| **40-59** | 🔵 Letni | Dodaj do nurturingu (content, newsletter) |
| **20-39** | ⚪ Zimny | Monitoruj — scoring może się zmienić |
| **0-19** | ❌ Niekwalifikowany | Nie kontaktuj — nie pasuje do ICP |

## AI w scoringu — jak to działa

### Krok 1: Zbierz dane o firmie
```
Input: "Nazwa firmy: XYZ Sp. z o.o., Strona: xyz.pl"
AI: Czyta stronę, LinkedIn, KRS → JSON z danymi firmowymi
```

### Krok 2: Porównaj z ICP
```
AI: Porównuje dane firmy z profilem ICP
→ Score firmograficzny: 35/40
→ Uzasadnienie: "Branża e-commerce, 25 pracowników, Kraków — idealny fit"
```

### Krok 3: Sprawdź sygnały intencji
```
AI: Sprawdza aktywność firmy w ostatnich 30 dniach
→ Score intencji: 20/35
→ Uzasadnienie: "Nowe ogłoszenie o pracę na marketing managera + post CEO o skalowaniu"
```

### Krok 4: Wynik końcowy
```
Łączny score: 55+20+15 = 90/100 → 🔥 GORĄCY
Priorytet: 1
Zalecana akcja: Natychmiastowy kontakt handlowca
Sugerowany hook: "Widzę, że szukacie marketing managera — mogę pomóc skalować marketing szybciej"
```

## Dyskwalifikatory (automatyczny score 0)

Niezależnie od punktacji, niektóre firmy są automatycznie wykluczone:

- Firma w upadłości / likwidacji
- Bezpośredni konkurent
- Firma z "czarnej listy" (złe doświadczenia)
- Brak jakiejkolwiek obecności online (ghost company)
- Firma jednoosobowa, gdy ICP wymaga >10 pracowników

## Kalibracja modelu

### Co 2 tygodnie:
1. Sprawdź wyniki: ile gorących leadów faktycznie kupiło?
2. Jeśli <20% — scoring jest zbyt łatwy (podnieś progi)
3. Jeśli >80% — scoring jest zbyt restrykcyjny (obniż progi)

### Co kwartał:
1. Przeanalizuj zamknięte deale — jakie cechy mieli klienci?
2. Zaktualizuj wagi w matrycy scoringowej
3. Dodaj nowe sygnały intencji, które się potwierdziły

## Narzędzia do scoringu

| Narzędzie | Scoring | Cena | Uwagi |
|-----------|---------|------|-------|
| **HubSpot** | Wbudowany | Od $0 (limited) | Dobry na start |
| **Apollo.io** | AI scoring | Od $49/mies. | Najlepszy stosunek cena/jakość |
| **Clearbit** | Enrichment + score | Enterprise | Premium dane |
| **Własny (LLM)** | Custom | Koszt API LLM | Pełna kontrola |

→ Szczegóły: [Matryca scoringu](../templates/scoring-matrix.md)

## Co dalej?

→ [04 — Personalizacja](04-personalizacja.md)
