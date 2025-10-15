---
tags:
  - mat
  - analizis
aliases:
  - sorozat
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
share: true
---
## Konvergencia

>[!info] Definíció 
>$a_n$ konvergens és határértéke $A\in\mathbb R$, jelölés:$$\lim\limits_{n\to\infty}a_n=A$$ ha  $\forall\varepsilon>0$-hoz  $\exists N(\varepsilon)\in\mathbb R$, melyre igaz, hogy ha
$n>N(\varepsilon)\Rightarrow |a_n-A|<\varepsilon$ 

Megjegyzés: A definíció ekvivalens azzal, hogy $\forall\varepsilon>0$ az $(A-\varepsilon, A+\varepsilon)$ intervallumon kívül a sorozatnak véges eleme van
## Divergencia

>[!info] Definíció:
>$a_n\rightarrow\infty,$ ha $\forall K\in\mathbb R$-re $\exists N(K),$ hogy $a_n>K$ ha $n>N(K)$
>
 $a_n\rightarrow -\infty,$ ha $\forall K\in\mathbb R$-re $\exists N(K),$ hogy $a_n<-K$ ha $n>N(K)$

## Tételek sorozatokra
#### Határérték egyértelműsége

>[!warning] Tétel
Ha $a_n\rightarrow A$ és $a_n\rightarrow B\Rightarrow A=B$

Bizonyítás: indirekt
Tfh $A\neq B$
legyen $\varepsilon={d\over{3}}$
ekkor $n>N({d\over 3})\Rightarrow |a_n-A|< {d\over 3}\Rightarrow a_n < A+{d\over{3}}$
és  $n>N({d\over 3})\Rightarrow |a_n-B|< {d\over 3}\Rightarrow a_n > B-{d\over{3}}$
tehát $a_n<A+{d\over 3}<B-{d\over 3}< a_n\rightarrow$ ellentmondás

$\Rightarrow$ A=B
#### Konvergencia szükséges feltétele

>[!warning] Tétel
>Ha $a_n\rightarrow A$ (konvergens) $\Rightarrow$ {$a_n, n\in\mathbb N$} korlátos 

Bizonyítás:
$a_n\rightarrow A\Leftrightarrow\forall\varepsilon>0$-hoz $\exists N(\varepsilon),$ hogy ha $n>N(\varepsilon)\Rightarrow|a_n-A|<\varepsilon$

Legyen $\varepsilon=1$     $N(1)=N$
ha $n>N$ és $a_n<A+1$ és $a_n>A-1$
akkor $K_f=max(a_1,a_2,....,a_{n-1},A+1$) és $K_a=min(a_1,a_2,......,a_{n-1},A-1)$ 
tehát korlátos

Megjegyzés: $P\Rightarrow Q\equiv\lnot Q\Rightarrow\lnot P$
Ha nem korlátos akkor nem konvergens

### Határérték és műveletek

#### Összegzés

> [!warning] Tétel
$(a_n\rightarrow A)\land (b_n\rightarrow B)\Rightarrow (a_n+b_n)\rightarrow A+B$

Bizonyítás:
Van két sorozatunk, $a_n\text{ és } b_n$
A konvergencia definíciója szerint:
1. $(a_n\rightarrow A)\Leftrightarrow$ $\forall\varepsilon >0$-hoz $\exists N_a(\varepsilon)$ ha $n>N_a(\varepsilon)$ akkor $|a_n-A|<\varepsilon$
2. $(b_n\rightarrow B)\Leftrightarrow$ $\forall\varepsilon >0$-hoz $\exists N_b(\varepsilon)$ ha $n>N_b(\varepsilon)$ akkor $|b_n-B|<\varepsilon$
Adjuk össze a két összefüggést:
$|a_n-A|+|b_n-B|<2\varepsilon$, amiből következik, hogy
$a_n+b_n-(A+B)<2\varepsilon$ vagy $-a_n-b_n+A+B<2\varepsilon=a_n+b_n-(A+B)>-2\varepsilon$
Tehát $-2\varepsilon<a_n+b_n-(A+B)<2\varepsilon$
Legyen $2\varepsilon=\delta$
$-\delta<a_n+b_n-(A+B)<\delta$

$a_n+b_n\rightarrow A+B$ mert $\forall\delta>0\text{-hoz }\exists N_{a+b}(\delta)=\max(N_a({\delta\over 2}),N_b({\delta\over 2}))\text{  ha   }n>N_{a+b}(\delta)\rightarrow -\delta<a_n+b_n-(A+B)<\delta$
#### Skalárral szorzás
 
