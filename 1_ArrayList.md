## Zadanie 1: Lista

* Termin zajęć: 7.03.2019
* Termin oddania: 14.03.2019
* Sposób zaliczenia: prezentacja na zajęciach
* Punkty: 5

## Opis zadania

**1. Lista (1 pkt.)**

* Zadanie polega na zaimplementowaniu własnej listy (*ArrayList*) na bazie struktury *Array*
* Typ elementów przyjmowanych przez listę powinien być definiowany przez użytkownika w procesie deklaracji nowej listy w kodzie
* Proszę rozważyć możliwe strategie powiększania *Array* w momencie przekroczenia jej długości

**2. Metody (1 pkt.)**

* W ramach zadania wymagane jest poprawne zaimplementowanie podstawowych metod listy, mianowicie:

	* *size*
	* *isEmpty*
	* *contains*
	* *indexOf*
	* *get*
	* *set*
	* *add*
	* *remove*
	* *clear*
* W razie wątpliwości co do zamierzonego działania poszczególnyych opcji, proszę posiłkować się [oficjalną specyfikacją listy](https://docs.oracle.com/javase/8/docs/api/java/util/List.html)

**3. Iterator (3 pkt.)**

* Implementacja powinna zawierać iterator, co wymaga następujących czynności:
	* Zastosowanie operatora *implements*
	* Użycie instrukcji *@override* celem nadpisania podstawowych metod iteratora (*hasNext*, *next*, *remove*)
* Iterator należy wykoszystać w metodach listy które wymagają przesukiwania (np. *contains*).

## Materiały

* Poniżej zamieszczam ściągawkę ogólnego schematu programu.

```Java
import (...)


public class MyList<T> implements Iterable<T> {

    private Object[] data;
    private int default_size;
    
    public MyList(){
    }
    
    public int size(){
    }
    
    public void add(T elem){
    }
    
    (...)
    
    
    @override
    Iterator<Type> iterator(){
        Iterator<Type> iterator = new Iterator<Type>() {

            private int currentIndex = 0;

            @Override
            public boolean hasNext() {

            }


            @Override
            public Type next() {

            }

            @Override
            public void remove(){

            }
        };

        return iterator;
    }
}
```
