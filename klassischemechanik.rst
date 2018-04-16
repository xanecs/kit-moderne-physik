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