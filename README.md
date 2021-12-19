# PRiR zadania lab 9
Efektywność środowiska CUDA w Google Colab na podstawie algorytmu liczącego zbiór Mandelbrota
Dane wejściowe:
- Wycinek {-1. 0.0} {-0.5 0.5}
- Iteracje próbkowania - 256
- 
Rozmiar: 
- dla CPU: 1000x1000 (na potrzeby obliczeń przyśpieszenia wynik mnożony jest razy 100)
- dla GPU: 10000x10000


&nbsp; | Wersja CPU | Wersja 1D 128 wątków | Wersja 2D 8x16 wątków | Wersja 1D 32 wątki | Wersja 2D 8x4 wątków | Wersja 1D 16 wątków | Wersja 2D 4x4 wątków
--- | --- | --- | --- | --- | --- | --- | --- 
&nbsp; | 1.324761 | 0.467153 | 0.591118 | 0.589712 | 0.732755 | 0.979265 | 0.1021822 ```halko ``` 
&nbsp; | 1.361270 | 0.268454 | 0.360448 | 0.377719 | 0.436735 | 0.668177 | 0.760824
&nbsp; | 1.355375 | 0.241209 | 0.325455 | 0.381538 | 0.422064 | 0.666395 | 0.760183
&nbsp; | 1.350882 | 0.224091 | 0.321363 | 0.382268 | 0.423905 | 0.666302 | 0.758028
&nbsp; | 1.354562 | 0.227449 | 0.323251 | 0.379849 | 0.424684 | 0.664782 | 0.759824
&nbsp; | 1.368545 | 0.226171 | 0.321221 | 0.379140 | 0.424622 | 0.670371 | 0.762265
&nbsp; | 1.334326 | 0.228137 | 0.317735 | 0.378515 | 0.425582 | 0.667938 | 0.761594
&nbsp; | 1.380336 | 0.226318 | 0.321999 | 0.380004 | 0.423138 | 0.666500 | 0.759610
&nbsp; | 1.373423 | 0.225304 | 0.319872 | 0.380832 | 0.423866 | 0.667634 | 0.757079
&nbsp; | 1.386933 | 0.225243 | 0.321628 | 0.381524 | 0.424085 | 0.667744 | 0.758745 
min | 1.334326 | 0.224091 | 0.317735 | 0.377719 | 0.422064 | 0.666302 | 0.758028
przyśpieszenie względem CPU | 1x | 595x | 420x | 353x | 316x | 200x | 176x
![](p1.PNG)<br><br>
