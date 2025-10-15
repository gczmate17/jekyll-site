---
tags:
  - mat
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
share: true
aliases:
  - testek
---
Az algebrában a test egy olyan $F=(T;+,\cdot)$ kétműveletes algebrai [struktúrát](Matematikai%20strukt%C3%BAra.md) jelöl, ahol $T$ kommutatív csoportot alkot a $+$ műveletre nézve, a $\cdot$ kommutatív, asszociatív, minden nem nulla elemnek van inverze a $\cdot$ műveletre nézve, továbbá a $\cdot$ művelet disztributív a $+$ műveletre

Olyan algebrai struktúrákat, ahol a $\cdot$ nem feltétlen kommutatív, de a többi tulajdonság egyébként teljesül **ferdetest**nek nevezzük
### Példák

**Test**:
	$(\mathbb Q,\mathbb R,\mathbb C$) [racionális számok](Racion%C3%A1lis%20sz%C3%A1mok.md), [valós számok](./valos-szamok.md) és [komplex számok](./komplex-szamok.md)
**Ferdetest**:
	$\{a+bi+cj+dk|a,b,c,d\in\mathbb R\}$ [kvaterniók](./komplex-szamok.md#Kvaterniók)
### Test axiómák

* Az összeadás és szorzás művelet asszociatív
	$\forall a,b,c\in F:\quad a+(b+c)=(a+b)+c\quad\text{ és }\quad a\cdot(b\cdot c)=(a\cdot b)\cdot c$
* Az összeadás és szorzás művelet kommutatív
	$\forall a,b\in F:\quad a+b=b+a\quad\text{ és }\quad a\cdot b=b\cdot a$
* A szorzás disztributív az összeadásra nézve
	$\forall a,b,c\in F:\quad a\cdot(b+c)=a\cdot b + a\cdot c$
* Létezik nullelem, azaz olyan 0-val jelölt elem, hogy
	$\exists 0\in F:\quad \forall a\in F:\quad a+0=a$
* Létezik egységelem, azaz olyan 1-gyel jelölt elem, hogy
	$\exists 1\in F:\quad\forall a\in F:\quad a\cdot 1=a$
* Léteznek additív inverz elemek másnéven ellentettek
	$\forall a\in F:\quad \exists -a\in F:\quad a+(-a)=0$
* Léteznek multiplikatív inverzek másnéven reciprokok
	$\forall a\neq 0\in F:\quad \exists a^{-1}\in F:\quad a\cdot a^{-1}=1$

### Résztest

Ha az elemek egy részhalmaza is testet alkot az $F$-beli műveletekkel, beleértve, hogy tartalmazza a 0-t és 1-et, akkor beszélhetünk a részhalmaz elemei által alkotott **résztest**ről

Jelölhető $K\subset F$-ként vagy, ha egy nagyobb testet egy kisebb test bővítéseként tekintünk, akkor $F|K$ vagy $F/K$

Egy $F$ test tetszőleges számú résztestének metszete is résztest, így kimondhajtuk a $T$ egy $A$ részhalmazának generált résztestét.
Ez jellemezhető kívülről: az összes $A$-t tartalmazó résztest metszete
és belülről: $A$-ból, 0-ból és 1-ből a testműveletekkel megkapható az összes $F$-beli elem által alkotott részhalmaz, ami résztest

A bővebb $F$ test a $K$ fölött [lineáris teret](Vektort%C3%A9r.md) alkot a testműveletekkel
A testbővítés fokának nevezzük ennek a vektortérnek a dimenzióját

Az $F$ bővebb test egy elem *algebrai* $K$ felett, ha gyöke egy nem konstans nulla $K$-beli együtthatós [polinom](./polinomok.md); különben *transzcendens*
	Például $\pi$ transzcendens a racionális számok teste felett 
### Prímtest

Bármely testnek van minimális részteste $\to$ **prímtest**
véges $p$ karakterisztika esetén a prímtest az $F_p$  $p$ elemű véges testtel izomorf, 0 karakterisztika esetén pedig a racionális számok testével izomorf

### Véges testek

Minden véges ferdetest test: [Wedderburn-tétel](Wedderburn-t%C3%A9tel.md)