>[!warning] Tétel
$(a_n\rightarrow A)\Rightarrow(c\cdot a_n\rightarrow c\cdot A)$

Bizonyítás:
Legyen $a_n$ sorozat
Definíció szerint $a_n\rightarrow A\Leftrightarrow \forall\varepsilon>0$-hoz $\exists N(\varepsilon)$ ha $n>N(\varepsilon)$ akkor $|a_n-A|<\varepsilon$
Tehát $-\varepsilon<a_n-A<\varepsilon$
Szorozzunk fel $|c|$-vel
$-|c|\varepsilon<ca_n-cA<|c|\varepsilon$
Legyen $\delta=|c|\varepsilon$
$-\delta<ca_n-cA<\delta$

Ekkor $ca_n\rightarrow cA$ mert $\forall\delta>0$-hoz $\exists N_{ca}(\delta)=N_a(|c|\varepsilon)$ ha $n>N_a({\delta\over|c|})$
$\Rightarrow$ $|a_n-A|<\delta$

Következmény: $(c_1, c_2)\in\mathbb R^2$
$c_1a_n+c_2b_n\rightarrow c_1A+c_2B$

>[!abstract] Megjegyzés:
Ha van egy $a_n: \mathbb N\rightarrow\mathbb R$ függvényünk, akkor $\lim\limits_{n\to\infty}(a_n)=A$ a függvény [operátora](Oper%C3%A1torok.md) (funkcionálja)

A sorozatok vektorteret alkotnak
(konvergens sorozatok alteret alkotnak)

$\lim\limits_{n\to\infty}(c_1a_n+c_2b_n)=c_1\lim\limits_{n\to\infty} a_n+c_2\lim\limits_{n\to\infty} b_n$
=> limesz egy lineáris funkcionál

#### Sorozatok szorzása

>[!warning] Tétel
$(a_n\to A)\land(b_n\to B)\Rightarrow a_nb_n\to AB$

>[!tip] Lemma: $(a_n\rightarrow 0)\land(b_n\rightarrow 0)\Rightarrow a_nb_n\rightarrow 0$

A tétel bizonyításához először a lemmát bizonyítjuk és majd abból vezetjük le a tételt

Lemma bizonyítása:
Legyen $a_n,$ $b_n$ két sorozat
Konvergencia definíciója szerint
1. $a_n\to 0\Leftrightarrow$ $\forall\varepsilon>0$-hoz $\exists N_a(\varepsilon)$ ha $n>N_a(\varepsilon)$ : $-\varepsilon<a_n<\varepsilon$
2. $b_n\to 0\Leftrightarrow$ $\forall\varepsilon>0$-hoz $\exists N_b(\varepsilon)$ ha $n>N_b(\varepsilon)$ : $-\varepsilon<b_n<\varepsilon$
Szorozzuk össze a két összefüggést
$$
\begin{rcases}
-\varepsilon<a_n<\varepsilon \\
-\varepsilon<b_n<\varepsilon
\end{rcases}\implies-\varepsilon^2<a_nb_n<\varepsilon^2
$$
Legyen $\varepsilon^2=\delta$
Ekkor $a_nb_n\rightarrow 0$ mert $\forall\delta>0$-hoz $\exists N_{ab}(\delta)=\max(N_a(\sqrt{\delta}),N_b(\sqrt{\delta}))$ ha
$n>N_{ab}(\delta)\implies -\delta<a_nb_n<\delta$

Tétel bizonyítása a lemmával:
$a_n-A\to 0$, $b_n-B\to 0$ $\implies$ $(a_n-A)(b_n-B)\rightarrow 0$
A szorzást elvégezve
$a_nb_n-Ab_n-Ba_n+AB\to 0$

$a_nb_n=(a_nb_n-Ab_n-Ba_n+AB)+Ab_n+Ba_n-AB\rightarrow AB$
a zárójeles tag 0-hoz, $Ab_n$ $AB$-hez, $Ba_n$ $BA$-hoz,$-AB$ $-AB$-hez tart tehát az egész tart $AB$-hez

#### Abszolútérték

>[!warning] Tétel
>$a_n\to A\implies |a_n|\to|A|$

