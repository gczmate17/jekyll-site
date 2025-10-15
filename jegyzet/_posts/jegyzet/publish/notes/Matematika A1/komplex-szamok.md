---
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
tags: []
share: true
aliases:
  - komplex-szamok
---
### Komplex számok algebrai alakja
$$z=a+bi$$
ahol $a, b\in \mathbb R$ és $i^2=-1$

$a$-t hívjuk a komplex szám valós részének míg $b$-t a komplex szám képzetes részének
$Re z=a$
$Imz=b$

Komplex számok halmaza: $\mathbb C$

Geometriai reprezentáció: $xy$ sík $P(a,b)$ pontja és a P pontba mutató $\vec{OP}=\vec r$ vektor
$\vec r=a\vec i+b\vec j$

``` tikz
\begin{document}
\begin{tikzpicture}[scale=3.5,>=stealth]
  % Tengelyek
  \draw[->] (-0.5,0) -- (1.5,0) node[right] {Valós tengely};
  \draw[->] (0,-0.5) -- (0,1.5) node[above] {Képzetes tengely};

  % Pont és vektor
  \coordinate (O) at (0,0);
  \coordinate (P) at (1,1);

  % Vektor
  \draw[->, thick, black] (O) -- (P) node[midway, sloped, above] {$\vec{r} = a\vec{i} + b\vec{j}$};
  
   \draw[->, thick] (0.5,0) arc[start angle=0, end angle=45, radius=0.5cm];
  \node at (0.6,0.15) {\(\theta\)};

  % Pont
  \filldraw[black] (P) circle (0.5pt) node[above right] {$P(a,b)$};
  \filldraw[black] (O) circle (0.5pt) node[above left] {$O$};
   \draw[dashed] (P) -- (1,0) node[below] {$a$};
  \draw[dashed] (P) -- (0,1) node[left] {$b$};
\end{tikzpicture}
\end{document}
```
$z\in \mathbb C$ komplex számnak konjugáltja $\overline z,$ ahol $\overline z=a-bi$

$z$ konjugáltja az x-tengelyre vett tükörképe
#### Műveletek komplex számokkal

##### Összeadás, kivonás
A valós és képzetes részekkel külön-külön elvégezzük az összeadást (kivonást)
$$z_1\pm z_2=(a_1+b_1i)\pm(a_2+b_2i)=a_1\pm a_2 + (b_1\pm b_2)i$$
##### Szorzás
Minden tagot minden taggal összeszorzunk
$$z_1\cdot z_2=(a_1+b_1i)(a_2+b_2i)=a_1a_2-b_1b_2+(a_1b_2+a_2b_1)i$$
Következmény: $z\cdot \overline z= a^2-b^2i^2=a^2+b^2=|z|^2$
Tehát $|z|=\sqrt{z\cdot \overline z}$
##### Osztás
Mindig bővítünk a nevező konjugáltjával
$${z_1\over z_2}={a_1+b_1i\over a_2+b_2i}={(a_1+b_1i)(a_2-b_2i)\over (a_2+b_2i)(a_2-b_2i)}$$
### Komplex számok trigonometrikus alakja

Az $xy$ síkon ábrázolt $\vec r$ vektor $\theta$ szöget zár be az x-tengellyel 
E két adat egyértelműen meghatároz egy $P(a,b)$ pontot a komplex számsíkban

Ekkor
$\cos\theta = {a\over r}, \sin\theta={b\over r},$ ahol $r=\sqrt{a^2+b^2}$
$\rightarrow a=r\cdot\cos\theta, b=r\cdot\sin\theta$

Az algebrai alakból kiindulva
$z=a+bi=r\cos\theta + ir\sin\theta$ $$z=r(\cos\theta+i\sin\theta)$$
ahol $r\geq 0$ az abszolút érték, $\theta \in [0,2\pi)$ a szögtartomány

#### Műveletek trigonometrikus alakban
##### Szorzás
$$z_1\cdot z_2= r_1r_2(\cos({\theta_1+\theta_2})+i\sin({\theta_1+\theta_2}))$$
tehát a szorzás egy nyújtva forgatást jelent a síkban 
##### Osztás
$$z_1\cdot z_2= {r_1\over r_2}(\cos({\theta_1-\theta_2})+i\sin({\theta_1-\theta_2}))$$
##### Hatványozás
$$z^n=r^n(\cos{(n\theta)}+i\sin{(n\theta)})$$
$r=1$ esetén $(cos\theta+sin\theta)^n=\cos(n\theta)+\sin(n\theta)$
[de-moivre](./de-moivre.md)
##### Gyökvonás
$$\sqrt[n]z=\sqrt[n]r(\cos{\theta+2k\pi\over n}+\sin{\theta+2k\pi\over n})$$
ahol $k=1,2,3,....,n-1$
a gyökvonás nem függvény hanem [reláció](./relacio.md) és a gyökök a síkon egy szabályos n-szöget alkotnak
### Komplex számok exponenciális alakja
$$z=r\cdot e^{i\theta}$$
Következmény: $e^{i\theta}=(\cos\theta+i\sin\theta)$
Euler formula
$e^{i\pi}=(\cos\pi+i\sin\pi)=-1$
##### Szorzás
$z_1\cdot z_2=r_1r_2\cdot e^{i(\theta_1+\theta_2)}$
### Taylor sorok

Koszinusz:
$$\cos\alpha = \sum_{K=0}^\infty {\alpha^{2K}\over {2K!}}(-1)^K$$
Szinusz: $$\sin\alpha=\sum_{K=0}^\infty{\alpha^{2K+1}\over (2K+1)!}(-1)^K$$
e$^x$: $$e^x=\sum_{K=0}^\infty {x^K\over K!}$$
### Komplex számok általánosítása

#### Kvaterniók

Def: A kvaterniók a komplex számok négy dimenzióra történő nem kommutatív kiterjesztései

$i^2=j^2=k^2=-1$

| $ij=k$ | $ji=-k$ |
| ------ | ------- |
| $jk=i$ | $kj=-i$ |
| $ki=j$ | $ik=-j$ |
Minden kvaternió felírható a báziskvaterniók lineáris kombinációjaként
$$a+bi+cj+dk$$ ahol $a, b, c, d\in \mathbb R$

Halmazelméleti szempontból a kvaterniók a komplex számok önmagukkal vett [direkt szorzata](./descartes-szorzat.md)
### Algebra alaptétele

Minden n-ed fokú valós együtthatós [polinomnak](./polinomok.md) multiplicitásokkal együtt pontosan n darab gyöke van