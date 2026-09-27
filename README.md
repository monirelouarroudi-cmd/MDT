# 📘 Séance — Perspective cavalière et sections planes

**Terminale · Spécialité Maths**

| | |
|---|---|
| ⏱️ **Durée** | 2 heures |
| 🔑 **Prérequis** | Vecteurs de l'espace, coplanarité, produit scalaire dans l'espace |
| 🎯 **Objectif** | Comprendre ce que conserve/trahit une perspective cavalière, construire une section plane d'un cube avec les 3 outils, utiliser un repère pour calculer des points de section |

---

## 📑 Sommaire

- [Déroulement des 2 heures](#-déroulement-des-2-heures)
- [Retour rapide](#-retour-rapide)
- [Cours](#-cours)
  - [1. La perspective cavalière](#1-la-perspective-cavalière)
  - [2. Ce que le dessin conserve / trahit](#2-ce-que-le-dessin-conserve--trahit)
  - [3. Construire une section plane : les 3 outils](#3-construire-une-section-plane--les-3-outils)
  - [4. Intersection d'une droite et d'un plan (sans repère)](#4-intersection-dune-droite-et-dun-plan-sans-repère)
- [Exercices](#-exercices)
- [Mini-évaluation finale](#-mini-évaluation-finale)
- [Bilan](#-bilan)
- [Notes pour le professeur](#-notes-pour-le-professeur)

---

## ⏳ Déroulement des 2 heures

| Temps | Activité |
|---|---|
| 0–10 min | Retour rapide (repère de l'espace, cube) |
| 10–30 min | Cours : perspective cavalière, ce qu'elle conserve/trahit |
| 30–50 min | Cours : construire une section plane (3 outils) |
| 50–60 min | Cours : intersection droite/plan sans repère |
| 60–75 min | 4 exercices faciles |
| 75–90 min | 4 exercices moyens |
| 90–103 min | 3 exercices difficiles |
| 103–113 min | 2 exercices de réflexion |
| 113–120 min | Mini-évaluation |

> 📌 Dans toute la fiche, sauf mention contraire : $ABCDEFGH$ est le cube d'arête $1$, muni du repère $(A;\vec{AB},\vec{AD},\vec{AE})$, avec $A(0;0;0)$, $B(1;0;0)$, $C(1;1;0)$, $D(0;1;0)$, $E(0;0;1)$, $F(1;0;1)$, $G(1;1;1)$, $H(0;1;1)$.

---

## 🔁 Retour rapide

<details>
<summary><b>Question 1</b> — Dans le cube $ABCDEFGH$ ci-dessus, donner les coordonnées de $C$ et de $H$.</summary>

$$C(1;1;0), \qquad H(0;1;1)$$
</details>

<details>
<summary><b>Question 2</b> — Comment reconnaît-on qu'un vecteur $\vec n$ est normal à un plan dirigé par $\vec u,\vec v$ ?</summary>

$\vec n\cdot\vec u = 0$ et $\vec n\cdot\vec v = 0$.
</details>

<details>
<summary><b>Question 3</b> — Que signifie « deux points sont dans une même face du cube » pour construire une section ?</summary>

Le segment qui les joint est alors un côté de la section (il est entièrement contenu dans cette face).
</details>

---

## 📚 Cours

### 1. La perspective cavalière

On choisit un **plan frontal** (parallèle à la feuille), un angle $\alpha$ et un coefficient de réduction $k$ (dans cette fiche : $\alpha=45°$, $k=0{,}5$).

- Les longueurs et angles du plan frontal sont dessinés **en vraie grandeur**.
- Les droites perpendiculaires au plan frontal (les **fuyantes**) sont dessinées selon des droites faisant un angle $\alpha$ avec l'horizontale, avec des longueurs multipliées par $k$.

**Formule.** Si $\overrightarrow{AM}=x\overrightarrow{AB}+y\overrightarrow{AD}+z\overrightarrow{AE}$ (avec $(AB,AE)$ dans le plan frontal et $AD$ la profondeur), alors $M$ est dessiné au point de coordonnées $2D$ :

$$\boxed{(x+cy\ ;\ z+cy)} \qquad \text{avec } c = k\cos\alpha$$

(ici $c=0{,}5\times\cos45°=\dfrac{\sqrt2}{4}\approx0{,}354$).

---

### 2. Ce que le dessin conserve / trahit

| Conservé | Trahi |
|---|---|
| Alignement, appartenance (un point d'une arête est dessiné sur cette arête) | Longueurs et angles hors du plan frontal |
| Parallélisme (deux droites parallèles restent parallèles sur le dessin) | Les intersections apparentes : deux segments qui se croisent sur le dessin ne se coupent pas forcément dans l'espace |
| Rapports de longueurs sur une même droite ou deux droites parallèles (milieu $\to$ milieu) | La réciproque du parallélisme : deux droites dessinées parallèles ne sont pas forcément parallèles dans l'espace |

> ⚠️ Une figure ne permet pas, à elle seule, de retrouver un point de l'espace : il faut savoir sur quelle arête, dans quel plan il se trouve.

---

### 3. Construire une section plane : les 3 outils

| Outil | Principe |
|---|---|
| **1** | Si deux points de $\mathcal P$ (le plan sécant) sont dans une même face, le segment qui les joint est un côté de la section |
| **2** | Deux faces parallèles sont coupées par $\mathcal P$ selon deux segments **parallèles** |
| **3** | Deux droites d'un même plan non parallèles se coupent : on peut prolonger un côté dans une face jusqu'à couper la droite d'une autre face, ce qui fournit un nouveau point |

**Méthode :**

1. Joindre les points donnés qui sont dans une même face.
2. Sur la face parallèle, tracer le parallèle au côté obtenu, si l'on y connaît déjà un point.
3. Sinon, prolonger un côté jusqu'à couper une arête (outil 3), et contrôler (au plus 6 côtés, côtés portés par des faces parallèles sont parallèles).

---

### 4. Intersection d'une droite et d'un plan (sans repère)

Pour déterminer $\mathcal D\cap\mathcal P$ sans repère :

1. Choisir un **plan auxiliaire** $\Omega$ contenant $\mathcal D$ (une face, ou un plan déjà tracé).
2. Déterminer la droite $\Delta=\Omega\cap\mathcal P$ (par un point commun connu et le **théorème du toit**).
3. Dans le plan $\Omega$, $\mathcal D$ et $\Delta$ se coupent en un point : c'est le point cherché (ou $\mathcal D$ est parallèle à $\mathcal P$ si $\Delta$ l'est).

> 💡 **Propriété utile.** Si une droite est incluse dans un plan $P_1$ parallèle à un plan $P_2$ (et n'est pas incluse dans $P_2$), alors elle est parallèle à $P_2$.

---

## ✏️ Exercices

### 🟢 Exercices faciles

<details>
<summary><b>Exercice 1</b> — Calculer les coordonnées dessinées (perspective cavalière, $\alpha=45°,k=0{,}5$) du point $C(1;1;0)$.</summary>

$c=\dfrac{\sqrt2}{4}\approx0{,}354$.

$$(x+cy\,;\,z+cy) = (1+0{,}354\,;\,0+0{,}354) = (1{,}354\,;\,0{,}354)$$
</details>

<details>
<summary><b>Exercice 2</b> — Calculer les coordonnées dessinées du point $D(0;1;0)$.</summary>

$$(0+0{,}354\,;\,0+0{,}354)=(0{,}354\,;\,0{,}354)$$
</details>

<details>
<summary><b>Exercice 3</b> — Sur le dessin, $[AH]$ est-il représenté en vraie grandeur ? Justifier.</summary>

$A(0;0;0)$, $H(0;1;1)$ : le segment $[AH]$ est dans la face $ADHE$ (le plan $x=0$), qui n'est **pas** le plan frontal (celui-ci est $ABFE$, le plan $y=0$). $[AH]$ a une composante en profondeur ($y=1$ pour $H$) : sa longueur dessinée n'est donc **pas** la vraie grandeur.
</details>

<details>
<summary><b>Exercice 4</b> — Citer un segment du cube dont la longueur ET l'angle sont fidèlement représentés sur le dessin. Justifier.</summary>

N'importe quel segment de la face frontale $ABFE$ (par exemple $[AB]$, $[AE]$ ou $[BF]$) : ces segments sont contenus dans le plan frontal, donc dessinés en vraie grandeur.
</details>

---

### 🟡 Exercices moyens

<details>
<summary><b>Exercice 5</b> — $I,J,K$ milieux respectifs de $[AB],[BC],[BF]$. Justifier que la section du cube par le plan $(IJK)$ est le triangle $IJK$.</summary>

$I\in[AB]$ et $J\in[BC]$ sont tous deux dans la face $ABCD$ : $[IJ]$ est un côté de la section (outil 1).

$J\in[BC]$ et $K\in[BF]$ sont tous deux dans la face $BCGF$ : $[JK]$ est un côté.

$K\in[BF]$ et $I\in[AB]$ sont tous deux dans la face $ABFE$ : $[KI]$ est un côté.

La section est donc directement le triangle $IJK$ (elle « coupe le coin » $B$).
</details>

<details>
<summary><b>Exercice 6</b> — Avec le repère, donner les coordonnées de $I,J,K$ (exercice précédent) et montrer que le triangle $IJK$ est équilatéral.</summary>

$I=(0{,}5;0;0)$, $J=(1;0{,}5;0)$, $K=(1;0;0{,}5)$.

$$\vec{IJ}=(0{,}5;0{,}5;0) \quad \|\vec{IJ}\|=\sqrt{0{,}25+0{,}25}=\frac{\sqrt2}2$$

$$\vec{JK}=(0;-0{,}5;0{,}5) \quad \|\vec{JK}\|=\frac{\sqrt2}2$$

$$\vec{KI}=(-0{,}5;0;-0{,}5) \quad \|\vec{KI}\|=\frac{\sqrt2}2$$

Les trois côtés sont égaux : le triangle $IJK$ est **équilatéral** de côté $\dfrac{\sqrt2}2$.
</details>

<details>
<summary><b>Exercice 7</b> — Calculer les coordonnées dessinées du centre $M$ de la face $ADHE$ (perspective cavalière, $\alpha=45°,k=0{,}5$).</summary>

$M=\left(0;\,0{,}5;\,0{,}5\right)$ (moyenne de $A,D,H,E$).

$$(x+cy\,;\,z+cy) = (0+0{,}354\times0{,}5\,;\,0{,}5+0{,}354\times0{,}5) = (0{,}177\,;\,0{,}677)$$
</details>

<details>
<summary><b>Exercice 8</b> — $I$ milieu de $[EF]$, $J$ milieu de $[HG]$. La droite $(IJ)$ est-elle parallèle au plan $(ABC)$ ? Justifier sans repère.</summary>

$(IJ)$ est incluse dans la face $EFGH$ (plan du dessus), qui est **parallèle** à la face $ABCD$ (plan de base) — ce sont deux faces opposées du cube.

Une droite incluse dans un plan parallèle à un autre plan (et non incluse dans ce second plan) est parallèle à ce plan. Donc $(IJ)$ est parallèle à $(ABC)$.
</details>

---

### 🟠 Exercices difficiles

<details>
<summary><b>Exercice 9</b> — $M$ milieu de $[AB]$, $N$ milieu de $[AD]$, $P$ le point de $[AE]$ tel que $AP=\frac13$. Justifier la construction de la section par $(MNP)$ et donner sa nature.</summary>

$M\in[AB]$ et $N\in[AD]$ sont tous deux dans la face $ABCD$ : $[MN]$ est un côté.

$N\in[AD]$ et $P\in[AE]$ sont tous deux dans la face $ADHE$ : $[NP]$ est un côté.

$P\in[AE]$ et $M\in[AB]$ sont tous deux dans la face $ABFE$ : $[PM]$ est un côté.

La section est donc le triangle $MNP$ (les trois points appartiennent chacun à deux des trois faces qui se rejoignent en $A$, aucune extension n'est nécessaire).
</details>

<details>
<summary><b>Exercice 10</b> — $I,J,K$ milieux de $[AB],[AD],[AE]$. On admet que le plan $(IJK)$ a pour vecteur normal $(1;1;1)$.<br>a. Retrouver l'équation cartésienne de $(IJK)$.<br>b. La diagonale $[AG]$ coupe $(IJK)$ en un point $M$. Déterminer $M$ et le rapport $AM/AG$.</summary>

**a.** $I=(0{,}5;0;0)$. Équation avec normal $(1;1;1)$ : $1(x-0{,}5)+1(y-0)+1(z-0)=0 \Longrightarrow x+y+z=0{,}5$.

Vérification : $J(0;0{,}5;0)$ : $0{,}5$ ✓. $K(0;0;0{,}5)$ : $0{,}5$ ✓.

**b.** $[AG]$ : $M=A+s(G-A)=(s;s;s)$ pour $s\in[0;1]$ (car $G=(1;1;1)$).

$$s+s+s=0{,}5 \Longrightarrow s=\frac16$$

$$M=\left(\frac16;\frac16;\frac16\right), \qquad \frac{AM}{AG}=s=\frac16$$
</details>

<details>
<summary><b>Exercice 11</b> — Avec $c=\dfrac{\sqrt2}4$, montrer que $M_1(c;0;c)$ et $M_2(0;1;0)$ ont le même dessin en perspective cavalière. Que peut-on en conclure ?</summary>

Dessin de $M_1(c;0;c)$ : $(c+c\times0\,;\,c+c\times0)=(c;c)$.

Dessin de $M_2(0;1;0)$ : $(0+c\times1\,;\,0+c\times1)=(c;c)$.

Les deux dessins sont identiques : $(c;c)$.

**Conclusion :** un dessin en perspective cavalière ne détermine pas de façon unique le point de l'espace représenté — il faut connaître, en plus, sur quelle arête ou dans quel plan se trouve le point.
</details>

---

### 🔴 Exercices de réflexion

<details>
<summary><b>Exercice 12</b> — Généraliser l'exercice 6 : montrer que dans un cube d'arête $a$ quelconque, la section passant par les milieux de trois arêtes concourantes en un même sommet est toujours un triangle équilatéral.</summary>

Plaçons l'origine au sommet commun (par symétrie du rôle des trois arêtes). Les milieux sont $I(\frac a2;0;0)$, $J(0;\frac a2;0)$, $K(0;0;\frac a2)$.

$$\vec{IJ}=\left(-\frac a2;\frac a2;0\right),\qquad \|\vec{IJ}\|=\frac a2\sqrt2$$

Par symétrie des rôles de $x,y,z$ (permutation circulaire), $\|\vec{JK}\|$ et $\|\vec{KI}\|$ valent aussi $\dfrac a2\sqrt2$.

Les trois côtés sont égaux quel que soit $a$ : la section est **toujours un triangle équilatéral**, de côté $\dfrac{a\sqrt2}2$.
</details>

<details>
<summary><b>Exercice 13</b> — En perspective cavalière ($c=k\cos\alpha$ quelconque), montrer que $M(x;y;z)$ et $M'(x';y';z')$ ont le même dessin si et seulement si $x-x'=z-z'=-c(y-y')$. En déduire une condition pour que deux points distincts soient confondus sur le dessin.</summary>

$\text{dessin}(M)=\text{dessin}(M') \Longleftrightarrow x+cy=x'+cy' \ \text{et}\ z+cy=z'+cy'$

$$\Longleftrightarrow x-x'=-c(y-y') \ \text{et}\ z-z'=-c(y-y')$$

Ces deux égalités entraînent en particulier $x-x'=z-z'$, et cette valeur commune doit valoir $-c(y-y')$.

**Conséquence :** si $y=y'$ (même profondeur), il faut $x=x'$ et $z=z'$, donc $M=M'$ — deux points de même profondeur distincts sont toujours distingués sur le dessin. L'ambiguïté n'apparaît que pour des points de profondeurs différentes ($y\neq y'$) vérifiant $x-x'=z-z'=-c(y-y')$.
</details>

---

## 📝 Mini-évaluation finale

<details>
<summary><b>A.</b> Citer les trois outils permettant de construire une section de cube.</summary>

1. Deux points d'une même face $\to$ le segment est un côté.
2. Deux faces parallèles $\to$ côtés parallèles.
3. Deux droites non parallèles d'un même plan se coupent (prolongement).
</details>

<details>
<summary><b>B.</b> Une droite incluse dans un plan parallèle à un plan $P_2$ (sans y être incluse) est-elle toujours parallèle à $P_2$ ?</summary>

Oui : ne pouvant jamais rencontrer $P_2$ (les deux plans ne se coupent pas), elle est parallèle à $P_2$.
</details>

<details>
<summary><b>C.</b> Donner le dessin du point $F(1;0;1)$ en perspective cavalière.</summary>

$y=0$ : $F$ est dans le plan frontal, dessiné en vraie grandeur : $(1;1)$.
</details>

<details>
<summary><b>D.</b> Qu'est-ce que la section plane d'un solide par un plan $\mathcal P$ ?</summary>

C'est l'intersection du solide et de $\mathcal P$ : un polygone dont chaque côté est l'intersection de $\mathcal P$ avec une face du solide.
</details>

---

## ✅ Bilan

### Les réflexes à retenir

1. Seul le plan frontal est représenté en vraie grandeur — toujours identifier ce plan avant de juger une longueur ou un angle sur un dessin.
2. Pour une section : chercher d'abord les points dans une même face (outil 1), puis les faces parallèles (outil 2), et prolonger seulement en dernier recours (outil 3).
3. Deux segments qui se croisent **sur le dessin** ne se coupent pas forcément dans l'espace.
4. « Sans repère » pour les arguments de parallélisme/incidence ; « avec repère » dès qu'il faut calculer un point ou un coefficient précis.

---

## 🧑‍🏫 Notes pour le professeur

- [ ] Distingue plan frontal / fuyantes, sait ce qui est en vraie grandeur
- [ ] Applique correctement les 3 outils de construction de section
- [ ] Justifie une section sans se contenter de « on relie les points »
- [ ] Sait passer d'un raisonnement géométrique à un calcul avec repère
- [ ] Comprend la propriété d'ambiguïté du dessin en perspective
- [ ] Erreurs surtout calculatoires
- [ ] Erreurs surtout méthodologiques / de justification
