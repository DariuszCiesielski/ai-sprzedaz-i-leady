# 06 — Zgodność RODO w generowaniu leadów

## Dlaczego RODO jest kluczowe?

Kary za naruszenie RODO:
- Do **20 mln EUR** lub **4% rocznego obrotu** (wyższa kwota)
- W Polsce: UODO (Urząd Ochrony Danych Osobowych) aktywnie kontroluje
- Reputacja: firma "spamerska" traci zaufanie

## Podstawy prawne przetwarzania danych

### W kontekście B2B lead gen

| Podstawa prawna | Kiedy stosować | Przykład |
|-----------------|---------------|---------|
| **Uzasadniony interes (art. 6.1.f)** | B2B outreach na publiczne emaile firmowe | Email na info@firma.pl |
| **Zgoda (art. 6.1.a)** | Formularze, newsletter, B2C | Formularz na landing page |
| **Wykonanie umowy (art. 6.1.b)** | Kontakt z istniejącym klientem | Follow-up po ofercie |

### Uzasadniony interes — kiedy możesz go użyć?

**TAK:**
- Email na adres firmowy (info@, kontakt@, biuro@) → B2B outreach
- LinkedIn message do osoby na stanowisku decyzyjnym
- Telefon na numer firmowy opublikowany na stronie

**NIE:**
- Email na prywatny adres osoby (gmail, wp.pl) bez zgody
- SMS marketing bez zgody
- Masowy mailing na zakupioną bazę osób fizycznych
- Profilowanie osób fizycznych bez informacji

### Test równowagi interesów

Przed skorzystaniem z "uzasadnionego interesu" odpowiedz na 3 pytania:

1. **Czy masz uzasadniony interes?** (np. marketing B2B — tak)
2. **Czy przetwarzanie jest niezbędne?** (czy nie ma mniej inwazyjnego sposobu?)
3. **Czy interes osoby nie przeważa?** (czy kontakt nie narusza prywatności?)

## Obowiązki informacyjne

### Przy pierwszym kontakcie MUSISZ poinformować o:

1. **Kim jesteś** (administrator danych)
2. **Skąd masz dane** (strona firmy, Google Maps, LinkedIn)
3. **Cel przetwarzania** (kontakt handlowy)
4. **Podstawa prawna** (uzasadniony interes)
5. **Prawo do sprzeciwu** (jak się wypisać)

### Przykład klauzuli w emailu

```
---
Pana/Pani dane kontaktowe (adres email firmowy) pozyskałem ze strony 
internetowej firmy [NAZWA]. Przetwarzam je na podstawie uzasadnionego 
interesu (art. 6 ust. 1 lit. f RODO) w celu przedstawienia oferty 
współpracy. Ma Pan/Pani prawo do sprzeciwu — wystarczy odpowiedzieć 
"STOP" na ten email, a natychmiast usunę Pana/Pani dane.
Administratorem danych jest [TWOJA FIRMA], [ADRES].
```

> ⚠️ W cold emailu klauzula może być w stopce (nie musi być na początku).

## Prawo do sprzeciwu i usunięcia

### Gdy ktoś powie "wypisz mnie" / "stop" / "nie kontaktuj":

1. **Natychmiast** (max 72h) usuń z listy mailingowej
2. Dodaj do **blacklisty** (żeby nie kontaktować ponownie)
3. Potwierdź: "Usunąłem Pana/Pani dane. Przepraszam za kontakt."
4. Nie odpowiadaj na sprzeciw ofertą ("ale może warto...")

### Prawo do usunięcia danych (art. 17)

Na żądanie musisz:
- Usunąć dane ze wszystkich systemów (CRM, Excel, listy)
- Potwierdzić usunięcie w ciągu 30 dni
- Udokumentować, że dane zostały usunięte

## Scraping a RODO

### Co wolno scrapować?

| Dane | Wolno? | Uwagi |
|------|--------|-------|
| Nazwa firmy | ✅ | Dane firmowe, nie osobowe |
| Adres firmy | ✅ | Publiczny |
| Telefon firmowy | ✅ | Opublikowany na stronie |
| Email firmowy (info@) | ✅ | Publiczny |
| **Email imienny (jan@firma.pl)** | ⚠️ | Dane osobowe — uzasadniony interes |
| **Numer prywatny** | ❌ | Bez zgody — nie wolno |
| **Email prywatny** | ❌ | Bez zgody — nie wolno |
| Dane z LinkedIn | ⚠️ | Zgodnie z ToS LinkedIn (ograniczenia) |

### Zabezpieczenia przy scrapingu

1. Scrapuj **tylko dane firmowe publiczne**
2. Nie masuj danych osobowych bez podstawy prawnej
3. Przechowuj dane bezpiecznie (szyfrowanie)
4. Ustalony okres retencji (np. 6 miesięcy bez kontaktu → usunięcie)

## Rejestr czynności przetwarzania

Każda firma >250 pracowników MUSI prowadzić rejestr. Ale przy cold outreachu warto go mieć niezależnie od rozmiaru:

```
Czynność: Lead generation B2B
Cel: Kontakt handlowy z potencjalnymi klientami
Podstawa: Art. 6 ust. 1 lit. f (uzasadniony interes)
Kategorie danych: Imię, nazwisko, email firmowy, stanowisko, firma
Źródło: Strony firmowe, Google Maps, LinkedIn
Okres przechowywania: 6 miesięcy od ostatniego kontaktu
Środki bezpieczeństwa: Szyfrowanie, ograniczony dostęp, backup
```

## Ustawa o świadczeniu usług drogą elektroniczną

Oprócz RODO, w Polsce obowiązuje dodatkowa regulacja:

- **Art. 10** — zakaz przesyłania niezamówionej informacji handlowej drogą elektroniczną
- W praktyce B2B: email na adres firmowy z ofertą współpracy → dozwolone (uzasadniony interes)
- B2C: email marketingowy do osoby fizycznej → wymaga zgody

## Podsumowanie: Co robić, czego nie robić

### ✅ Rób:
- Kontaktuj firmy na publiczne emaile firmowe
- Informuj o źródle danych w każdym emailu
- Umożliwiaj łatwy opt-out (odpowiedź "STOP")
- Prowadź blacklistę (nie kontaktuj ponownie)
- Przechowuj dane bezpiecznie
- Usuwaj dane po okresie retencji

### ❌ Nie rób:
- Nie kupuj baz emaili osób fizycznych
- Nie wysyłaj >3 emaili bez odpowiedzi
- Nie ignoruj sprzeciwu
- Nie przechowuj danych dłużej niż potrzeba
- Nie udostępniaj danych osobowych bez podstawy prawnej
- Nie profiluj osób bez informacji o tym

→ Pełna checklista: [RODO Checklist](../checklists/rodo-checklist.md)

## Co dalej?

→ [07 — Narzędzia](07-narzedzia.md)