Bizonyítás:
A háromszög egyenlőtlenség valós számokra való általánosításából következik, hogy
$||a_n|-|A||\leq|a_n-A|<\varepsilon\implies||a_n|-|A||<\varepsilon$
#### Osztás

>[!warning]- $(a_n\to A)\land (A\neq 0)\Rightarrow \frac{1}{a_n}\to\frac{1}{A}$
>Bizonyítás:
>Legyen $a_n$ sorozat, aminek határértéke nem nulla
>Konvergencia definíciója szerint $a_n\to A\iff\forall\varepsilon>0$-hoz $\exists N(\varepsilon)$ ha $n>N(\varepsilon)$ akkor $|a_n-A|<\varepsilon$ 
>Legyen $\delta=\frac{|A|}{2}$ $\varepsilon=\frac{2\delta}{|A|}$, mert nem akarjuk, hogy $a_n$ túl közel legyen nullához (bármilyen $0<\delta<|A|$ szám megfelelő lenne)
>$|a_n-A|<\delta$
>Ekkor $|a_n|>|A|-|a_n-A|>|A|-\frac{|A|}{2}$ így $|a_n|>\frac{|A|}{2}$ azaz $|a_n|$ nem lesz nullához közel a nevezőben
>Nézzük a törtes kifejezést
>$|\frac{1}{a_n}-\frac{1}{A}|=|\frac{a_n-A}{a_nA}|\longrightarrow$ $|a_nA|=|a_n||A|$ 
>Ha $n>N(\delta)$ akkor $|a_n|>\frac{|A|}{2}$ tehát
>$|\frac{1}{a_n}-\frac{1}{A}|<\frac{|a_n-A|}{\frac{|A|}{2}|A|}=\frac{2|a_n-A|}{|A|^2}$
>
>$\varepsilon$-ban kifejezve
>$|\frac{1}{a_n}-\frac{1}{A}|=|\frac{a_n-A}{a_nA}|<\varepsilon$
>$|\frac{|a_n-A|}{\frac{|A|^2}{2}}|<\varepsilon\implies|a_n-A|<\varepsilon\cdot\frac{|A|^2}{2}$
>$|a_n-A|<\varepsilon\cdot\frac{|A|^2}{2}$ garantálja, hogy
>$|\frac{1}{a_n}-\frac{1}{A}|<\varepsilon$ tehát $\frac{1}{a_n}\to\frac{1}{A}$

#### További tételek

>[!warning] Tétel
$(a_n\rightarrow 0)$ és $b_n$ korlátos => $a_nb_n\rightarrow 0$

Bizonyitás:
Legyen $a_n$ és $b_n$ sorozat és $a_n\to 0$ $b_n$ pedig legyen korlátos
$b_n$ korlátos tehát $\exists K$ ahol $|b_n|<K$ $\forall n\in\mathbb N$
$a_n\to 0\iff\varepsilon>0$-hoz $\exists N_a(\varepsilon)$ ha $n>N_a(\varepsilon)$

$|a_nb_n|<|a_n|K<\varepsilon\cdot K\longrightarrow$ $\delta=\varepsilon\cdot K\implies\varepsilon=\frac{\delta}{K}$ 

$a_nb_n\to0$ mert $\forall\delta>0$-hoz $\exists N_{ab}(\delta)=N_a(\frac{\delta}{K})$, ha $n>N_{ab}(\delta)$ akkor $|a_nb_n-0|<\delta$ 
 
>[!warning] Tétel
$(a_n\rightarrow A)\land (\forall a_n\geq0)\Rightarrow \sqrt{a_n}\rightarrow\sqrt{A}$

Bizonyítás:
$a_n\to A$ tehát $\forall\epsilon>0$-hoz $\exists N(\epsilon)$ hogy ha $n>N(\epsilon)$ akkor $|a_n-A|<\epsilon$
$\implies a_n-A<\epsilon$  mivel $a_n\geq 0$  
$\implies \sqrt{a_n}<\sqrt{\epsilon}\longrightarrow\sqrt{\epsilon}=\delta\implies\epsilon=\delta^2$
Tehát $\sqrt{a_n}\to 0$ mert $\forall\delta>0$-hoz $\exists N_{\sqrt a}(\delta)=N_a(\delta^2)$ hogy ha $n>N_{\sqrt{a}}(\delta)$ akkor $\sqrt{a_n}<\delta$


>[!warning] Tétel
>$a_n\to\infty\implies\frac{1}{a_n}\to 0$

