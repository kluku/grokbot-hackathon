# Contract Sentinel — GrokBot Hackathon

Materiały do demo systemu agentów, który pomaga zespołowi biznesowemu przeglądać umowy, odpowiada na pytania o zobowiązania i wykrywa potencjalne sprzeczności z nowymi warunkami usług.

Hackathon: Wrocław, 5 listopada 2026. Sprint: 18:00–21:00.

## Zakres demo

- Karta najważniejszych warunków umowy z cytatami.
- Pytania dla sales: marketing, poufność i ochrona pracowników.
- Porównanie nowych warunków z istniejącymi zobowiązaniami.
- Opcjonalny przegląd terminów z wyraźnie oznaczonym scenariuszem testowym.

Boty: **Sentinel** koordynuje pracę, **Contracts** analizuje klauzule, **Security** ocenia zagadnienia bezpieczeństwa, a **Reviewer** weryfikuje źródła i wnioski.

## Jak zacząć

1. Przeczytaj [opis danych](CZYTAJ_NAJPIERW.txt).
2. Otwórz [instrukcję i plan sprintu](GROKBOT_STARTER/START.txt).
3. Użyj [promptów botów](GROKBOT_STARTER/PROMPTY.txt) oraz [rozszerzenia biznesowego](GROKBOT_STARTER/ROZSZERZENIE_BIZNESOWE.txt).
   Następnie jednorazowo wdróż [stałą procedurę obsługi](GROKBOT_STARTER/HARNESS.txt), aby użytkownik mógł zadawać zwykłe pytania bez instrukcji dla poszczególnych agentów. Zapis pliku w repo nie oznacza aktywacji w GrokBocie.
4. Przeprowadź próby z [przypadkami demonstracyjnymi](GROKBOT_STARTER/SCENARIUSZE_DEMO.json) i [oczekiwaniami testów](GROKBOT_STARTER/OCZEKIWANIA_TESTOW.txt).
5. Po działającej próbie skonfiguruj [rutynę i webhook](GROKBOT_STARTER/AUTOMATYZACJA.txt).

## Zawartość

- `Umowy/`: trzy zanonimizowane historyczne umowy, w formatach TXT i PDF.
- `ISO/`: sześć edukacyjnych opracowań zagadnień bezpieczeństwa, w formatach TXT i PDF.
- `GROKBOT_STARTER/`: prompty, scenariusze, odnośniki do klauzul i instrukcje konfiguracji.
- `MANIFEST.json`: sumy kontrolne dostarczonej paczki danych.

Do analizy wybierz jeden format dokumentów, aby nie wczytywać ich podwójnie.

## Stan i interpretacja wyników

W GrokBocie uruchomiono cztery boty. W obserwowanym czacie 2026-11-05 zakończyły przygotowanie kart i pytań bezpieczeństwa oraz cykl poprawek v2 z recenzją (CS-04–CS-08). To potwierdzenie przebiegu widocznego w aplikacji, nie niezależny audyt wszystkich wyników. Stała procedura obsługi prostych pytań wymaga wdrożenia i testu trwałości. Webhook i harmonogramy pozostają nieprzetestowane.

Umowy są historycznymi kopiami demonstracyjnymi; część tekstu pochodzi z OCR. Materiały `ISO/` nie są tekstem normy ani obowiązującymi politykami firmy. Warunki DemoAI i daty w próbach alertów są fikcyjne. Wyniki analizy nie oznaczają automatycznej akceptacji umowy, zgody na publikację ani potwierdzenia zgodności z ISO.

Repozytorium jest przeznaczone do pracy prywatnej. Anonimizacja nie rozstrzyga możliwości publicznego udostępnienia warunków umownych.
