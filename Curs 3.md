## Locul si rolul traductoarelor in sistemele automate

Marimea de referinta $y_{ref}$ se compara in cadrul comparatorului diferential cu marimea de reactie $y$ si se obtine marimea de eroare $\varepsilon$. In concordanta cu legea de reglare din blocul R, se elaboreaza marimea de comanda $u$ care produce in elementul de actionare marimea de actionare $w$. Actionarea se produce in sensul micsorarii erorii stationare. Traductorul este pe calea informationala, oferind cantitativa despre variabila investigata. 

In automatizarea realizata in lumea digitala, preluarea marimilor de proces, respectiv transmiterea comenzilor catre proces se face in doua moduri. La procesul 1, atat traductorul cat si dispozitivul de actionare sunt conectate la o interfata de conversie si comunicatie (ICC). Aceasta modalitate este evidentiata la structurile de traductoare inteligente capabile sa preia din sarcinile sistemului de automatizare, reducandu-se consumul de timp si resurse. La nivelul procesului 2, se evidentiaza ICC-uri dedicate: pentru traductoare ICCT, respectiv pentru dispozitive de actionare ICCTA. Aceasta modlitate se intalneste la sistemele de achizitie/distributie a datelor (SAD/SDD). 

In continuare, prin magistrala de camp, se trece la nivelul de conducere locala, unde sunt plasate automate programabile.

Prin magistrala locala de aplicatie (MLA) se trece la nivelul de aplicatie unde este plasat serverul de aplicatie SA1 cu rezerva calda SA2. La nivel de aplicatie se afla consola operatorului de proces (CP) prin care specialistul automatist poate interveni in procesul de conducere.

La nivel de intreprindere, prin magistrala locala de intreprindere, se afla conducerea numerica de intreprindere (CNI), iar prin retele extinse se ajunge la nivel de corporatie.

## Structura generala a unui traductor

Privit din punctul de verede al definitiei, orice traductor are in componenta sa urmatoarele elemente:

- ES: element sensibil

- A: adaptor

- ELT: element de legatura si transmisie

- SAE: surse auxiliare de energie 

**Elementul sensibil** asigura cuplarea cu procesul. Are o serie de proprietati:

- selectivitatea: elementul sensibil trebuie sa fie sensibil numai la marimea pentru care a fost construit si sa rejecteze celelalte marimi ale mediului in care se face masurarea 

- sa nu exercite efect de retroactiune catre marimea investigata 

- sa permita cuplari diverse cu marimea investigata

Semnalul S1 din iesirea elementului sensibil este un semnal electric necalibrat, continand pe langa informatia utila si componente parazite care trebuie eliminate.

**Adaptorul** are dublu rol:

- preia semnalul de la elementul sensibil si prin transformari cu caracter liniar sau neliniar asigura in iesire semnalul electric calibrat 

- permite cuplarea pe iesire a elementelor din bucla de reglare fara sa apara efect de retroactiune catre intrare

Curentul continuu cu 0 decalat este cel mai folosit ca semnal de iesire. Daca iesirea este $0mA$ se semnifica o stare de defect. 

Curentul continuu poate fi transmis la distanta intrucat rezistenta de sarcina $R_s\in\left[0\Omega, 800\Omega\right]$. 

Semnalul de curent permite scurtcircuit in iesirea traductorului.

**Elementele de legatura si transmisie** asigura conexiuni simple intre ES si A de natura mecanica, electrica, optica, termica, etc.

**Sursele auxiliare de energie** alimenteaza circuitistica auxiliara si de intrare a traductorului.

## Caracteristicile si performantele traductoarelor

### Caracteristici in regim static

Regimul stationar presupune ca atat intrarea, cat si iesirea traductorului sunt invariante in timp pe durata de observatie. Se considera ca pe intervale reduse de timp se asigura invarianta intrarii si iesirii astfel ca dependenta $y=f(x)$ reprezinta caracteristica statica ideala a traductorului in absenta marimilor de influenta. 

Traductorul are o buna selectivitate daca sensibilitatile marimilor de influenta sunt mult inferioare sensibilitatilor utile. Se considera caracteristica statica a traductorului ca fiind $y=f(x)$, iar efectul marimilor de influenta se va regasi in eroarea de neliniaritate care insoteste traductorul respectiv.

Pe domeniul mari de functionare, traductoarele au o caracteristica statica neliniara, aproximarea prin una liniara facandu-se in limite unor erori. Un traductor are o functionare pe o caracteristica statica liniara daca eroarea de neliniaritate este inferioara unei valori impuse 

Sensibilitatea se exprima ca $S=\frac{dy}{dx}$.

Clasa de precizie este data eroarea admisibila de baza data in forma normata (raportata la domeniu). $c=\frac{|\Delta X_{ad}|}{x_{max}-x_{min}}$ Eroarea admisibila de baza este data pentru valori ale mediului in care se face masurarea sub forma de intevale de referinta.

In prezent, constructorii de traductoare folosesc materiale si tehnologii care conduc la erori admisibile suplimentare neglijabile pe domeniile nominale de functionare ale traductoarelor.

Rezolutia este saltul elementar din intrare care produce o crestere elementara in iesire.

Repetabilitatea este abiltatea unui traductor de a reproduce valori apropiate in iesire atunci can intrarea ia aceeasi valoare.

Reproductibilitatea este asemanatoare repetabilitatii  cu observaita  ca experimentele se fac la momente de timp diferite de operatori diferiti cu instrumentatie diferita.


















