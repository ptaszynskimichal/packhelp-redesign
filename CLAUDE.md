# Packhelp Redesign — instrukcje projektu

Przed zbudowaniem lub edycją jakiejkolwiek strony/sekcji w tym repo przeczytaj
[`PAGE_BUILDING_GUIDELINE.md`](PAGE_BUILDING_GUIDELINE.md). Mapuje on intencję
("chcę sekcję X", "potrzebuję kroku konfiguratora do wyboru Y") na konkretny
komponent, wariant przycisku, wzorzec karty i odstęp między sekcjami — na
podstawie analizy `index.html`, `build-your-box.html` i `packaging.html`.

Trzymaj się kanonicznych rekomendacji z tego pliku (m.in. sekcja 8 — znane
niespójności prototypu i ich zalecane rozwiązanie, np. rozmiar H2 czy domyślna
widoczność `.section-badge`) zamiast bezrefleksyjnie kopiować niespójności ze
starych sekcji do nowych.

To static HTML/CSS/JS prototype — bez build toolingu. `tokens.css`, `base.css`,
`components.css` to warstwa design tokenów/atomów wspólna dla wszystkich stron;
layout specyficzny dla sekcji zostaje inline w `<style>` danej strony, dopóki nie
powtórzy się na więcej niż jednej stronie (wtedy dopiero awansuje do
`components.css`).
