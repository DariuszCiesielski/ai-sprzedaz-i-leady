# Checklista RODO — Generowanie leadów

## Przed rozpoczęciem kampanii

### Podstawa prawna
- [ ] Określona podstawa prawna przetwarzania (art. 6.1.f — uzasadniony interes dla B2B)
- [ ] Przeprowadzony test równowagi interesów (Twój interes vs. prywatność osoby)
- [ ] Udokumentowane uzasadnienie ("dlaczego kontaktuję te osoby")

### Źródła danych
- [ ] Dane pozyskane z legalnych źródeł (strony firmowe, LinkedIn, KRS/CEIDG)
- [ ] NIE kupujesz baz danych osób fizycznych
- [ ] Udokumentowane źródło każdego kontaktu (skąd masz ten email)
- [ ] Dane firmowe (nie prywatne) — email na domenę firmy, nie gmail/wp.pl

### Infrastruktura
- [ ] Osobna domena do cold emaili (nie główna domena firmy)
- [ ] SPF, DKIM, DMARC skonfigurowane
- [ ] Bezpieczne przechowywanie danych (szyfrowanie, ograniczony dostęp)
- [ ] Blacklista (osoby, które prosiły o brak kontaktu) — AKTYWNA

## W treści każdego emaila

### Obowiązkowe elementy
- [ ] Twoje dane: imię, firma, stanowisko
- [ ] Źródło danych: "Pana/Pani dane pozyskałem z [ŹRÓDŁO]"
- [ ] Cel: "Kontaktuję się w sprawie [CEL]"
- [ ] Podstawa prawna: "Art. 6 ust. 1 lit. f RODO"
- [ ] Opt-out: "Odpowiedz STOP, a usunę dane"
- [ ] Administrator: nazwa i adres Twojej firmy

### Przykład stopki RODO

```
---
Pana/Pani służbowy adres email pozyskałem ze strony internetowej
firmy [NAZWA]. Przetwarzam go na podstawie uzasadnionego interesu
administratora (art. 6 ust. 1 lit. f RODO) w celu nawiązania
współpracy biznesowej. Administratorem danych jest [TWOJA FIRMA],
[ADRES]. Przysługuje Panu/Pani prawo dostępu do danych, ich
sprostowania, usunięcia oraz sprzeciwu wobec przetwarzania.
Aby zrezygnować z kontaktu, wystarczy odpowiedzieć "STOP".
```

## Zarządzanie sprzeciwami

### Gdy ktoś powie "stop" / "wypisz" / "nie kontaktuj"
- [ ] Usunięcie z aktywnej listy — natychmiast (max 72h)
- [ ] Dodanie do globalnej blacklisty
- [ ] Potwierdzenie emailem: "Usunąłem Pana/Pani dane"
- [ ] Usunięcie z CRM (lub oznaczenie "do not contact")
- [ ] NIE wysyłasz odpowiedzi z ofertą ("ale może warto...")

### Gdy ktoś żąda usunięcia danych (art. 17)
- [ ] Usunięcie ze WSZYSTKICH systemów (CRM, Excel, listy, backup)
- [ ] Potwierdzenie usunięcia na piśmie — w ciągu 30 dni
- [ ] Dokumentacja (kto zażądał, kiedy, co usunięto)
- [ ] Zachowanie wpisu na blackliście (żeby nie kontaktować ponownie)

## Limity i etyka

### Częstotliwość kontaktu
- [ ] Max 1 email + 3 follow-upy (łącznie 4 wiadomości)
- [ ] Przerwa minimum 3 dni między wiadomościami
- [ ] Po braku odpowiedzi na 4. wiadomość — STOP (nie kontaktujesz ponownie)
- [ ] Breakup email na koniec (jasna informacja, że to ostatni kontakt)

### Treść
- [ ] Brak fałszywych tematów ("Re:", "Fwd:" bez kontekstu)
- [ ] Brak manipulacji ("Twoja firma jest zagrożona...")
- [ ] Brak obietnic bez pokrycia
- [ ] Jasna identyfikacja nadawcy (nie anonimy)

## Retencja danych

### Okresy przechowywania
- [ ] Leady bez odpowiedzi: max 6 miesięcy → usunięcie
- [ ] Leady z odmową: natychmiastowe usunięcie (blacklista zostaje)
- [ ] Leady w pipeline: do zakończenia procesu + 6 mies.
- [ ] Klienci: przez czas trwania umowy + okres prawny

### Automatyzacja retencji
- [ ] Cron job / reminder: co miesiąc sprawdź stare kontakty
- [ ] Automatyczne usunięcie po 6 mies. bez aktywności
- [ ] Raport retencji: ile danych przechowujesz i dlaczego

## Dokumentacja

### Rejestr czynności przetwarzania
- [ ] Prowadzony i aktualny (art. 30 RODO)
- [ ] Zawiera: cel, podstawę, kategorie danych, źródła, okres, zabezpieczenia

### Polityka prywatności
- [ ] Na stronie www — aktualna
- [ ] Obejmuje przetwarzanie w celach marketingowych
- [ ] Link w stopce emaila (opcjonalnie, ale zalecane)

### Umowy powierzenia (art. 28)
- [ ] Podpisane z dostawcami narzędzi (CRM, email tool, scraping tool)
- [ ] Sprawdzone: czy dostawca przechowuje dane w UE?

## Audyt kwartalny

Co 3 miesiące sprawdź:
- [ ] Czy blacklista jest aktualna?
- [ ] Czy retencja danych jest przestrzegana?
- [ ] Czy stopka RODO w emailach jest aktualna?
- [ ] Czy nowi pracownicy znają zasady?
- [ ] Czy nie było naruszeń (sprawdź logi)?

## Naruszenie danych — plan awaryjny

Jeśli dojdzie do wycieku danych:
1. [ ] Powiadom UODO w ciągu **72 godzin**
2. [ ] Powiadom osoby, których dane dotyczą (jeśli wysokie ryzyko)
3. [ ] Udokumentuj: co się stało, kiedy, jakie dane, jakie działania
4. [ ] Wdróż środki zapobiegawcze

> ⚠️ Ta checklista nie zastępuje porady prawnej. Skonsultuj się z prawnikiem specjalizującym się w RODO.