Bizonyítás:
$a_n\to\infty\iff\forall P\in\mathbb R$-hez $\exists N(P)$ hogy ha $n>N(P)$ akkor $a_n>P$
$\implies\frac{1}{a_n}<\frac{1}{P}=\epsilon$
$\frac{1}{a_n}\to 0$ mert $\forall\epsilon>0$-hoz $\exists N(\epsilon)=N_a(\frac{1}{P})$ hogy ha $n>N(\epsilon)$ akkor $|\frac{1}{a_n}|<\epsilon$

>[!warning] Tétel
>$(a_n\to 0\land a_n>0)\implies\frac{1}{a_n}\to\infty$

$a_n\to 0\land a_n>0\equiv a_n\to 0+$
Bizonyítás:
$a_n\to 0+$
$\implies\forall\epsilon>0$-hoz $\exists N(\epsilon)$ hogy ha $n>N(\epsilon)$ akkor $0<a_n<\epsilon$
	$\implies\forall P\in\mathbb R$-re $\exists N_{\frac{1}{a_n}}(P)=N_a(\frac{1}{a_n})$ ha $n>N(P)$ akkor $\frac{1}{a_n}>P$

>[!warning] Tétel
>$(a_n\to 0\land a_n<0)\implies\frac{1}{a_n}\to-\infty$

$a_n\to 0\land a_n<0\equiv a_n\to 0-$
Bizonyítás:
$a_n\to 0-$
$\implies\forall\epsilon>0$-hoz $\exists N(\epsilon)$ hogy ha $n>N(\epsilon)$ akkor $-\epsilon<a_n<0$
	$\implies\forall P\in\mathbb R$-re $\exists N_{\frac{1}{a_n}}(P)=N_a(\frac{1}{a_n})$ ha $n>N(P)$ akkor $\frac{1}{a_n}<P$

>[!warning] Tétel
>Ha $a_n<b_n$ és $a_n\to A,$ $b_n\to B$, akkor $A\leq B$ 

Bizonyítás: indirekt
Tfh $B<A$
B és A között ekkor $A-B$ a távolság
legyen $\epsilon=\frac{A-B}{2}$ 
$\implies\exists N_a(\epsilon)$ és $\exists N_b(\epsilon)$ 
	ha $n>N_a(\epsilon)$ és $n>N_b(\epsilon)$
	$\implies$ $|a_n-A|<\epsilon$ és $|b_n-B|<\epsilon$
		$A-\epsilon<a_n$ és $b_n<B+\epsilon$
		$\implies b_n<a_n$ $\unicode{x21af}$

>[!warning] Tétel: **Rendőrelv**
>$a_n\leq c_n\leq b_n$ és $(a_n\to A)$ $(b_n\to A)\implies c_n\to A$

Bizonyítás:
$\forall\epsilon>0$-ra $\exists N_c(\epsilon)=\max(N_a(\epsilon), N_b(\epsilon))$
ha $n>N_c(\epsilon)\implies A-\epsilon<a_n$ és $b_n<A+\epsilon$
$\implies A-\epsilon<a_n\leq c_n\leq b_n<A+\epsilon$
	$\implies |c_n-A|<\epsilon$ 

>[!warning] Tétel: **Speciális rendőrelv**
>$a_n\leq b_n\forall n\in\mathbb N$
>* $a_n\to\infty\implies b_n\to\infty$ 
>* $a_n\to-\infty\implies b_n\to-\infty$ 

Bizonyítás:
$N_a(P)=N_b(P)$
$N_a(P)=N_b(P)$

>[!quote] Jelölés: $a_n>>b_n$ 
>$a_n$ sokkal jobban tart a végtelenbe, mint $b_n$ ha $\frac{b_n}{a_n}\to 0\iff\frac{a_n}{b_n}\to\infty$

