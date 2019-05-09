## Zadanie 6: Drzewa i kopce dwumianowe

* Termin zajęć: 09/05/2019
* Termin oddania: 16/05/2019
* Sposób zaliczenia: prezentacja na zajęciach
* Punkty: 15

## Opis zadania

**1. Drzewo dwumianowe (5 pkt.)**

1.1 Ogólne

* Drzewo dwumianowe ma zawsze 2^k elementów, gdzie k to stopień drzewa
* Drzewo dwumianowe o stopniu k składa się z drzewa dwumianowego o stopniu k-1, k-2, ... , k - k

1.2 Wymagania
* Zaimplementowanie rekursywnej struktury drzewa dwumianowego
  * Klasa na element drzewa
  * Klasa na samo drzewo
* Zaimplementowanie metody łączenia dwóch drzew dwumianowych
* Zaimplementowanie podstawowych metod:
  * Konstruktory parametryczne (z elementu lub ze stopnia)
  * *clear*
  * *size*
  * *isEmpty*
  * *print*
* Zaimplementowanie graficznej reprezentacji ***(nieobowiązkowe, +1 pkt)***

**2. Kopiec dwumianowy (10 pkt.)**

1.1 Ogólne

* Kopiec dwumianowy to zbiór drzew dwumianowych
* W danym kopcu dwumianowym może znajdować się tylko jedno drzewo dwumianowe o danym stopniu
* Wszystkie drzewa wewnątrz kopca dwumianowego są uporządkowane kopcowo, tj. klucz danego elementu jest nie mniejszy niż klucz rodzica

1.2 Wymagania

* Zaimplementowanie struktury kopca dwumianowego
  * Z wykorzystaniem uprzednio zaimplementowanego drzewa dwumianowego
  * W postaci klasy kopca dwumianowego przechowującej drzewa dwumianowe
* Zaimplementowanie metody wyszukiwania minimalnego drzewa dwumianowego na kopcu, tj. z najmniejszym korzeniem
* Zaimplementowanie metody łączenia dwóch kopców dwumianowych
* Zaimplementowanie metody *zmniejszającej* wartość klucza danego potomka w określonym drzewie
* Zaimplementowanie podstawowych metod:
  * Konstruktor nieparametryczny
  * Konstruktor parametryczny (z drzewa dwumianowego)
  * *clear*
  * *size*
  * *isEmpty*
  * *print*
  * *insert*
  * *remove*
 * Zaimplementowanie graficznej reprezentacji ***(nieobowiązkowe, +1 pkt)***
