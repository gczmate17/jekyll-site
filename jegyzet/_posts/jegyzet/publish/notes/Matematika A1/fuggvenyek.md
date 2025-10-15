---
tags:
  - mat
  - analizis
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
share: true
aliases:
  - fuggvenyek
---

>[!info] Definíció
Ha az R [reláció](./relacio.md) olyan, hogy $\forall x\in X((x,y)\in R)\land (((x,z)\in R)\Rightarrow y = z)$, akkor R függvény.

$Dom(f)\to Domain(f)$
$Ran(f)\to Range(f)$

Az $F\subset X\times Y$
* Szürjektív: ${\forall y\in Y}\land {\exists x\in X}\land (x,y)\in F \Rightarrow F(x)=y$
* Injektív: $\forall x,y\in X\land x\neq z \Rightarrow F(x)\neq F(z)$ 
* Bijektív: ha F szürjektív és bijektív

### Függvény tulajdonságok

>[!info] Korlátosság
>
>$f$ felülről korlátos, ha $\exists K\in\mathbb R$, amire $f(x)\leq K\quad(x\in D_f)$ vagy $R_f\subset(-\infty,K]$
>
>$f$ alulról korlátos, ha $\exists K\in\mathbb R$, amire $f(x)\geq K\quad(x\in D_f)$ vagy $R_f\subset(-\infty,K]$
>
>$f$ korlátos, ha alulról és felülről is korlátos, azaz $\exists K\in\mathbb R,$ amire $|f(x)|\leq K,$ vagy $R_f\subset[-K,K]$

>[!info] Monotonitás
>$f$ monoton nő, ha $\forall(x_1,x_2)\in D_f$-re ahol $x_1\leq x_2\implies f(x_1)\leq f(x_2)$
>$f$ szigorúan monoton nő, ha $\forall(x_1,x_2)\in D_f$-re ahol $x_1< x_2\implies f(x_1)< f(x_2)$ 
>
>$f$ monoton csökken, ha $\forall(x_1,x_2)\in D_f$-re ahol $x_1\geq x_2\implies f(x_1)\geq f(x_2)$
>$f$ szigorúan monoton nő, ha $\forall(x_1,x_2)\in D_f$-re ahol $x_1> x_2\implies f(x_1)>f(x_2)$ 

>[!info] Paritás
>$f$ páros, ha $x\in D_f\implies -x\in D_f$ és $f(-x)=f(x)$
>$f$ páratlan, ha $x\in D_f\implies -x\in D_f$ és $f(-x)=-f(x)$

>[!info] Periodikusság
>$f$ periodikus $p>0$ periodussal, ha $f(x+p)=f(x),\quad x\in D_f\implies(x+p)\in D_f$
>


