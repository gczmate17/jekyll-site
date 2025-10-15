---
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
tags: []
share: true
aliases:
  - halmazok
---
### Halmazalgebra

Def: $I$ alaphalmaz, $A, B \subseteq I$
$x\in (A\cap B) \equiv (x\in A)\land (x\in B)$
$x\in (A\cup B)\equiv (x\in A)\lor (x \in B)$
$x\in \overline A \equiv \lnot(x\in A)$
$A\subset B\equiv \forall x(x\in A \Rightarrow x\in B)$
$A\subseteq B \land B\subseteq A \Rightarrow A=B$

#### Tétel
Legyen $A,B,C \subset I$
1. Asszociativitás: 
$A\cap(B\cap C)=(A\cap B)\cap C$
$A\cup(B\cup C)=(A\cup B)\cup C$
2. Disztributivitás:
$A\cup(B\cap C)= (A\cup B)\cap (A\cup C)$
$A\cap(B\cup C)=(A\cap B)\cup (A\cap C)$
3. Egységelem, Zéruselem:
$A\cap I = A, A\cup I=I, A\cap \emptyset=\emptyset, A\cup \emptyset = A$
4. [de-morgan](./de-morgan.md)
$\overline{(A\cap B)}=\overline A\cup \overline B$
$\overline{(A\cup B)}=\overline A\cap \overline B$
5. Komplementer
$A\cup \overline A=I, A\cap \overline A= \emptyset$

### Halmazok elemszáma

Jelölés: $|A|$

$A\cup B$ elemszámát [logikai szitával](./logikai-szita.md) lehet kiszámolni