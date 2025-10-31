#problema medianei

variante: 
1)mediana simpla - gasirea unui nod intr-un graf care minimizeaza suma distantelor catre celelalte noduri:
Formulă:
$$ v^* = \min_v \left[ \sum_{u \in V} d(v, u) \right] $$
- v* este nodul care minimizeaza suma distantelor fata de toate celelalte noduri 

2) mediana ponderata- fiecare nod are o importanta specifica, de exemplu distanta unui nod poate fi multiplicata cu importanta lui( un nod important va avea o pondere mai mica la distanta totala) 
$$ v^* = \min_v \left[ \sum_{u \in V} w(u) \cdot d(v, u) \right] $$
        -w(u)= ponderea

3) mediana pe grafuri orientate – la fel ca mediana simpla doar ca pe un graf orientat

$$ v^* = \min_v \left[ \sum_{u \in V} d(v, u) \right] $$

4)problema medianei dinamice- grafurile pot fi dinamice, adica sa se schimbe distanta in functie de timp


algoritmi de rezolvare: 
Calculăm toate distanțele minime (de exemplu cu algoritmul Dijkstra)
Algoritmi euristici (Greedy)
Metaeuristici:  algoritmi genetici.
. 
5) suma distantelor minime de la nodul v catre toate celelalte noduri calculata cu djikstra
$$ cost(v) = \sum_{u \in V} d(v, u) $$

si functia de fitness
$$ fitness(v) = \frac{1}{1 + cost(v)} $$
