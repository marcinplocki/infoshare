# Plan Zarządzania Zmianą (PZZ) — Grupa Merito

Uproszczone narzędzie do przygotowania Planu Zarządzania Zmianą, zastępujące
rozbudowaną formatkę Excel. Działa jako pojedynczy plik HTML — bez instalacji,
bez serwera, wystarczy otworzyć `plan-zarzadzania-zmiana.html` w przeglądarce.

## Zawartość narzędzia

- **Dane projektu** — metryczka projektu/programu, główne korzyści biznesowe
  i etapy/kamienie milowe zaciągnięte z karty projektu (.docx) automatycznie
  po wczytaniu pliku.
- **Ankieta — skala zmiany** — 3-częściowa ankieta (max 65 pkt), klasyfikuje
  zmianę do poziomu 1 (mała), 2 (średnia) lub 3 (duża).
- **Checklisty (poziom 1–2)** — zaślepka dla uproszczonej ścieżki; docelową
  treść przygotowuje Martyna.
- **Diagnoza** — pełny PCT jako zestaw pytań z automatycznym wyliczaniem
  wyniku (poziom 3, z wizualizacją na klasycznym trójkącie Prosci) oraz
  ocena ADKAR dla 5 stałych ról wobec zmiany (w tym „Klienci — zewnętrzni
  odbiorcy zmiany”), z automatycznym „szybkim skanem”. Dostępna dla
  poziomu 2 i 3 (dla poziomu 2 bez sekcji PCT).
- **Plan działań** — zagregowany na poziomie roli wobec zmiany, z
  przykładowymi działaniami podpowiadanymi automatycznie po
  zidentyfikowaniu bariery ADKAR.
- **Pulpit** — podsumowanie zarządcze: statusy działań, limit WIP, sygnały do
  decyzji.
- **Przewodnik** — jak pracować z PZZ.

Zapis wersji działa lokalnie w przeglądarce (localStorage). Jedyny format
pliku do zapisu/odczytu poza przeglądarką to Excel (przycisk „Zapisz plik”,
w pełni stylowany paletą marki Grupa Merito, wczytywany z powrotem
przyciskiem „Otwórz plik”).

## Stan prac / otwarte tematy

Zgodnie z notatką ze spotkania zespołu (Joanna, Marcin, Martyna, Izabela):

- [ ] Checklisty dla poziomu 1 i 2 — docelowa treść (Martyna).
- [ ] Uzgodnienie z HR jednego określenia „menedżerowie liniowi” (Joanna).
- [ ] Weryfikacja merytoryczna finalnej wersji narzędzia (Izabela).

## Uwaga techniczna

Plik ładuje React, Babel Standalone i SheetJS z CDN (unpkg) — wymaga
połączenia z internetem przy pierwszym uruchomieniu. Jeśli narzędzie ma
działać w pełni offline, kolejnym krokiem może być spakowanie bibliotek
lokalnie (bundling) zamiast odwołań do CDN.
