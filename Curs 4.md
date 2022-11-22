# Caracteristici dinamice

## Indicatori de calitate dedusi in regim dinamic

Regimul dinamic preupune ca atat intrarea cat si iesirea traductorului sunt variabile in timp. Cum traductoarele au o caracteristica statica liniara, dinamica se poate exprima prin ecuatia diferenitala $\sum_{k=0}^na_ky^{(k)}(t)=\sum_{j=0}^mb_jx^{(j)}(t)$. Coeficientii $a_k$ si $b_j$ sunt constanti, intrucat traductorul este o componenta construita. Se indeplineste conditia de realizabilitate fizica, adica $m>n$.

Rezolvarea ecuatiei diferentiale se face pentru intrari tipice caracteristice traductorului.  Se evidentiaza doua cai:

- raspunsul in timp: presupune gasirea lui $y$ folosind calculul operational 

- determinarea raspunsului in frecventa: presupune aplicarea unui semnal sinusoidal cu amplitudinea constanta si frecventa variabila pe o plaja larga de valori

Din punct de vedere dinamic, un traductor are in componenta sa unul sau cel mult doua elemente acumulatoare de energie de natura mecanica, termica sau electromagnetica astfel ca, in regim dinamic, comportamentul este descris de functii de transfer de ordinul 1 sau ordinul 2.

### Element de intarziere de ordinul I

$a_1\frac{dy}{dt}+a_0y(t)=b_0x(t) \overset{\mathscr{L}}\implies H(s)={k\over1+Ts}$

**Indicatori:**

- eroarea dinamica $\varepsilon_D$: $\varepsilon_D(t)=y(t)-y_s$

- timpul de stabilizare $t_s$: $|\varepsilon_D(t)|\le B_s, \forall\ t\ge t_s$
  
  - are durata $3T$ pt banda ±3% si $4T$ pentru banda ±5%

- constanta de timp T se poate pune in evidenta ca fiind valoarea valoarea tangentei pentru $t=0$: ${k\over T}=tg(\alpha)$

- pulsatia de banda $\omega_B$: $\omega_B={1\over T}$

### Element de intarziere de ordinul II

$a_2{d^2y\over dt^2}+a_1{dy\over dt}+a_0y(t)=b_0x(t)\overset{\mathscr{L}}\implies H(s)={k\over T^2_a s^2+T_bs+1}$

Daca radacinile ecuatiei caracteristice sunt reale, raspunsul in timp duce la regimul aperiodic supraamortizat, adica iesirea parurge drumul de la $0$ la $y_s$ intr-un timp indelungat.

Daca radacinile ecuatiei caracteristice sunt egale, raspunsul in timp este aperiodic critic, in care valoarea de regim stationar este atinsa in cel mai scurt timp.

Daca radacinile sunt complex conjugate, in timp se obtine oscilatoriu amortizat. 

In practica, cea mai utilizata solutie este regimul oscilatoriu amortizat.

Se poate nota

$T_a^2={1\over \omega_R^2}$ si $T_b={2\xi\over \omega_n},\ 0<\xi<1$.

**Indicatori**:

- timupl de crestere $t_c$: durata in care iesirea parcurge distanta de la $0.1y_s$ si $0.9ys$ 

- perioada oscilatiilor amortizate $T$: care are valoarea $T={2\pi\over\omega}$

- supracresterea $\sigma$: eroarea dinamica corespunzatoare primului maxim al iesirii; de obicei se exprima in procente $\sigma_r[\%]={y_{max}-y_s\over y_s}*100$

- timpul de stabilizare $t_s$: $|\varepsilon_D(t)<B_s,\forall\ t\ge t_s$

- pulsatia de rezonanta $\omega_r$: valoarea pentru care $H'(w)=0$, adica $\omega_r=\omega_n\sqrt{1-2\xi^2}$

- pulsatia de banda $\omega_B$: valoarea pentru care amplitudinea $H(\omega_B)={H(0)\over\sqrt2}$

Daca $w_n$ creste si $\xi$ ramane constant, pulsatia de banda creste, deci dinamica se imbunatateste. Daca $\xi$ creste si $\omega_n$ este constanta, dinamica se inrautateste.

# Caracteristici energetice

Traductoarele efectueaza operatia de masurare, care presupune un consum energetic. Aceste consum este total la marimile active, sau partial la marimile parametrice. 

Puterea, care prin integrare in timp da energia, nu trebuie sa depaseasca o valoare denumita putere disponibila. 

Se considera o marime $X$ supusa operatiei de masurare careia i se ataseaza o marime $Y$ astfel incat produsul lor sa fie de natura unei puteri, iar raportul lor de natura unei impedante (impedanta meteorologica): $P=XY$, $Z_m={X\over Y}$. Un traductor este cu cat mai bun cu cat $Z_m$ este mai mare. Aceasta poate fi crescuta prin scaderea masei si dimensiunilor. 

La marimile active trebuie indeplinita conditia $Z_s\ll Z_m$, prin utilizarea de amplificatoare.

La marimile pasive se utilizeaza o sursa auxiliara de energie. Se considera doua aspecte: sursa externa sa fie folosita pentru a evidentia marimea parametrica; valorile practice nu trebuie sa conduca la eronarea rezultatului.

In prezent, firmele constructoare de traductoare folosesc circuite si tehnologii de ultima generatie cu consum energetic foarte redus (*ultra low power*).

# Caracteristici constructive

**Indicatori**:

- robustete: calitatea traductorului de a dispune de stabilitate in functionare 

- capacitatea de supraincarcare: proprietatea unui traductor de a suporta valori ale marimii de masurate care depasesc limita superioara a domeniului pentru care este destinat

- protectia climatica: in concordanta cu zonele climatice 

- protectia contra exploziilor: o serie de masuri specifice aplicate in constructia si montarea traductoarelor pentru a evita aprinderea atmosferelor explozive exterioare.

- protectia anticoroziva

# Caracteristici de fiabilitate

Fiabilitatea poate fi: previzionala, experimentala si operationala.

- previzionala: calcule facute in prealabil pentru fiabilitate

- experimentala: incercari accelerate de fiabilitate 

- operationala: urmarirea in functionare a produslui
