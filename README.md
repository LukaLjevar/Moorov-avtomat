# Nedeterministični Mooreov avtomat
Projektna naloga pri predmetu Programiranje 1.

Projekt vsebuje implementacijo nedeterminističnega Moorovega avtomata, ki kot vhod sprejme dva niza - niz1 in niz2. Nato avtomat preveri, ali niz2 vsebuje niz1 kot strnjeni podniz. Na podlagi prejetega niza1, program pripravi avtomat, ki bo preverjal, ali nek niz vsebuje niz1 kot podniz. Avtomat je nedeterminističen, kar pomeni, da se lahko nahaja v večih stanjih naenkrat. Niz2 je sprejet, če je po koncu izvajanja programa vsaj eno izmed (lahko večih) stanj, v katerih se nahaja avtomat, sprejemno. Avtomat je opremljen še z dodatno funkcijo, odvisno od trenutnih stanj, ki po koncu izvajanja enega preverjanja vrne element tipa unit in natisne seznam vseh trenutnih stanj. Zato govorimo o Moorovem avtomatu. 

## Matematična definicija
Nedeterministični Mooreov avtomat opišemo kot šesterico $(S, \ s_{0}, \ \Sigma , \ O, \ \delta , \ G)$, kjer je: 
- $S$ končna množica stanj, v katerih se lahko avtomat nahaja,
- $s_{0} \in S$ začetno stanje, torej stanje, v katerem avtomat prične,
- $\Sigma$ končna množica simbolov oziroma abeceda, ki jo sprejme naš avtomat,
- $O$ končna množica simbolov, ki jo naš avtomat vrača
- $\delta :S'\times \Sigma \rightarrow S''$ prehodna funkcija, ki $S' \subset S$ preslika v $S'' \subset S$, torej starim stanjem priredi nova stanja
- $ G:S'\rightarrow O $ izhodna funkcija, ki trenutnim stanjem $S' \subset S$ priredi izhod.


