# Plan Zarządzania Zmianą (PZZ) — Grupa Merito

Uproszczone narzędzie do przygotowania Planu Zarządzania Zmianą, zastępujące
rozbudowaną formatkę Excel. Działa jako pojedynczy plik HTML — bez instalacji,
bez serwera, wystarczy otworzyć `plan-zarzadzania-zmiana.html` w przeglądarce.

## Zawartość narzędzia

- **Dane projektu** — metryka projektu/programu.
- **Ankieta — skala zmiany** — 3-częściowa ankieta (max 65 pkt), klasyfikuje
  zmianę do poziomu 1 (mała), 2 (średnia) lub 3 (duża).
- **Checklisty (poziom 1–2)** — zaślepka dla uproszczonej ścieżki; docelową
  treść przygotowuje Martyna.
- **Diagnoza** — ocena gotowości całego przedsięwzięcia (pełny PCT jako
  zestaw pytań dla poziomu 3, skrócona „Szybka ocena gotowości” dla
  poziomu 2, obie z wizualizacją na wykresie radarowym) oraz ocena ADKAR
  dla 4 stałych kategorii interesariuszy (+ opcjonalna 5.
  „Klienci/studenci”), z automatycznym „szybkim skanem”. Dostępna dla
  poziomu 2 i 3.
- **Plan działań** — zagregowany na poziomie kategorii, limit **3 działania
  na kategorię**, z przykładowymi działaniami podpowiadanymi automatycznie
  po zidentyfikowaniu bariery ADKAR.
- **Pulpit** — podsumowanie zarządcze: statusy działań, limit WIP, sygnały do
  decyzji.
- **Przewodnik** — jak pracować z PZZ.

Zapis wersji działa lokalnie w przeglądarce (localStorage). Jedyny format
pliku do zapisu/odczytu poza przeglądarką to Excel (eksport przyciskiem
„Eksport Excel”, w pełni stylowany paletą marki Grupa Merito, wczytywany
z powrotem przyciskiem „Wczytaj Excel”).

## Stan prac / otwarte tematy

Zgodnie z notatką ze spotkania zespołu (Joanna, Marcin, Martyna, Izabela):

- [ ] Checklisty dla poziomu 1 i 2 — docelowa treść (Martyna).
- [ ] Test czterech kategorii interesariuszy na żywym projekcie, w tym czy
      klienci/studenci potrzebują osobnej kategorii (Joanna, Marcin, Martyna).
- [ ] Uzgodnienie z HR jednego określenia „menedżerowie liniowi” (Joanna).
- [ ] Weryfikacja merytoryczna finalnej wersji narzędzia (Izabela).

## Uwaga techniczna

Plik ładuje React, Babel Standalone i SheetJS z CDN (unpkg) — wymaga
połączenia z internetem przy pierwszym uruchomieniu. Jeśli narzędzie ma
działać w pełni offline, kolejnym krokiem może być spakowanie bibliotek
lokalnie (bundling) zamiast odwołań do CDN.
