---
tags:
  - mat
  - geometria
  - vektor
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
share: true
aliases:
  - tergeo
---
### Egyenes megadása

A $P_0=(x_0,y_0,z_0)$ kezdőpontú és $\bar{v}=(v_1,v_2,v_3)$ irányvektorral megadott egyenesen azok az $x,y,z$ pontok vannak, amik a 
$$\begin{array} xx=x_0+t\cdot v_1 \\ y= y_0 + t\cdot v_2 \\ z = z_0 +t\cdot v_3
\end{array}\iff \frac{x-x_0}{v_1}=\frac{y-y_0}{v_2}=\frac{z-z_0}{v_3}=t$$
egyenletrendszert kielégítik
### Sík megadása

$P$ pont rajta van a síkon, ha $\overline{P_0P}$ merőleges az $\bar{n}$ normálvektorra $\iff$ $\overline{P_0P}\cdot\bar{n}=0$ 

$(x-x_0,y-y_0,z-z_0)\cdot(n_1, n_2, n_3)=0$
$n_1(x-x_0)+n_2(y-y_0)+n_3(z-z_0)=0$
$n_1x+n_2y+n_3z=n_1x_0+n_2y_0+n_3z_0$

### Pontszorzat
(skalárszorzat, belső szorzat)

Jelölés: $\bar{a}\cdot\bar{b},\quad\bar{a}\bar{b},\quad(\bar{a},\bar{b}),\quad\langle\bar{a},\bar{b}\rangle$

$\bar{a}\cdot\bar{b}=\sum^n_{i=1}a_ib_i\quad$ ahol $n$ a dimenzió fokát jelöli

$|\bar{a}\cdot\bar{b}|=|\bar{a}||\bar{b}|\cdot\cos\theta\quad$ ahol $\theta$ $\bar{a}$ és $\bar{b}$ közbezárt szöge

>[!abstract] Megjegyzés 
>$\bar{a}$ és $\bar{b}$ merőleges $\iff\bar{a}\cdot\bar{b}=0$  

### Keresztszorzat
(vektoriális szorzat)

Jelölés: $\bar{a}\times\bar{b}$

$\bar{a}\times\bar{b}=\begin{bmatrix}i & j & k\\ a_1 & a_2 & a_3\\ b_1 & b_2 & b_3\end{bmatrix}=i(a_2b_3-b_3a_2)-j(a_1b_3-a_3b_1)+k(a_1b_2-a_2b_1)=i(a_2b_3-b_3a_2)+j(a_3b_1-a_1b_3)+k(a_1b_2-a_2b_1)$
$|\bar{a}\times\bar{b}|=|\bar{a}||\bar{b}|\sin\theta\quad$ ahol $\theta$ $\bar{a}$ és $\bar{b}$ közbezárt szöge

Az eredmény:
1. állása merőleges mind $\bar{a}$-ra mind $\bar{b}$-re 
2. iránya olyan, hogy $\bar{a},\bar{b},\bar{a}\times\bar{b}$ jobbsodrású rendszert alkot

>[!abstract] Megjegyzés
>Jobbsodrású rendszernek hívunk egy vektorrendszert, ha a jobbkezünket beállítjuk úgy, hogy hüvelykujjunk $\bar{a}$-val, mutatóujjunk $\bar{b}$-vel, középsőujjunk pedig $\bar{a}\times\bar{b}$-vel azonos irányba mutat

### Vegyesszorzat

Jelölés: $(\bar{a}\times\bar{b})\cdot \bar{c}$

$(\bar{a}\times\bar{b})\cdot \bar{c}=i(a_2b_3-b_3a_2)+j(a_3b_1-a_1b_3)+k(a_1b_2-a_2b_1)\cdot(c_1, c_2, c_3)=c_1(a_2b_3-b_3a_2)+c_2(a_3b_1-a_1b_3)+c_3(a_1b_2-a_2b_1)=$
$$\begin{bmatrix}c_1 & c_2 & c_3 \\ a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3\end{bmatrix}=\begin{bmatrix}a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \\ c_1 & c_2 & c_3\end{bmatrix}$$

A vegyesszorzat egy paralelepipedon térfogatát feszíti ki

### Vetítés

$\bar{b}$ vektor $\bar{a}$ vektorra vetítése: $$\bar{b}^{\bar{a}}=\frac{\bar{a}\cdot\bar{b}}{\Vert \bar{a}\Vert^2}\cdot \bar{a}$$
>[!abstract] Megjegyzés
>Ha $\bar{b}$ merőleges $\bar{a}$-ra $\implies\bar{b}^{\bar{a}}=$
