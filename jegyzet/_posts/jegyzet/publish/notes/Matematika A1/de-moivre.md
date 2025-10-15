---
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
tags: []
share: true
aliases:
  - de-moivre
---
Minden $x$ valós szám és minden $n$ egész szám esetén fenn áll
$$(\cos x+i\sin x)^n=\cos nx+i\sin nx$$
A tétel összeköti a komplex számokat a [trigonometriával](Trigonometria.md)
#### Bizonyítás [teljes indukcióval](./logika.md#Bizonyítási%20módszerek)

Ha n>0
1. $n=1$ esetén az állítás igaz
2. Tegyük fel, hogy tetszőleges $k\in \mathbb Z$ esetén is igaz
3. $n=k+1$ esetén:
$(\cos x+i\sin x)^{k+1}=(\cos x+i\sin x)^k(\cos x+i\sin x)=$ 
$= (\cos kx+i\sin kx)(\cos x+i\sin x)$ **az indukciós feltevés miatt**
$=\cos kx \cos x - \sin kx \sin x + \cos kx i\sin x + i\sin kx \cos x =$
$= \cos ((k+1)x)+i\sin ((k+1)x)$ **trigonometrikus azonosságok miatt**

Ha n=0
a képlet igaz, mivel $\cos 0x +i\sin 0x=1+i0=1$ és $(\cos x +i\sin x)^0=1$

Ha n<0
vegyük azt az $m\in \mathbb Z^+,$ amelyre $n=-m$
$(\cos x+i\sin x)^n=(\cos x +i\sin x)^{-m}={1\over(\cos x+i\sin x)^m}$
$={1\over(\cos mx+i\sin mx)}=\cos mx-i\sin mx$ **konjugáltal szorzunk**
$=\cos(-mx)+i\sin(-mx)=\cos nx +i\sin nx$

tehát a tétel $\forall n\in\mathbb Z$-re igaz
