Klassische Mechanik
===================

Abriss der Newtonschen Mechanik
-------------------------------

**Problemstellung** der Mechanik:

Orte :math:`\vec{r_i}` und Geschwindigkeiten :math:`\vec{v_i}`
zur Zeit :math:`t_0` gegeben für ein System von Massepunkten,
:math:`1 \le i \le N`

Es wirken Kräfte :math:`\vec{F_j}` auf die Massepunkte und ggf.
Kräfte :math:`\vec{F_{ij}}` zwischen den Massepunkten.

Wie lauten die **kinematischen Größen** :math:`\vec{r_i}(t)`
und :math:`\vec{v_i}(t) = \dot{\vec{r_i}}(t)` für beliebige
Zeiten :math:`t` danach?

Die kinematischen Größen :math:`\vec{r_i}(t)` und :math:`(\dot{\vec{r_i}}, \ddot{\vec{r_i}}, ...)`
werden als Lösungen gewöhnlicher Differentialgleichungen gefunden,
das sind die **Bewegungsgleichungen**.

.. sidebar:: Notation

    .. math::
        \dot{\vec{r_i}} = \frac{d}{dt}\vec{r_i}

        (\frac{dx_i}{dt}, \frac{dy_i}{dt}, \frac{dz_i}{dt})


Neben den Kinemstischen Größen gibt es die wichtigen Begriffe
**Kraft**, **Masse**, **Impuls**

Kraft: Vektorielle Größe :math:`\vec{F}`

Ursache der Bewegung oder: Änderung des Bewegungszustandes.

:math:`\leadsto` Kräftefrei :math:`\rightarrow` Bewegung unverändert.

:math:`\rightarrow` **Newtonsche Gesetze**

lex prima: Galileisches Trägheitsgesetz
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Es gibt **Inertialsysteme**, in denen ein kräftefreier Körper
(= Massepunkt) ruht, oder sich gradlinig, gleichförmig bewegt.

**Definition:** Jeder Massepunkt setzt der Einwirkung von
Kräften einen Trägheitswiderstand entgegen. = träge Masse (:math:m)

Damit Impuls :math:`\vec{p}=m\vec{v}`

lex secunda: Bewegungsgesetz
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. math::
    \dot{\vec{p}} = \vec{F}

Meist :math:`m` unveränderlich

.. math::
    \dot{\vec{v}} = \frac{d}{dt}\vec{v} &= \vec{a} & \mathrm{(Beschleunigung)}

    m\vec{a} &= \vec{F}

lex tertia: Actio = Reactio
~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. math::
    \vec{F_{ij}} = - \vec{F_{ji}}

:math:`\rightarrow` Festlegung der trägen Masse unabhängig von
der Kraft

.. figure:: figure001.svg

Spannen, loslassen :math:`\Rightarrow \vec{v_1},\vec{v_2}`

:math:`\Rightarrow` Verhältnis der Geschwindigkeiten

.. math::
    {\lvert}\vec{v_i}{\rvert} &= v_i

    \frac{v_1}{v_2} &= k(\frac{m_1}{m_2})

hängt nicht von Kraft oder Feder ab.

:math:`\rightarrow` Definition Masse als **Basiseinheit**

Wichtige Beispiele für Kräfte
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Gravitationskraft**

schwere Masse = träge Masse

:math:`\vec{r}` Ort von :math:`m` im System mit :math:`M` im Ursprung.

.. math::
    \vec{F} &= - \gamma \frac{Mm}{r^2}\hat{r}

    \hat{r} &= \frac{\vec{r}}{{\lvert}r{\rvert}}

Speziell auf der Erdoberfläche

.. math::
    r &= r_e \approx 6000\mathrm{km}

    M &= M_e

    \gamma &= \text{bekannt (Newtonsche Gravitationskonstante)}

    &\Rightarrow \vec{F} = \underbrace{(\gamma\frac{M}{r^2})}_{=g=9.81\mathrm{ms}^{-2}\approx 10\mathrm{ms}^{-2}}m


**Coulombkraft**

.. math::
    \vec{F} = \frac{1}{4\pi\varepsilon_0}\frac{q_1 q_2}{r^2}\hat{r}

mit Ladungen :math:`q_1` und :math:`q_2`


(beides Zentralkräfte)

**Lorentzkraft**

Kraft auf geladene Teilchen (Ladung :math:`e`) im elektromagnetischen Feld.

