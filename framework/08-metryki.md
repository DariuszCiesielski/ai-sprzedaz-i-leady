# 08 — Metryki i KPI kampanii lead gen

## Dlaczego metryki?

"Co nie jest mierzone, nie jest zarządzane." Bez metryk nie wiesz:
- Czy kampania działa
- Gdzie są wąskie gardła
- Czy ROI jest pozytywne

## Lejek konwersji

```
Firmy zidentyfikowane (1000)
        ↓ 60% match ICP
Firmy zakwalifikowane (600)
        ↓ 80% email found
Kontakty z emailem (480)
        ↓ 35% open rate
Otwarte emaile (168)
        ↓ 10% reply rate
Odpowiedzi (48)
        ↓ 40% positive
Pozytywne odpowiedzi (19)
        ↓ 60% meeting booked
Spotkania umówione (12)
        ↓ 25% close rate
Zamknięte deale (3)
```

**Z 1000 firm → 3 klientów.** To typowy wynik w B2B cold outreach.

## KPI na każdym etapie

### Etap 1: Pozyskanie danych

| KPI | Cel | Jak mierzyć |
|-----|-----|-------------|
| ICP match rate | >50% | Zakwalifikowane / zidentyfikowane |
| Email found rate | >70% | Emaile znalezione / zakwalifikowane |
| Email validity rate | >95% | Zweryfikowane / znalezione |
| Koszt na kontakt | <$0.50 | Łączny koszt narzędzi / kontakty |

### Etap 2: Outreach

| KPI | Cel | Jak mierzyć |
|-----|-----|-------------|
| **Open rate** | >35% | Otwarte / wysłane |
| **Reply rate** | >8% | Odpowiedzi / wysłane |
| **Positive reply rate** | >4% | Pozytywne / wysłane |
| Bounce rate | <3% | Odbite / wysłane |
| Unsubscribe rate | <1% | Wypisani / wysłane |

### Etap 3: Konwersja

| KPI | Cel | Jak mierzyć |
|-----|-----|-------------|
| **Meeting book rate** | >40% | Spotkania / pozytywne odpowiedzi |
| **SQL rate** | >30% | Sales Qualified Leads / spotkania |
| **Close rate** | >20% | Zamknięte / SQL |
| Avg deal size | Zależy | Średnia wartość kontraktu |
| Sales cycle | <30 dni | Od pierwszego kontaktu do zamknięcia |

## Metryki finansowe

### Koszt pozyskania leada (CPL)

```
CPL = Łączne koszty kampanii / Liczba leadów

Przykład:
- Narzędzia: 500 PLN/mies.
- Czas handlowca: 2000 PLN/mies. (50% czasu)
- AI API: 100 PLN/mies.
- Łącznie: 2600 PLN
- Leadów (pozytywne odpowiedzi): 48
- CPL = 2600 / 48 = ~54 PLN
```

### Koszt pozyskania klienta (CAC)

```
CAC = Łączne koszty sprzedaży i marketingu / Nowi klienci

Przykład:
- Koszty lead gen: 2600 PLN
- Koszty sprzedaży (spotkania, demo): 1500 PLN
- Łącznie: 4100 PLN
- Nowi klienci: 3
- CAC = 4100 / 3 = ~1367 PLN
```

### ROI kampanii

```
ROI = (Przychód z nowych klientów - Koszty) / Koszty × 100%

Przykład:
- 3 klientów × 5000 PLN MRR × 12 mies. = 180,000 PLN LTV
- Koszty: 4100 PLN
- ROI = (180,000 - 4100) / 4100 × 100% = 4290%
```

### LTV:CAC ratio

```
LTV:CAC = Lifetime Value / Customer Acquisition Cost

Cel: >3:1 (zdrowy biznes)
Idealnie: >5:1

Przykład: 60,000 PLN LTV / 1,367 PLN CAC = 43.9:1 (świetnie)
```

## Dashboard tygodniowy

Raportuj co tydzień:

```
=== Raport tygodniowy: Lead Gen ===
Okres: [DATA - DATA]

📊 WOLUMEN
- Nowe firmy zidentyfikowane: 150
- Emaile wysłane: 120
- Follow-upy: 85

📈 OUTREACH
- Open rate: 38% (cel: >35%) ✅
- Reply rate: 11% (cel: >8%) ✅
- Positive replies: 7
- Bounce rate: 2% (cel: <3%) ✅

🎯 KONWERSJA
- Spotkania umówione: 4
- SQL: 2
- Pipeline wartość: 24,000 PLN

💰 KOSZTY
- Narzędzia: 500 PLN
- AI API: 95 PLN
- Łącznie: 595 PLN
- CPL: 85 PLN

📋 WNIOSKI
- Najlepszy temat emaila: "Re: [TEMAT]" (45% open)
- Najgorsza branża: retail (2% reply)
- Najlepsza branża: e-commerce (15% reply)
- Akcja: wykluczyć retail z ICP, skupić na e-commerce
```

## Benchmarki branżowe (B2B Polska)

| Metryka | Słaba | Średnia | Dobra | Świetna |
|---------|-------|---------|-------|---------|
| Open rate | <20% | 20-30% | 30-40% | >40% |
| Reply rate | <3% | 3-6% | 6-12% | >12% |
| Meeting book rate | <20% | 20-35% | 35-50% | >50% |
| Close rate | <10% | 10-20% | 20-30% | >30% |
| CPL | >200 PLN | 100-200 PLN | 50-100 PLN | <50 PLN |
| CAC | >5000 PLN | 2000-5000 PLN | 1000-2000 PLN | <1000 PLN |

## Optymalizacja na podstawie metryk

### Open rate niski (<20%)?
→ Problem: **temat emaila**
→ Testuj: inne tematy, personalizacja w temacie, krótsze tematy

### Open rate OK, reply rate niski (<3%)?
→ Problem: **treść emaila**
→ Testuj: inny hook, krótszy email, silniejsze CTA

### Reply rate OK, ale mało spotkań?
→ Problem: **kwalifikacja lub CTA**
→ Testuj: lepsze ICP, prostszy booking (Calendly link), niższy commitment

### Dużo spotkań, mało zamknięć?
→ Problem: **kwalifikacja lub oferta**
→ Testuj: lepszy scoring (za niski próg), doskonalenie prezentacji

## Co dalej?

To ostatni rozdział frameworka. Wykorzystaj szablony:
- [Szablon ICP](../templates/icp-template.md)
- [Szablony emaili](../templates/outreach-email-templates.md)
- [Matryca scoringu](../templates/scoring-matrix.md)
- [Checklista RODO](../checklists/rodo-checklist.md)
- [Checklista kampanii](../checklists/kampania-checklist.md)