>[!warning]- $n^n>>n!>>a^n>>n^k>>\log_an$, ahol $a>1$ és $k>0$
>
>Bizonyítás:
>Mutassuk meg, hogy
>1. $n^n>>n!$
>$0<\frac{n!}{n^n}=\frac{1\cdot2\cdot3\cdot ...\cdot n}{n\cdot n\cdot n...\cdot n}\leq\frac{1}{n}\to 0$, mivel $0\to0$ és $\frac{1}{n}\to 0$ a rendőrelv miatt $\frac{n!}{n^n}\to 0$
>  2. $n!>>a^n$
>$\frac{a^n}{n!}=\frac{a\cdot a\cdot a\cdot a\cdot ... \cdot a}{1\cdot 2\cdot ...\cdot n}=\frac{a^{[a]}}{[a]!}\cdot\frac{a}{K}\cdot\frac{a}{K+1}\cdot...\cdot\frac{a}{n},$ ahol $K>a$
>legyen $\frac{a}{K}=q<1$
>$\frac{a^{[a]}}{[a]!}\cdot\frac{a}{K}\cdot\frac{a}{K+1}\cdot...\cdot\frac{a}{n}<\frac{a^{[a]}}{[a]!}\cdot q^{n-K}\to 0$
>tehát $\frac{a^{[a]}}{[a]!}\cdot\frac{a}{K}\cdot\frac{a}{K+1}\cdot...\cdot\frac{a}{n}$ is tart 0-ba
>3. $a^n>>n^k$
>$b_n=\frac{n^k}{a^n}$
>$\frac{b_{n+1}}{b_n}=\frac{(n+1)^k\cdot a^n}{a^{n+1}\cdot n^k}=\frac{(n+1)^k}{n^k}\cdot\frac{1}{a}$
>$\frac{(n+1)^k}{n^k}\to 1$
>$\frac{1}{a}\to 1$
>$\frac{(n+1)^k}{n^k}\cdot\frac{1}{a}=q<1$ ha $n$ elég nagy $n>N_1$
>$b_{n+N_1}\leq b_{N_1}\cdot q$
>4. $n^k>>\log_an$
>$\frac{\log_an}{n^k}=\frac{\ln n}{\ln a\cdot n^k}=\frac{1}{\ln a}\cdot \frac{\ln n}{n^k}$
>az állítás miatt $\frac{\ln n}{n^k}\to 0$ tehát $\frac{\log_an}{n^k}\to 0$

>[!note] Állítás: $\frac{\ln n}{n^k}$ monoton csökken egy idő után
>Bizonyítás: 
>$(\frac{\ln x}{x^k})'=\frac{(\ln x)'\cdot x^k-\ln x\cdot (x^k)'}{(x^k)^2}=\frac{\frac{1}{x}\cdot x^k-\ln x\cdot k\cdot x^{k-1}}{x^{2k}}=\frac{x^{k-1}-\ln x\cdot k\cdot x^{k-1}}{x^{2k}}=\frac{x^{k-1}}{x^{2k}}\cdot(1-k\ln x)$
>$(1-k\ln x)=0$
>$(k\ln x)=1$
>$\ln x=\frac{1}{k}$
>$x=e^{\frac{1}{k}}$-tól monoton csökken

>[!danger] Néhány nevezetes számsorozat
>$$
>\lim\limits_{n\to\infty}a^n\begin{cases}
>0, \text{ ha } |a|<1 \\
>1,\text{ ha } a=1 \\
>\infty,\text{ ha } a>1 \\
>\text{oszcillálóan divergens egyébként}
>\end{cases}
>$$
>$$\sqrt[n]P\to 1$$
>$$\sqrt[n]n\to 1$$
Bizonyítás:
$\forall\epsilon>0$-ra
$(1-\epsilon)^n<P<(1+\epsilon)^n$ ha n elég nagy
$\implies 1-\epsilon<\sqrt[n]P<1+\epsilon$ tehát $\sqrt[n]P\to 1$
$\forall\epsilon>0$-ra
$(1-\epsilon)^n<n<(1+\epsilon)^n$ ha n elég nagy
$\implies 1-\epsilon<\sqrt[n]n<1+\epsilon$ tehát $\sqrt[n]n\to 1$

>[!warning]- $a_n\nearrow$ és felülről korlátos $\implies$ konvergens és $a_n\searrow$ és alulról korlátos $\implies$ konvergens
>Ha $a_n$ sorozat monoton nő és felülről korlátos, akkor $a_n$ konvergens
>Ha $a_n$ sorozat monoton csökken és alulról korlátos, akkor konvergens
>
Bizonyítás:
Tegyük fel, hogy $a_n$ monoton nő és korlátos
$A=\{a_n|n\in\mathbb N\}$ $\sup A=\lim\limits_{n\to\infty}a_n$
Tegyük fel, hogy $\lim\limits_{n\to\infty}a_n\neq\sup A=B$
$\lnot(\forall\varepsilon>0\text{-ra }\exists N(\varepsilon)\text{, hogy }n>N(\varepsilon)\implies |a_n-B|<\varepsilon)$
$\longrightarrow \exists\varepsilon>0\text{ melyre }\forall N\text{-ra } n>N\text{ és} |a_n-B|>\varepsilon$
Ekkor $B+\varepsilon<a_n\implies$ $B$ nem felső korlát
és $a_n<B-\varepsilon\implies$ $B-\varepsilon$ felső korlát azaz $B$ nem szuprénum
Ellentmondás, tehát a tétel igaz

