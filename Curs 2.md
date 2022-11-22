# Notiunile de senzori si traductori

Aceste echipamente sunt pe larg folosite in sistemele de automatizare. Pentru a face o diferentiere intre cele doua notiuni, s-a introdus notiunea de traductor de intrare (dispozitivul cu intrare non-electrica si iesire electrica: senzor) si traductor de iesire (intrarea este electrica si iesirea non-electrica: actuator).

$$
\xrightarrow[nonelectrica]{intrare}\overset{TI}{\boxed{Senzor}}\xrightarrow[electrica]{iesire} 
\hspace{1.5cm}
\xrightarrow[electrica]{intrare}\overset{TE}{\boxed{Actuator}}\xrightarrow[nonelectrica]{iesire} 
$$

Cele doua notiuni pot fi diferentiate daca se are in vedere ca senzorul constituie partea de detectie, iar traductorul realizeaza, impreuna cu senzorul, marimea masurata.

## Traductorul

Intr-o acceptiune unanima, un traductor face trecerea de la un tip de semnal la altul, adica utilizeaza energia marimii de masurat in procesul de conversie. Energia folosita in procesul de conversie poate fi preluata integral in cazul marimilor active sau partial in cazul marimilor pasive. Puterea nu trebuie sa depaseasca o valoare precizata numita *putere disponibila*. 

Intrucat exista sase calse de semnale: mecanic, termic, magnetic, electric, radiant si chimic, orice dispozitiv care face trecerea dintr-un tip de semnal in celalalt poate fi un traductor. Totusi, doar dispozitivele care au iesire electrica sunt numite traductoare.

Datorita structurii electronice a materiei, exista cel putin o modalitate electrica de investigare a marimilor non-electrice. 

Dispozitivele si circuitele electronice capabile sa preia semnalele de la elementele sensibile ale traductoarelor sunt accesibile.

Semnalele electrice pot fi prelucrate, memorate, afisate si transmise la distanta prin procedee consacrate.

Traductoarelor le sunt specifice doua restrictii:

- se impune proportionalitatea intrare-iesire, deci o caracteristica statica liniara

- pentru usurinta utilizarii, semnalul electric de iesire este standardizat

**Concluzii:**

- traductorul este un element al instalatiei de automatizare care ofera un semnal electric in iesire
- traductorul are caracter dual
- valorile obtinute in iesirea traductorului sunt proportionale cu interarea si oferite sub forma de semnal electric unificat (calibrat) 

**Definitie:**

Traductorul este dispozitivul folosit pentru investigarea unei variable de proces cu limite de variatie predefinite care ofera in iesire un semnal electric calibrat, in concordanta cu o stare de masurare precizata. 

In consecinta, traductorul poate fi considerat interfata intre proces si dispozitivele de automatizare si poate fi reprezentat cu simbolul $T$.

## Senzorul

Exista trei categorii de senzori:

- fizici

- chimic

- biosenzori (senzori moleculari)

Un senzor fizic incearca sa imite comportamentul unui organ uman de simt, dar **nu** principiul de functionare. 

Un senzor trebuie sa aiba dimensiuni mici si, deoarece se masoara o scena de lucru, definitia se extinde catre arie sau matrice de senzori.

**Definitie:**

Un senzor este un dispoztiv de foarte mici dimensiuni care permite determinarea unui camp de valori pentru marimea investigata intr-un mod similar comportamentului uman.

---

Vom folosi diferentiat notiunile de senzor si traductor in functie de modul de operare si aplicatii. Totusi, in vorbirea curenta, cele doua notiuni se folosesc interschimbabil, deoarece ambele elemente realizeaza operatia de baza (operatia de masurare).

Totusi, senzorilor le sunt specifice urmatoarele operatii:

- miniaturizarea senzoriala

- multiplicarea senzoriala - presupune unitati identice plasate pe aceeasi structura

- fuziunea senzoriala - presupune senzori diferiti principial folositi pentru detectia unei marimi

Aceste trei caracteristici, impreuna cu proprietatea de imitare a comportamentului uman fac diferenta fata de traductoare.

*Transmitter* reprezinta un dispozitiv ce permite transmiterea semnalului la distanta.

In literatura, se intalnesc notiunile de senzor/traductor inteligent. Aceasta denumire este atribuita echipamentelor de sine-statatoare care, pe langa comunicatia cu postul dispecer, realizeaza suplimentar functii de calcul, calibrare si autotestare (pentru verificarea funtionala).

## Clasificare

**Criterii:**

- dupa necesitatea unei surse auxiliare de activare:
  
  - traductoare active (tip generator) - senzori directi
  
  - traductoare pasive (tip parametrice) - seznori cu modulare

- dupa semnalul de iesire:
  
  - traductoare analogice: iesirea este functie continua in raport cu intrarea
  
  - traductoare numerice: se obtin stari distincte ale iesirii in functie de modul de realizare a elementului sensibil
  
  - traductoare cvasinumerice: au ca intrare o marime continua, iar iesirea este o frecventa sau durata de impuls

- dupa principiul care sta la baza transferului de energie intrare-iesire:
  
  - traductoare in regim dezechilibrat
  
  - traductoare cu echilibrare automata: tendintei de dezechilibru din intrare i se opune prin reactie un semnal care compenseaza dezechilibrul (ex: traductoare de presiune cu element elastic)

- dupa dinamica: sisteme de ordin 0, 1, 2, etc.

- dupa marimea masurata

- dupa numarul de porturi

- dupa principiul functional care sta la baza realizarii partii de intrare a traductorului:
  
  - rezustuve, capacitive, inductive, optice, acustice
  
  - cu acumulare de sarcina, cu generare de tensiune/curent

- dupa cantitatea de informatii oferita:
  
  - senzori binari
  
  - senzori analogici
  
  - senzori de imagine
