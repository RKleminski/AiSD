## Zadanie 4: Binarne drzewo poszukiwań

* Termin zajęć: 11.04.2019
* Termin oddania: 25.04.2019
* Sposób zaliczenia: prezentacja na zajęciach
* Punkty: 10

## Opis zadania

**1. BST (10 pkt.)**

  1.1 Ogólne
  * Zaimplementowanie poprawnej struktury drzewa, tj. wielopoziomowej struktury danych w której każdy element posiada dwa elementy potomne, lewy oraz prawy
  * Każdy element posiada wewnętrzne ID w drzewie oraz przechowywaną wartość (klucz)
  * Potomek lewy elementu zawsze ma klucz mniejszy or rodzica, prawy - większy
  * Wystarczy zaimplementowanie struktury dla prostego typu numerycznego klucza (np. int); generyczne drzewo będzie dodatkowo punktowane
  
  1.2 Metody
  * Add
  * Remove - *usuwa element po kluczu*
  * Size
  * Root - *zwraca korzeń drzewa*
  * Subtree - *zwraca pod-drzewo z korzeniem w podanym elemencie*
  * Min
  * Max
  * Find - *wyszukuje element o zadanym kluczu i zwraca jego ID*
  * Show - *wypisuje drzewo zgodnie z wybranym algorytmem przejścia, tj. pre-order, post-order lub in-order*
  * Draw - ***(nieobowiązkowe, +2pkt.)** wizualizuje drzewo w formie graficznej*
  
**2. AVL (nieobowiązkowe, +5pkt.)**

  * Zaawansowana wersja drzewa BST: zapewnia zbalansowanie drzewa, tj. reorganizuje drzewo za kadym razem tak, aby lewe i prawe poddrzewo różniły się głębokością o *co najwyżej* jeden poziom
  * Rebalansowanie następuje w ramach operacji *Add* i *Remove*
  * Rebalansowanie odbywa się za pomocą operacji rotacji
  * Materiał spoza wykładu, proponuję posiłkować się [zewnętrznymi źródłami](https://www.tutorialspoint.com/data_structures_algorithms/avl_tree_algorithm.htm)
