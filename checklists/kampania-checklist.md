# Checklista uruchomienia kampanii lead gen

## Faza 1: Przygotowanie (tydzień 1)

### Strategia
- [ ] ICP zdefiniowany i zatwierdzony → [Szablon ICP](../templates/icp-template.md)
- [ ] Wybrany model: inbound / outbound / hybrid
- [ ] Budżet kampanii ustalony (narzędzia + czas)
- [ ] KPI zdefiniowane (open rate, reply rate, spotkania, deale)
- [ ] Okres kampanii ustalony (min. 4 tygodnie na ocenę)

### Narzędzia
- [ ] Email finder aktywny (Hunter.io / Snov.io / Apollo)
- [ ] Narzędzie do sekwencji skonfigurowane (Lemlist / Woodpecker / Instantly)
- [ ] CRM gotowy do przyjmowania leadów
- [ ] LinkedIn Sales Navigator (jeśli multichannel)
- [ ] AI API key (GPT-4o-mini / Claude) do personalizacji

### Infrastruktura email
- [ ] Domena do cold emaili kupiona (osobna od głównej)
- [ ] Skrzynki email utworzone (2-3 na kampanię)
- [ ] SPF, DKIM, DMARC skonfigurowane
- [ ] Warmup uruchomiony (min. 2 tygodnie przed kampanią)
- [ ] Podpis emailowy gotowy (imię, firma, telefon)

### RODO
- [ ] Checklista RODO przejrzana → [RODO Checklist](rodo-checklist.md)
- [ ] Stopka RODO w szablonach emaili
- [ ] Blacklista aktywna
- [ ] Rejestr czynności przetwarzania zaktualizowany

## Faza 2: Budowanie listy (tydzień 1-2)

### Źródła danych
- [ ] Źródła leadów wybrane → [Źródła leadów](../framework/02-zrodla-leadow.md)
- [ ] Lista firm (min. 200-500 firm na start)
- [ ] Dane zweryfikowane (nazwy, branże, rozmiary)
- [ ] Emaile znalezione (email finder)
- [ ] Emaile zweryfikowane (bounce check <3%)

### Enrichment
- [ ] Dane firmowe uzupełnione (strona, opis, technologie)
- [ ] Osoby decyzyjne zidentyfikowane
- [ ] LinkedIn profile znalezione
- [ ] AI scoring przeprowadzony → [Scoring](../framework/03-scoring-ai.md)

### Segmentacja
- [ ] Lista podzielona na segmenty (branża / rozmiar / score)
- [ ] Każdy segment ma dedykowany messaging
- [ ] Gorące leady (>80 pkt) — osobna ścieżka (priorytet)

## Faza 3: Przygotowanie contentu (tydzień 2)

### Emaile
- [ ] Szablon #1 wybrany i spersonalizowany → [Szablony emaili](../templates/outreach-email-templates.md)
- [ ] Follow-up #1 napisany (case study)
- [ ] Follow-up #2 napisany (inny kąt)
- [ ] Follow-up #3 napisany (breakup)
- [ ] AI personalizacja przetestowana (10 drafts → weryfikacja jakości)

### Landing page (jeśli inbound)
- [ ] Landing page gotowa (oferta, CTA, formularz)
- [ ] Thank you page z kolejnymi krokami
- [ ] Tracking (Google Analytics, UTM parameters)
- [ ] Lead magnet gotowy (jeśli używasz)

### LinkedIn (jeśli multichannel)
- [ ] Connection request template gotowy
- [ ] Pierwszy message template gotowy
- [ ] Profil LinkedIn zoptymalizowany (headline, about, banner)

## Faza 4: Uruchomienie (tydzień 3)

### Dzień uruchomienia
- [ ] Sekwencja emailowa załadowana do narzędzia
- [ ] Limity wysyłki ustawione (max 50/dzień na nową domenę)
- [ ] Timing ustawiony (wt-czw, 9:00-11:00 rano)
- [ ] Testowy email wysłany do siebie (sprawdź formatowanie, linki)
- [ ] Kampania uruchomiona!

### Pierwszy tydzień — monitoring codzienny
- [ ] Bounce rate <3%? (jeśli >3% → zatrzymaj, sprawdź listę)
- [ ] Spam complaints? (jeśli >0.1% → zatrzymaj, zmień treść)
- [ ] Odpowiedzi przychodzą? (sprawdź inbox 2x dziennie)
- [ ] Pozytywne odpowiedzi → natychmiast do CRM
- [ ] Negatywne odpowiedzi / "STOP" → natychmiast blacklista

## Faza 5: Optymalizacja (tydzień 3-4+)

### Co tydzień
- [ ] Raport tygodniowy → [Metryki](../framework/08-metryki.md)
- [ ] Open rate analiza (czy temat działa?)
- [ ] Reply rate analiza (czy treść działa?)
- [ ] A/B test: nowy wariant tematu lub treści
- [ ] Nowe leady dodane do listy (ciągły pipeline)

### Co 2 tygodnie
- [ ] Kalibracja scoringu (zamknięte deale vs. score)
- [ ] Aktualizacja ICP na podstawie danych
- [ ] Review follow-upów (które działają, które nie)
- [ ] Usunięcie nieaktywnych kontaktów (retencja RODO)

### Po miesiącu
- [ ] Pełna analiza ROI (koszty vs. pipeline vs. zamknięte deale)
- [ ] Decyzja: skalować / pivotować / zatrzymać
- [ ] Dokumentacja wniosków (co zadziałało, co nie)
- [ ] Aktualizacja szablonów i procesów

## Narzędzia kontrolne

### Metryki do śledzenia codziennie
| Metryka | Cel | Alert gdy |
|---------|-----|-----------|
| Emails sent | Wg planu | 0 (narzędzie nie wysyła) |
| Bounce rate | <3% | >5% |
| Open rate | >35% | <20% |
| Reply rate | >8% | <3% |
| Spam complaints | <0.1% | >0.5% |

### Red flags — natychmiast zatrzymaj kampanię
- 🔴 Bounce rate >10% (zła lista emaili)
- 🔴 Spam complaints >1% (treść problematyczna)
- 🔴 Domena na blackliście (sprawdź MXToolbox)
- 🔴 Odpowiedzi prawne / groźba UODO
