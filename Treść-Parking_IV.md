# Parking (IV)
Parking składa się z 32 stanowisk postojowych. Pojazdy wjeżdżają na parking i opuszczają go. Czujniki monitorują zajętość miejsc i przesyłają do systemu informatycznego skompresowaną informację w postaci 32-bitowej liczby w kodzie U2 przy założeniu, że 1 oznacza miejsce zajęte, a 0 miejsce wolne. Napisz program, który poda informację o liczbie pojazdów, które opuściły parking.
## Wejście
W pierwszym wierszu wejścia liczba całkowita w kodzie U2 w systemie dziesiętnym oznaczająca informację na temat zajętości miejsc.
W drugim wierszu wejścia liczba całkowita w kodzie U2 w systemie dziesiętnym oznaczająca informację na temat zajętości miejsc po krótkiej chwili (na tyle krótkiej, że w jej trakcie nie dochodzi do sytuacji, w której jakiś pojazd zdąży zaparkować na zwolnionym przed chwilą miejscu lub inny pojazd zdąży zaparkować na wolnym miejscu i odjechać).
## Wyjście
Liczba całkowita z przedziału <0; 32> - liczba pojazdów, które opuściły parking.
## Przykład
### Wejście:
```
-19415
-197151703
```
### Wyjście:
```
5
```
Wyjaśnienie do przykładu: Zajęte i wolne stanowiska zapisane w postaci liczby -19415 odpowiadają ciągowi bitów 11111111111111111011010000101001, w którym są 23 jedynki (czyli zajęte miejsca).
Po chwili sytuacja zmienia się i zajęte i wolne miejsca zapisane w postaci liczby -197151703 odpowiadają ciągowi bitów 11110100001111111011010000101001.
W przedstawionej sytuacji 5 pojazdów opuściło parking (pozycje 5, 7, 8, 9 i 10 od lewej).
