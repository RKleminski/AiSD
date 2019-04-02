## Zadanie 3: Algorytmy sortowania

* Termin zajęć: 21.03.2019
* Termin oddania: 11.04.2019
* Punkty: 20
* Sposób zaliczenia: przesłanie programu i sprawozdania w wersji elektronicznej do wyznaczonego terminu

## Opis zadania

**1. Algorytmy sortowania (12 pkt.)**

1.1. Algorytmy

* W ramach realizacji zadania należy zaimplementować *dokładnie* trzy algorytmy sortowania z udostępnionej listy
  * Każdy algorytm sortowania ma przypisaną do niego liczbę punktów, tj. maksymalną liczbę punktów jaka zostanie przyznana za poprawną implementację
  * W przypadku implementacji więcej niż trzech algorytmów, ocenione zostaną tylko trzy o największej wartości punktowej
* Ocenie podlega:
  * Zgodność implementacji z algorytmem
  * Poprawność działania, tj. faktyczna zdolność sortowania
  * Raportowana złożoność obliczeniowa *(w umiarkowanym stopniu, więcej informacji u prowadzącego)*

| Algorytm | Punkty | Uwagi |
| :---: | :---: | --- |
| Bubble-sort | 2 | |
| Selection-sort | 2 | |
| Insertion-sort | 2 | |
| Bucket-sort | 3 | |
| Merge-sort | 3 | |
| Comb-sort | 3 | |
| Library-sort | 4 | W badaniach porównać ze sobą diałanie <br> przy zastosowaniu conajmniej dwóch <br> różnych wartości parametru epsilon |
| Shell-sort | 4 | W badaniach porównać ze sobą działanie <br> przy zastosowaniu conajmniej dwóch <br> różnych ciągów odstępów |
| Quicksort | 4 | |

1.2. Interfejs

* Stworzenie prostego interfejsu pozwalającego na przeprowadzenie szybkich testów programu
* Forma interfejsu (graficzny/tekstowy) jest całkowicie dowolna
* Interfejs powinien pozwalać na wybór:
  * Algorytmu sortowania do testu
  * Stopnia posortowania ciągu testowego
  * Długości ciągu testowego
* Opcjonalnie można pozwolić na wczytanie ciągu z pliku

**2. Badania (8 pkt.)**

2.1. Badania

* Badania przeprowadzane są poprzez posortowanie każdej kombinacji długość-stopień posortowania sto razy każdym z zaimplementowanych algorytmów
* Czas każdego z wymienionych sortowań należy zmierzyć odpowiednią funkcją, a wynik zapisać do późniejszego wykorzystania
* Proszę zwrócić uwagę, że obciążenie systemu wpływać będzie na szybkość działania programu - przed badaniami zalecane jest wyłączenie wszystkich innych programów (w miarę możliwości), lub upewnienie się, że całość badań przebiega na identycznym/porównywalnym obciążeniu systemu
* Proszę również pamiętać o obciążeniach i opóźnieniach wynikających z inicjalizacji maszyny wirtualnej Javy; w niektórych przypadkach może się zdarzyć, że pierwszy wynik pomiaru będzie z tego powodu znacząco wyższy niż pozostałe. Odrzucenie takiego wyniku do sprawozdania jest zalecane, ale należy o nim wspomnieć

2.2. Ciągi testowe

* W badaniach należy wykorzystać ciągi o następujących długościach (w elementach):
  * 100 tys.
  * 500 tys.
  * 1 mln
  * 2 mln
* W badaniach należy wykorzystać ciągi o następujących stopniach posortowania:
  * W pełni losowy
  * Posortowany w 50%
  * W pełni posortowany
  * Posortowany odwrotnie
* Dla uzyskania najbardziej miarodajnych wyników, zalecane jest wygenerowanie stu różnych ciągów dla każdej kombinacji długość-stopień posortowania i zapisanie na dysku, celem wykorzystania w badaniach
* Dla uzyskania najbardziej miarodajnych wyników, zalecane jest generowanie ciągów o pewnym stopniu posortowania przez zastosowanie jednej z zaimplementowanych metod na ciągu losowym. Generowanie częściowo posortowanego ciągu za pomocą pętli `for` jest dopuszczalne, ale odradzane

```python
# Pseudokod procesu badań:

for algorithm in sorting_algorithms:
    for sequence_length in sequence_lengths:
        for sequence_type in sequence_types:
            for sequence_ID in range(0, 100):
                sort_sequence(algorithm, sequence_length, sequence_type, sequence_ID)
```


2.3. Sprawozdanie
* Struktura sprawozdania, przy poszczególnych sekcjach wymienione przykładowe informacje jakie można w nich zawrzeć:
  * Krótkie wprowadzenie teoretyczne
    * Ogólny opis działania wybranych algorytmów
    * Teoretyczna złożoność obliczeniowa algorytmów
  * Opis schematu i przebiegu badań
    * Sposób generowania ciągów
    * Obciążenie systemu i działania na celu wyrównania
    * Sposób pomiaru czasu i organizacja funkcji testowych
  * Prezentacja wyników
    * Analiza statystyczna wyników (czas średni, odchylenie standardowe)
    * Identyfikacja obserwacji odstających
    * Prezentacja graficzna: wykresy ilustrujące wyniki
  * Analiza wyników
    * Omówienie obserwacji odstających
    * Omówienie różnic w działaniu algorytmów w zależności od typu posortowania ciągu
    * Porównanie zaobserwowanej złożoności obliczeniowej z teoretyczną
  * Wnioski
    * Podsumowanie obserwacji
    * Identyfikacja możliwych błędów i/lub przyczyn rozbieżności z teorią
