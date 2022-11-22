# Circuite de prelucrare intermediara

Circuitele de prelucrare intermediara preiau semnalul de la circuitul de intrare si, prin transformari interne, cu caracter liniar sau neliniar realizeaza in iesire o tensiune continua proportionala cu semnalul de intrare. 

**Categorii:**

- de tip liniarizare (unuele dintre cele mai frecvente)

- de tip mediere si redresare: folosite la circuitele de intrare destinate elementelor sensibile, inductive si capacitive

- de tip valoare efectiva: este folosit la semnale multiarmonice, unde se cere exprimarea in raport cu fundamentala

## Circuitul de prelucrare intermediara de tip liniarizare

Elementele sensibile si chiar metodele de masurare au neliniaritati importante care depasesc cu mult cerintele impuse. De exemplu, un element sensibil piezorezistiv folosit la traductoarele de presiune are eroarea de neliniaritate in jurul 5-8%. Un traductor de presiune cu un astfel de element poate avea o eroare de neliniaritate de 0.01%  prin folosirea unor structuri inteligente cu microcontroller (aproximarea polinomiala).

De obicei, firmele constructoare de elemente sensibile prezinta dependenta intrare-iesire sub forma tabelata si rareori sub forma relationala. De exemplu, un termocuplu este data ca $E_{TC}(\theta)$ din $\degree C$ in $\degree C$ pe intervalul $[-200\degree C, 1400 \degree C]$.

Stiind valorile elementului sensibil si modul lui de conectare in circuitul de intrare se poate afla tensiunea de iesire $U_{CI}$ in functie de parametrul respectiv. Rezulta o succesiune de puncte foarte apropiate care intr-o reprezentare normala se confunda cu o functie continua.

Ideal, trebuie generata o caracteristica oglindita, astfel ca functionarea pe aceasta sa duca la eroare de neliniaritate 0. O metoda frecvent folosita la traductoarele analogice este prin aproximarea cu segmente de dreapta a caracteristicii reale, astfel incat pe fiecare segment, in orice punct, eroarea de neliniaritate $\varepsilon_n[\%] \le \varepsilon_{na}$, unde $\varepsilon_{na}$ este eroarea de neliniaritate admisa.

Practic, liniarizarea prin segmente de dreapta se poate face folosind elemente semiconductoare, rezistoare si amplificatoare operationale. Liniarizarea se poate face pe calea directa sau pe reactie. 

Schemele practice de traductoare analogice folosesc structuri de liniarizare plasate pe reactie cu comutatoare electronice bazate pe tranzsitoare de comutatie.

## Convertorul de iesire

Acesta preia semnalul din circuitul de prelucrare intermediara si oferta in iesire semnalul electric calibrat cu liniile normalizate de functionare. 

Deoarece sunt standardizate, exista 2 tipuri de semnale de iesire rezulta doua categorii de converotare:

- tensiune - tensiune

- curent - curent

# Solutii de achizitie si distributie a datelor de la si catre proces

In automatizarea de medie si mare complexitate se folosesc solutii de achizite/distributie in doua variante consacrate reprezentate in figurile a) si b).

Figura a) reprezinta o interfata de conversie si comunicatie bidirectionala. Aceasta configuratie se intalneste la traductoarele inteligente amplasate langa proces capabile de functii suplimentare care degreveaza serverul de aplicatii de operatii mari consumatoare de resurse si timp. 

Figura b) exemplifica principial structurile de achizitie respectiv distributie a datelor de la mai multe traductoare analogice, trecute prin multiplexorul `MUXA`, respectiv mai multe comenzi analogice, trecute prin demultiplexorul `DMUXA`. 

Aceasta configuratie a condus la actualele structuri de sisteme de achizitie a datelor (SAD), respectiv sisteme de distributie a datelor (SDD).

## Sisteme de achizitii de date (SAD)

Pentru prelucrarea, stocarea, afisarea, transmiterea la distanta a datelor digitale se folosesc sisteme de achizitii de date la care trecerea din analog in digial se face printr-un CAN (convertor analog-numeric). Pe langa CAN, intr-un SAD se gasesc:

- circuite de conditionare analogica a semnalului

- dispozitive de esantionare cu retinere

- registrul de memorie temporara

- multiplexoare analogice/digitale

- un bloc de comenzi care garanteaza sincrionizarea operatiilor in SAD 

**Performantele unui SAD:**

- rezolutia si precizia cu care se realizeaza conversia A-N

- numarul canalelor analogice investigate

- frecventa de esantionare pe fiecare canal

- cadenta de transfer prin SAD, adica numarul maxim de esantioane convertite care se obtine la iesire in unitatea de timp

- facilitatile oferite de conditionare a semnalului de intrare

- costul

**Clasificare:**

- in functie de conditile mediului in care lucreaza
  
  - pentru medii de laborator
  
  - pentru medii cu conditii dificile

- dupa numarul de canale
  
  - cu un singur canal
  
  - cu mai multe canale

- din punct de vedere constructiv:
  
  - concentrator de date
  
  - de tip placa multifunctionala 
  
  - de tip inteligent
  
  - de tip instrumente, aparate programabile

## SAD-uri monocanal

Semnalul variabil de proces $x(t)$ este preluat de circuitul de conditionare (CC) cu o structura similara unui traductor analogic. In iesirea CC-ului se obtine un semnal de tensiune cu limite de viariatie din gama de lucru a CAN-ului.

Semnalul analogic este esantionat cu o perioada de esantionare $T_e$. Pe o durata de esantionare $T_e$ trebuie sa se faca conversia analog-numerica si echivalentul numeric sa fie transferat in RT (registrul temporar de memorie).

La structurile plug-in, blocul de comenzi este realizat in cadrul PC-ului, deci SAD-ul nu are control inteligent.

La SAD-urile de tip stand-alone, cu alimentare proprie si transmisie seriala cu PC-ul, blocul de comenzi este realizat de procesorul local.

## SAD-uri multicanal cu multiplexare numerica

## SAD-uri multicanal cu multiplexare analogica


