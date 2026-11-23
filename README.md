# Boty w akcji

**Onboarding pojazdu i kierowcy u partnera flotowego aplikacji przewozowych i taxi** - od umowy leasingu do pierwszego kursu kierowcy.

[![Film - onboarding pojazdu i kierowcy](obrazy/film.jpg)](https://onboarding.trynity.eu/)

▶ **Film (ok. 4,5 min):** https://onboarding.trynity.eu/ - pod filmem lista wszystkich kroków; kliknięcie kroku przenosi do tego miejsca w filmie.

## O projekcie

Partner flotowy udostępnia samochody i kierowców aplikacjom przewozowym i firmom taxi. Każdy nowy samochód i każdy nowy kierowca to dziesiątki czynności: faktury, dokumenty, terminy, protokoły, urządzenia, zgłoszenia w urzędach i aplikacjach. Ten projekt zamienia je w jeden proces prowadzony przez boty:

- pracownik rozmawia z botami w komunikatorze - bot podpowiada kolejny krok i pilnuje braków,
- dokumenty czyta sztuczna inteligencja, a pracownik tylko zatwierdza odczyt,
- kierowca podpisuje dokumenty i protokoły na tablecie, bez drukowania,
- wszystko trafia do jednej bazy z pełną historią zmian - kto, co i kiedy,
- terminy (OC, badania, przeglądy, uprawnienia) pilnuje bot i przypomina z wyprzedzeniem.

## Proces - 4 etapy

| Etap | Co się dzieje |
|---|---|
| **A. Samochód wchodzi do floty** | dane samochodu z faktury w KSeF, zgłoszenie VAT-26, ewidencja przebiegu z GPS, plan przeglądów zgodny z warunkami gwarancji producenta, roczny limit km, protokół odbioru na tablecie |
| **B. Przystosowanie do taxi** | GPS, taksometr, instalacja LPG, wpis TAXI w dowodzie, polisa OC, licencja i oklejenie, kategorie pojazdu i listy pojazdów w aplikacjach przewozowych |
| **C. Kierowca** | rejestracja z odczytem dokumentów, weryfikacja (dokumenty, tożsamość, kod SMS i e-mail, uprawnienia), kaucja, wniosek o identyfikator, kasa fiskalna i terminal |
| **D. Wydanie i opieka w czasie pracy** | protokół wydania na tablecie (wyposażenie, poprzednie i nowe uszkodzenia, uwagi głosowe), przeglądy umawiane automatycznie, ochrona przed przekroczeniem przebiegu, kontrola uprawnień, kontakt z kierowcą przez SMS i e-mail, mandaty - wskazanie kierującego |

| | | |
|---|---|---|
| ![Krok 1 - faktura z KSeF](obrazy/krok_01_faktura_ksef.jpg) | ![Krok 6 - protokół odbioru na tablecie](obrazy/krok_06_protokol_odbioru.jpg) | ![Krok 21 - wydanie samochodu](obrazy/krok_21_wydanie_samochodu.jpg) |
| Faktura z KSeF → dane samochodu w bazie | Protokół odbioru na tablecie | Wydanie samochodu kierowcy |

## Technologia

Python · boty Telegram · SQLite z historią zmian · odczyt dokumentów przez AI (Claude) · strona podpisów na tablecie (HTTPS) · raporty w Telegram Mini App · serwer VPS w Polsce. Kod powstaje we współpracy z Claude Code.

## Zasady

- **RODO:** dane osobowe są tylko w systemie, nigdy w repozytorium; w filmie i w tym opisie - dane przykładowe.
- **Historia:** każda zmiana danych jest zapisana - kto, co i kiedy.
- **Prawo i podatki:** wątpliwości są zbierane i konsultowane z prawnikiem i doradcą podatkowym, zanim trafią do procesu.

To repozytorium zawiera opis projektu. Kod źródłowy jest prywatny.

## Autor

**Trynity Sp. z o.o.** - wdrożenia enova365 i integracje AI · [trynity.eu](https://trynity.eu)
Mariusz Gajda

---
Muzyka w filmie: „Keep the Funk ON” - mixkit.co (licencja Mixkit) · „Funkorama” - Kevin MacLeod (incompetech.com), licencja Creative Commons: Uznanie autorstwa 4.0 (creativecommons.org/licenses/by/4.0).
