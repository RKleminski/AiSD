## Zadanie 7: Grafy

* Termin zajęć: 23/05/2019
* Termin oddania: 06/06/2019
* Sposób zaliczenia: prezentacja na zajęciach
* Punkty: 20

## Opis zadania

**1. Graf (5 pkt.)**

1.1 Wymagania

* Zaimplementowanie grafu, tj. struktury danych składającej się z wierzchołków i łączących ich krawędzi
* Graf powinien obsługiwać zarówno wariant skierowany jak i nieskierowany
* Graf powinien obsługiwać zarówno wariant ważony jak i nieważony
* Wierzchołki przechowują zmienną zadeklarowanego typu

1.2 Metody

* dodawanie/usuwanie wierzchołka
* dodawanie/usuwanie krawędzi
* modyfikacja wagi krawędzi
* modyfikacja wierzchołka
* wypisanie grafu jako listy krawędzi
* wypisanie wierchołków grafu
* zwrócenie stopnia wierchołka *(degree)*, także wchodzącego i wychodzącego
* wypisanie sąsiadów wierzchołka

**2. Minimalne drzewo rozpinające (5 pkt.)**

* Zaimplementowanie znajdowania minimalnego drzewa rozpinającego
* Proponowane algorytmem Kruskala lub Prima
* Proszę zwrócić uwagę na ograniczenia algorytmów: działają one dla nieskierowanego grafu spójnego

**3. Najkrótsza ścieżka (5 pkt.)**

* Zaimplementowanie znajdowania najkrótszej ścieżki w grafie
* Proponowane algorytmem Dijkstry lub Bellmana-Forda
* Proszę zwrócić uwagę na ograniczenie algorytmu Dijkstry: nie działa on dla grafu z ujemnymi wagami krawędzi

**4. Cykle (5 pkt.)**

* Zaimplementowanie wykrywania cykli w grafie
* Proponowane algorytmem Kosaraju lub Tarjana
