---
title: "{{title}}"
date:
  "{ date:YYYY-MM-DD }":
tags: []
share: true
aliases:
  - logika
---

>[!info] Definíció
>Állításoknak nevezzük azokat a kijelentéseket, melyek igazak vagy hamisak. ([Logikai érték](Logikai%20%C3%A9rt%C3%A9k.md))

#### Logikai műveletek

* konjunkció $\land$
* diszjunkció $\lor$
* negáció $\lnot$  
* implikáció $\Rightarrow$
* ekvivalencia $\Leftrightarrow$

#### Tétel

* Asszociativitás
* Disztributivitás
* Elnyelés
* [de-morgan](./de-morgan.md)

Def: [Logikai függvény](Logikai%20f%C3%BCggv%C3%A9ny.md)nek nevezzük azokat az állításokat, amelyek változókat tartalmaznak, és az igazságtartalmuk attól függ, hogy mit helyettesítünk be.

* univerzális kvantor: $\forall$
* egzisztenciális kvantor: $\exists$

#### Bizonyítási módszerek

1. Bizonyítás lánckövetkeztetéssel: $(P\Rightarrow Q)\land (Q\Rightarrow R)\Rightarrow (P\Rightarrow R)$
2. Bizonyítás kontrapozícióval: $(P\Rightarrow Q)\equiv (\lnot Q \Rightarrow \lnot P)$
3. Indirekt bizonyítás: $(\lnot P\Rightarrow Q)\land (\lnot P \Rightarrow \lnot Q)\Rightarrow P$
4. Teljes indukció: $A(1) \land (A(n)\Rightarrow A(n+1))\Rightarrow (\forall n)\Rightarrow A(n)(\forall n)$ 