:math:`\vec{E}`: elektrisches Feld,
:math:`\vec{B}`: magnetisches Feld

.. math::
    \vec{F} &= e(\vec{E}+\vec{V}\times\vec{B})

    (\vec{F} &= m\vec{a} = m \ddot{\vec{r}} = e(\vec{E}+\ddot{\vec{r}}\times\vec{B}))

**harmonischer Oszillator**

lineare, stets negative Kraft

.. math::
    F = - \alpha{\lvert}x{\rvert}<0

:math:`\Rightarrow` Schwingung um Ruhelage

wichtiges math. Beispiel für gebundene Systeme.

Inertialsysteme, Nichtinertialsysteme
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Im Inertialsystem:

    Kräftefrei = gleichförmige, gradlinige Bewegung

Systeme :math:`\Sigma`, :math:`\Sigma^\prime` vollkommen gleichwertig,
d.H. physikalische Gesetze sind **kovariant** unter
Galilei-Transformationen:

.. math::
    \vec{r}^\prime = \vec{r}+\vec{v_0}t

also wenn sich :math:`\Sigma`, :math:`\Sigma^\prime` mit :math:`\vec{v_0}`
realtiv zueinander bewegen.

(Galilei-Invarianz)

Später :math:`\rightarrow` Lorentz-Invarianz (SRT)

In **beschleunigten Bezugssystemen** gibt es zusätzlich
sogenannte Scheinkräfte. z.B. Zentrifugalkraft, Corioliskraft.

**Weitere spezielle Themen**:

- Schwingung, mit Dämpfung
- Mehrere Massepunkte, Eigenschwingungen
- starre Körper
    :math:`\rightarrow` Bewegung von Schwerpunkt und Rotation (Kreiselbewegung)


Lagrange-Mechanik
-----------------

Ausgangspunkt: Newton

.. math::
    m\ddot{\vec{r}} = \vec{F_i} + \sum^{N}_{i\ne j}\vec{F_{ij}} \text{ mit } i = 1,...,N

:math:`\vec{F_i}`: externe Kräfte auf Massepunkt :math:`i`.

:math:`\vec{F_{ij}}`: interne Kräfte der beteiligten Teilchen, paarweise.

:math:`\rightarrow` Problem vollständig formuliert:

    :math:`3N` gewöhnliche Differentialgleichungen 2. Ordnung
    
    Lösbar mit entsprechenden Anfangsbedingungen

**Probleme**

- Formulierung in Koordinaten :math:`(X, Y, Z)` meist zu kompliziert.
- Meist Probleme mit stark eingeschränlter Geometrie, z.B. Perle auf Kreisförmigem Draht

    :math:`\rightarrow` die :math:`\vec{F_{ij}}` beschreiben geometrische, fest
    vorgegebene Beziehungen auf zu komplizierte Weise.

    :math:`\rightarrow` **Zwangskräfte**
    (z.B. zwischen Perle und Draht) bewirken **Zwangsbedingungen**
    ("Perle bleibt auf Draht"), die oft direkt *viel einfacher*
    zu Formulieren sind.

:math:`\rightarrow` Ziel der Lagrange-Mechanik:
Elimination der Zwangskräfte,
gelingt durch **verallgemeinerte Koordinaten**
(immer weniger als ursprünglich).

Dazu verschiedene Zwangsbedingungen unterscheiden:

**holonom**

.. math:
    f_\nu(\vec{r_i},t)=0 & \nu = 1,...,p

..

    **holonom-skleronom**

    .. math::
        \frac{\partial f_\nu}{\partial t} = 0 \text{ mit } \nu = 1,...,p
    
    Keine Zeitabhängigkeit

    **holonom-rheonom**

    .. math::
        \frac{\partial f_\nu}{\partial t} \ne 0

**nicht-holonom**

sonst

    **als Ungleichungen**

    :math:`\rightarrow` Keine eliminierbaren Bedingungen

    **differential, aber nicht integrierbar**

    z.B. mit Geschwindigkeiten


**Beispiele**

*holonom-skleronom:* 

Hantel

.. math::
    (X_1-X_2)^2+(Y_1-Y_2)^2+(Z_1-Z_2)^2-l^2=0

Teilchen auf Kugel

.. math::
    X^2+Y^2+Z^2-R^2=0

*holonom-rheonom*

.. math::
    \frac{Z}{X} &=\tan \varphi = \tan \varphi(t)

    f(X,Z,t) &= \frac{Z}{X}-\tan \varphi(t)=0