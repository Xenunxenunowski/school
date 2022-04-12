# Liczby bliźniacze
###  Definicja
Liczyby bliniacze to liczby pierwsze których różnica to 2
### Pseudokod licznik = 1
    wypisz 3 5
    x = 5
    dopóki licznik < n to:
        jeśli Pierwsza(x) oraz Pierwsza (x+ 2) to:
            wypisz x i x+2
            licznik ++
        x = x+6
### Implementacja 
```
#include <iostream>

using namespace std;

bool Pierwsza (int n){
    int d=5;
    if(n==1) return false;
    if (n==2 && n%2==0) return false;
    if(n>3 && n%3==0) return false;
    while(d*d<=n){
        if (n%d==0) return false;
        else if (n%(d+2)==0) return false;
            else d+=6;
    }
    return true;
}

int main()
{
    int licznik =1, x=5,n;
    cout<<"Podaj liczbe par: "; cin >>n;
    cout<<3<<" "<<5<<endl;
    while(licznik<n){
        if ( Pierwsza(x) && Pierwsza(x+2)){
            cout <<x<<" "<<x+2<<endl;
            licznik++;
        }
        x+=6;
    }
    return 0;
}
```
### Przykłady
- 5 i 7
- 11 i 13
- 17 i 19
- 29 i 31

------------

# Liczby zaprzyjaźnione
### Definicja 
Liczby zaprzyjaźnione – para różnych liczb naturalnych, takich że suma dzielników właściwych (mniejszych od tej liczby) każdej z tych liczb równa się drugiej liczbie
### Przykłady
- 220 i 284
- 1184 i 1210
- 2620 i 2924
- 5020 i 5564
------------
# Liczby Mersenne'a

### Definicja 
Liczby Mersenne'a to liczby o postaci M = 2<sup>n</sup> -1 gdzie n jest liczbą naturalną 
### Przykłady 
- 3
- 7
- 31
- 127


------------


# Hipoteza Goldbaha

### Definicja 

każda liczba parzysta większa od 2 jest sumą dwóch liczb pierwszych

