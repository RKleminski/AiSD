## Zadanie 2: Stos i Kolejka

* Termin zajęć: 14.03.2019
* Termin oddania: 21.03.2019
* SPosób zaliczenia: prezentacja na zajęciach
* Punkty: 10

## Opis zadania

**1. Stos (5 pkt.)**

* Zaimplementowanie własnego stosu na bazie referencji
* Stos powinien przechowywać elementy dowolnego typu
* Implementacja na bazie referencji oznacza zdefiniowanie odpowiednich klas:
  * *Stack*, czyli klasa z którą będziemy daną strukturę identyfikować i wywoływać z jej poziomu metody. Zawiera zmienną *Top*, która identyfikuje element na szczycie stosu, oraz inne, pomocniczne zmienne
  * *Element*, czyli klasę dla obiektu umieszczanego na stosie. Zawiera zmienną *Value* w której znajduje się obiekt który chcemy przechowywać, oraz *Next* wskazujący na *Element* znajdujący się na stosie bezpośrednio poniżej danego
* Kluczowe metody do zaimplementowania:
  * *Push* - dodaje element do stosu
  * *Pop* - zdejmuje element ze stosu
  * *Peek* - "podgląda" tj. zwraca bez usuwania ze stosu element na szczycie
  * *isEmpty*
  * *size*
  * *clear*
* Dodatkowo warto zaimplementować takie metody jak *contains*, *indexOf* etc.

**2. Kolejka (5 pkt.)**

* Zaimplementowanie własnej kolejki na bazie referencji
* Kolejka powinna przechowywać elementy dowolnego typu
* Implementacja na bazie referencji oznacza zdefiniowanie odpowiednich klas:
  * *Queue*, czyli klasa z którą będziemy daną strukturę identyfikować i wywoływać z jej poziomu metody. Zawiera zmienną *Head*, która identyfikuje element na początku kolejki, *Tail* która identyfikuje element na końcu kolejki oraz inne, pomocniczne zmienne
  * *Element*, czyli klasę dla obiektu umieszczanego w kolejce. Zawiera zmienną *Value* w której znajduje się obiekt który chcemy przechowywać, *Next* wskazujący na *Element* następny w kolejce i (opcjonalnie) *Prev* który wskazuje *Element* poprzedzający
* Kluczowe metody do zaimplementowania:
  * *Enqueue* - dodaje element na koniec kolejki
  * *Dequeue* - usuwa element z początku kolejki
  * *Peek* - "podgląda" tj. zwraca bez usuwania z kolejki jej pierwszy element
  * *isEmpty*
  * *size*
  * *clear*
* Dodatkowo warto zaimplementować takie metody jak *contains*, *indexOf* etc.