>[!warning]- $(1+a_n)^{b_n}\to e^c$ 
> Tegyük fel, hogy $a_n\to0,$ $b_n\to\infty$ és $a_nb_n\to c$
> Ekkor $(1+a_n)^{b_n}\to e^c$ 
>> [!abstract] Megjegyzés: $(1+\frac{a}{n})^n\to e^a$
>ahol
>$a_n=\frac{a}{n}\to0$
>$b_n=n\to\infty$
>$a_nb_n\to a$
>
>Bizonyítás: Tegyük fel, hogy $L_n=(1+a_n)^{b_n}$
>$\ln(L_n)=\ln[(1+a_n)^{b_n}]=b_n\cdot\ln(1+a_n)$
>$\ln(1+x)=x-\frac{x^2}{2}+\frac{x^3}{3}-\frac{x^4}{4}...$ 
>>tehát $\ln(1+x)\approx x$
>>és $x-\frac{5}{6}x^2\leq\ln(1+x)\leq x$
>
>$b_n\to\infty$ és $a_n\to 0$ és $a_nb_n\to c$
>$\ln(L_n)=b_na_n\to c$
>$L_n\to e^c$ mivel $\ln$ és $e^x$ folytonos függvények

>[!warning]- Minden sorozatnak van monoton részsorozata
>
>Bizonyítás:
>"csúcs": $a_{n0}$ csúcs, ha $\forall n>n_0$-ra $a_n\leq a_{n0}$
>1. $\exists$ végtelen sok csúcs 
>>$\implies$ van monoton csökkenő részsorozat, hiszen ezek a csúcsok monoton csökkenő részsorozatot alkotnak
>2. véges sok csúcs van (esetleg 0)
>>$a_{s1}:$ a legnagyobb indexű csúcs után következő elem, tehát nem csúcs
>>$\exists s_2>s_1: a_{s_2}\geq a_{s1},$ különben $a_{s1}$ csúcs lenne
>>$\exists s_3>s_2: a_{s_3}\geq a_{s2},$ különben $a_{s2}$ csúcs lenne
>>Így tovább kapunk egy monoton növekvő részsorozatot

>[!warning]- [bolzano-weiestrass](./bolzano-weiestrass.md)
>Korlátos sorozatnak van konvergens részsorozata

## Cauchy sorozatok


>[!info] Definíció
>Egy $a_n$ sorozat Cauchy sorozat, ha $\forall\varepsilon>0$-hoz $\exists M(\varepsilon)$ ha $n,m>M(\varepsilon)$ akkor $|a_n-a_m|<\varepsilon$

>[!warning] $a_n\to A\iff a_n$ Cauchy sorozat, ha $\forall a_n\in\mathbb R$

>[!info] Definíció
>Azt a teret, ahol minden Cauchy sorozat konvergens [Hilbert-térnek](./hilbert-ter.md) nevezzük

## Környezet

>[!info] Definíció
>$A$ egy környezete:
>>$A\in\mathbb R\longrightarrow(A-\varepsilon;A+\varepsilon)$ intervallum
>>$A=\infty\longrightarrow(M,\infty)$ intervallum
>>$A=-\infty\longrightarrow(-\infty,M)$ intervallum

>[!info] Definíció
>A $t\in\mathbb R$ vagy $t=\infty$ vagy $t=-\infty$ torlódási pontja $a_n$ sorozatnak, ha $t$ minden környezetében $a_n$-nek végtelen sok eleme van

>[!info] Definíció
>$S$ a torlódási pontok halmaza $S\not\subset\mathbb R$
>$\lim\sup a_n=\overline{\lim}a_n=\sup(S)$
>$\lim\inf a_n=\underline{\lim}a_n=\inf(S)$

>[!abstract] Megjegyzés: $\exists\lim a_n\implies\overline{\lim}a_n=\underline{\lim}a_n=\lim a_n$

## Rekurzív sorozatok

 $a_{n+1}=f(a_n)$



