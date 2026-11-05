# Megaresumen — Física 1 (examen dic 2026)

Este resumen tiene solo lo que hace falta para aprobar. Sale de 32 exámenes finales (feb 2016 → feb 2026, 320 ejercicios; detalle en [ANALISIS.md](ANALISIS.md)) cruzados con los temas del curso y el Resnick (`teorico/`).

**Cómo leerlo.** Cada tema arranca desde cero:
1. **La idea**, la intuición.
2. **Un ejemplo resuelto** de un examen real, con la respuesta verificada contra la clave oficial.
3. **Qué preguntan**, con las fórmulas, cómo se resuelve y las trampas.
4. **Ejercicios para practicar.**

Las soluciones de 2017 a 2021 están en `examenes/resumen_examenes_resueltos_2017-2021.pdf`.

**Cómo citar ejercicios.** `F` = febrero, `J` = julio (incluye ago 2024), `D` = diciembre, `A20a`/`A20b` = los dos turnos de agosto 2020. El número final es el ejercicio. Ejemplo: `D23-8` es el ejercicio 8 de diciembre 2023. En `F26`, a partir del ejercicio 4 el número es la posición en el examen (el PDF repite el número 3).

---

## 0. Reglas del juego

- 10 preguntas múltiple opción, 5 opciones, de 3 a 3,5 h (unos 20 min por pregunta).
- **Aprobación (desde jul 2025):** 6 bien y como máximo 2 mal, o 7 bien sin importar las mal. Las respuestas en blanco no restan. Hasta feb 2025 se aprobaba con 50/100 y cada respuesta mal restaba hasta 2,5 puntos.
- **El examen te da:** $g = 9{,}8$ m/s² y casi siempre los momentos de inercia de disco, barra, esfera y aro. No hace falta memorizarlos; sí hace falta saber usar **Steiner**.
- **Todos los ejercicios se pueden resolver por separado.** Cuando hay un par ("considere el mismo sistema..."), el segundo suele ser una pregunta conceptual.

### Estrategia

1. **Meta: 7 bien seguras.** Con eso apruebo aunque marque mal las dudosas.
2. **Primera pasada por las fáciles:** ej. 1–4 (cinemática y Newton) y ej. 10 (oscilaciones, casi siempre una fórmula).
3. **Segunda pasada por el rígido:** ej. 6–9.
4. **Con la regla nueva, la respuesta dudosa conviene dejarla en blanco** si ya tengo 2 marcadas con duda. Las opciones sirven para descartar: revisar unidades, casos límite ($\mu = 0$, $\theta = 0$, $m \to 0$) y signos.

### Qué suele haber en cada posición del examen

| Ej. | Tema más frecuente | |
|---|---|---|
| 1 | Tiro / MRUA (T2) | 23 de 32 |
| 2 | Movimiento relativo (T3) | |
| 3–4 | Newton con poleas y rozamiento (T4) | |
| 5–6 | Choques (T8), energía (T7), equilibrio (T12) | |
| 7 | Dinámica del rígido (T10) | |
| 8–9 | Momento angular (T11), rígido (T10) | |
| 10 | Oscilaciones (T13) | 18 de 32 |

---

## 1. Prioridades

| Prioridad | Tema | Por examen | Resnick | Qué estudiar |
|---|---|---|---|---|
| ★★★ | **T10** Dinámica del rígido | 1,3 | 12-1 a 12-6 | todo lo de la §10 |
| ★★★ | **T4** Newton, poleas, rozamiento | 1,2 | 5-7, 5-10, 5-11, 6-1, 6-2 | todo lo de la §4 |
| ★★★ | **T11** Momento angular | 1,1 (30/32 exámenes) | **13**-1 a 13-4 | todo lo de la §11 |
| ★★★ | **T13** Oscilaciones | 1,0 (29/32) | 15-1 a 15-6 | todo lo de la §13 |
| ★★★ | **T2** Cinemática, tiro | 1,0 (1,25 desde 2022) | 2-1 a 2-7, 4-1 a 4-3 | todo lo de la §2 |
| ★★ | **T8** Choques y centro de masa | 1,0 (0,67 desde 2022) | 9-1 a 9-6, 10-1 a 10-5 | todo lo de la §8 |
| ★★ | **T12** Equilibrio | 0,8 (1,0 desde 2022) | **14**-1 a 14-3 | todo lo de la §12 |
| ★★ | **T7** Energía | 0,9 | 8-3, 8-4, 8-6 | todo lo de la §7 |
| ★★ | **T3** Movimiento relativo, MCU | 0,7 (1,1 desde 2022) | 4-4 a 4-6 | todo lo de la §3 |
| ★ | **T5** Dinámica circular | 0,4 | 6-3 | 3 fórmulas |
| ★ | **T6** Trabajo y potencia | 0,4 | 7-4, 7-5, 8-1, 8-2 | 2 fórmulas |
| ★ | **T9** Cinemática del rígido, I | 0,2 | 11-1 a 11-5, 12-3 | Steiner + rodadura |
| — | T1 Vectores | 0 | — | solo como herramienta |

> Los `summary.md` de los temas 11 y 12 tienen mal el capítulo. En este Resnick el **cap. 13 es momento angular** y el **cap. 14 es equilibrio**.

**No estudiar** (no aparecen en 32 exámenes): patrones y unidades (1-1 a 1-5), masa variable (9-8), marco del CM (10-6), trompo y precesión (13-5, 13-6), elasticidad (14-5), estabilidad del equilibrio (14-4), oscilaciones amortiguadas y forzadas (15-8, 15-9), combinación de MAS (15-7).

---

## 2. Cinemática de la partícula (T2) ★★★

**La idea**
- Cinemática es describir el movimiento sin preguntarse qué lo causa. La única regla es que $a = dv/dt$ y $v = dx/dt$.
- Si la aceleración es constante, salen las fórmulas del MRUA.
- Un tiro oblicuo son **dos movimientos independientes** que comparten el tiempo $t$:
  - en $x$, velocidad constante (no hay nada que empuje de costado);
  - en $y$, MRUA con $a = -g$.
- Todo problema de tiro se resuelve igual: escribir $x(t)$ e $y(t)$, traducir la condición del enunciado ("pasa por tal punto", "se encuentran") a ecuaciones y despejar.

**Ejemplo resuelto — D22-1.** Un proyectil sale desde una plataforma de $h = 4{,}9$ m con $v_0 = 19{,}6$ m/s a $60°$. ¿Con qué ángulo llega al suelo?
1. Componentes iniciales: $v_x = 19{,}6\cos60° = 9{,}8$ m/s, que no cambia nunca. $v_{y0} = 19{,}6\sin60° = 16{,}97$ m/s.
2. No hace falta el tiempo. Usar $v_y^2 = v_{y0}^2 + 2a\Delta y$ con $\Delta y = -4{,}9$ y $a = -9{,}8$: $v_y^2 = 288 + 96 = 384 \Rightarrow v_y = -19{,}6$ m/s (baja).
3. $\tan\theta_f = |v_y|/v_x = 19{,}6/9{,}8 = 2 \Rightarrow \theta_f = 63°$. Respuesta **e** ✔.

**Qué preguntan**
- **Tiro oblicuo con una condición geométrica:** pasar un obstáculo o un aro (F16-1, J17-1, D21-1, D25-1), caer en un plano inclinado (D16-1), caer desde una altura (F20-1, D22-1, J24-2).
- **Encuentro de dos móviles:** proyectil con caída libre (J21-7, J23-2, D23-1, J24-1), pelota con corredor o carrito (D19-1, F24-1, D24-2, F25-2).
- **MRUA por tramos:** carreras (J22-1, J23-1, D24-1), rebotes (F25-1).
- **Tres proyectiles con la misma $v_0$ que llegan al mismo blanco** (F26-3): por energía, todos llegan con la misma rapidez.

**Fórmulas**
$$x = x_0 + v_{0}\cos\theta\, t \qquad y = y_0 + v_0\sin\theta\, t - \tfrac12 g t^2$$
$$y(x) = x\tan\theta - \frac{g\,x^2}{2v_0^2\cos^2\theta} \quad (\text{usar } 1/\cos^2 = 1+\tan^2 \text{ para despejar } \theta)$$
$$\text{Mismo nivel:}\quad R = \frac{v_0^2\sin 2\theta}{g},\quad H = \frac{v_0^2\sin^2\theta}{2g},\quad t_v = \frac{2v_0\sin\theta}{g}$$
$$v^2 = v_0^2 + 2a\,\Delta x \qquad \text{alcance máximo en } 45°:\ R_{max} = v_0^2/g$$

**Cómo se resuelve**
1. Poner un solo origen y un solo $t = 0$ para los dos móviles. Si uno sale más tarde, usar $t - t_0$.
2. Encuentro: igualar $x$ y despejar $t$; después igualar $y$.

**Trampas**
- Los ángulos "por debajo de la horizontal" llevan $\sin\theta < 0$.
- El tiro desde una plataforma que se mueve se ve en el §3.
- Si un proyectil apunta directo a un objeto que se deja caer en el mismo instante, siempre le pega (los dos caen igual).

**Practicar:** D22-1, J24-2, D24-2, F25-2, D25-1, D23-1.

---

## 3. Movimiento relativo y MCU (T3) ★★

**La idea**
- Una velocidad siempre se mide **respecto a algo**. Si yo camino a 1 m/s dentro de un tren que va a 20 m/s, para el andén voy a 21 m/s.
- En vectores: $\vec v_{yo/andén} = \vec v_{yo/tren} + \vec v_{tren/andén}$. Los subíndices se encadenan como fichas de dominó: el del medio se cancela.
- MCU: algo que gira con rapidez constante igual acelera, porque la dirección de $\vec v$ cambia. Esa aceleración apunta al centro y vale $v^2/R$.

**Ejemplo resuelto — F26-2.** Un barco va a $\vec v_{B/O} = (-2{,}5;\,-1{,}0)$ respecto a la orilla. Un pasajero ve una rama a $\vec v_{R/B} = (-0{,}5;\,0{,}3)$. ¿Velocidad del agua?
1. La rama flota, así que su velocidad es la del agua: $\vec v_{A/O} = \vec v_{R/O}$.
2. Encadenar: $\vec v_{R/O} = \vec v_{R/B} + \vec v_{B/O} = (-0{,}5 - 2{,}5;\ 0{,}3 - 1{,}0) = (-3{,}0;\,-0{,}7)$. Respuesta **e** ✔.

**Qué preguntan**
- **Composición de velocidades:** río y bote (D16-2, D21-2, F26-2), viento y avión (D18-2, J23-3), lluvia vista desde un ómnibus (J21-4), trenes (F19-3, F24-3), escaleras mecánicas (D22-2), barco y persona y ave (J22-2), vehículos ortogonales (J25-2).
- **Pelota pateada desde una plataforma que se mueve:** A20a-1, D20-1.
- **MCU:** dar la posición a partir de $\vec a$ (J22-3), movimiento circular combinado con traslación (J21-6, F16-2).
- **Cambio de referencial dada la ley horaria** (D23-4).
- **Rebote contra un cuerpo que se mueve** (F25-5): en el sistema del cuerpo, la pelota rebota con la misma rapidez relativa.

**Fórmulas**
$$\vec v_{A/T} = \vec v_{A/B} + \vec v_{B/T} \qquad \vec v_{A/B} = \vec v_A - \vec v_B$$
$$\text{MCU:}\ v = \omega R,\quad a_c = \frac{v^2}{R} = \omega^2 R\ (\text{hacia el centro}),\quad T = \frac{2\pi}{\omega}$$
$$\text{Circular no uniforme:}\ a_t = \frac{dv}{dt} = \alpha R,\quad |\vec a| = \sqrt{a_t^2 + a_c^2}$$

**Cómo se resuelve:** escribir cada velocidad como vector $(v_x, v_y)$ con nombre "de qué, respecto a qué", y sumar como una cadena: $A/T = A/B + B/T$.

**Practicar:** D22-2, F24-3, J25-2, F26-2, D20-1.

---

## 4. Dinámica: Newton, poleas, rozamiento (T4) ★★★

**La idea**
- Las fuerzas cambian la velocidad: $\sum\vec F = m\vec a$. Todo el tema consiste en **listar bien las fuerzas** (el diagrama de cuerpo libre) y proyectarlas en ejes cómodos.
- **Las fuerzas que siempre hay que buscar:**
  - peso $mg$, hacia abajo;
  - normal $N$, perpendicular a la superficie, y vale lo que haga falta, no siempre $mg$;
  - tensión $T$, a lo largo de la cuerda;
  - rozamiento, que es paralelo a la superficie y se opone al deslizamiento.
- **Rozamiento.** Si desliza, vale exactamente $\mu_k N$. Si está quieto, vale "lo que haga falta" hasta un tope de $\mu_s N$.
- **Ejes.** En un plano inclinado conviene poner un eje a lo largo del plano y otro perpendicular. Así la aceleración tiene una sola componente.

**Ejemplo resuelto — D18-4.** Un bloque sube un plano de $45°$ empujado por una fuerza **horizontal** $F = 3mg$, con $a = g/\sqrt2$. ¿Cuánto vale $\mu_k$?
1. Ejes: $x$ a lo largo del plano (hacia arriba), $y$ perpendicular al plano.
2. $F$ horizontal tiene componente $F\cos45°$ a lo largo del plano (empuja hacia arriba) y $F\sin45°$ contra el plano, que aumenta la normal.
3. Eje $y$: $N = mg\cos45° + F\sin45° = \tfrac{\sqrt2}{2}(mg + 3mg) = 2\sqrt2\,mg$.
4. Eje $x$: $F\cos45° - mg\sin45° - \mu_k N = ma \Rightarrow \sqrt2\,mg - 2\sqrt2\,\mu_k\,mg = mg/\sqrt2$.
5. Dividir por $\sqrt2\,mg$: $1 - 2\mu_k = 1/2 \Rightarrow \mu_k = 1/4$. Respuesta **d** ✔.

**Qué preguntan**
- **Bloques y poleas** con poleas móviles: D18-3, D20-3, D21-4, D22-7, F25-3, D25-2.
- **Plano inclinado con rozamiento:** hallar $\mu$ (D18-4, J20-2, J24-4, F26-1), el rango de masas para que no se mueva (D18-9, J22-4), o la aceleración (F20-3, F20-4, J23-4, F24-4, D24-4).
- **Bloques apilados** (D17-2, D19-3), bloque apretado contra una pared (J18-3), diagrama de cuerpo libre conceptual (J25-5).
- **Equilibrio de una partícula con resorte y rozamiento** (F17-7, J20-3), nudo de cuerdas (F25-4).
- **Ascensor con resorte** (D24-3), persona levantando una caja (D23-2).

**Fórmulas**
$$\sum \vec F = m\vec a \qquad f_k = \mu_k N \qquad f_s \le \mu_s N$$
$$\text{Plano liso:}\ a = g\sin\theta \qquad \text{baja a velocidad constante:}\ \mu_k = \tan\theta$$
$$\text{Rugoso, bajando:}\ a = g(\sin\theta - \mu\cos\theta) \qquad \text{subiendo (frenándose):}\ a = -g(\sin\theta + \mu\cos\theta)$$

**Vínculo de cuerdas con polea móvil** (lo que más se pregunta en este tema):
- Escribir el largo de la cuerda como suma de tramos y derivar dos veces. Ejemplo: $x_1 + 2x_2 = \text{cte} \Rightarrow a_1 = -2a_2$.
- Una polea móvil sin masa tiene la misma $T$ a los dos lados, así que tira con $2T$ del cuerpo que cuelga de ella.

**Cómo se resuelve**
1. Diagrama de cuerpo libre de cada bloque.
2. Elegir un eje por bloque, en el sentido en que se mueve.
3. Plantear $F = ma$ por bloque y agregar el vínculo.
4. Resolver el sistema.

**Rozamiento estático: ¿se mueve o no?**
1. Suponer que no se mueve y calcular la $f$ necesaria.
2. Si $|f| \le \mu_s N$, queda quieto. Si no, desliza con $f = \mu_k N$.
3. Para un rango de masas: plantear los dos casos límite (a punto de subir y a punto de bajar), con $f$ en sentidos opuestos.

**Trampas**
- Si hay una fuerza aplicada con un ángulo, cambia la normal: $N = mg\cos\theta \pm F\sin\phi$.
- En bloques apilados, el rozamiento entre los bloques actúa sobre los dos (acción y reacción).

**Practicar:** D22-7, F25-3, D25-2, J22-4, F24-4, D24-3.

---

## 5. Dinámica circular (T5) ★

**La idea:** no existe una "fuerza centrípeta" aparte. Es el nombre que se le da a la **suma** de las fuerzas reales (tensión, normal, rozamiento) en la dirección del centro, y esa suma tiene que valer $m\omega^2 r$. En la dirección vertical, si la altura no cambia, las fuerzas se compensan.

**Ejemplo resuelto — F19-1.** Un brazo de $a = 10$ cm con una cuerda de $L = 20$ cm gira de modo que la cuerda forma $30°$ con la vertical. ¿Cuántas rpm?
1. Radio del círculo: $r = a + L\sin30° = 0{,}10 + 0{,}10 = 0{,}20$ m.
2. Vertical: $T\cos\theta = mg$. Radial: $T\sin\theta = m\omega^2 r$. Dividiendo, $\tan\theta = \omega^2 r/g$.
3. $\omega^2 = 9{,}8\cdot\tan30°/0{,}20 = 28{,}3 \Rightarrow \omega = 5{,}32$ rad/s $= 5{,}32\cdot60/2\pi = 51$ rpm. Respuesta **c** ✔.

**Qué preguntan:** péndulo cónico, embudo y cono que gira (F17-3, F19-1, F22-4, J25-3, A20b-3), plataforma giratoria con rozamiento (F16-3), peralte (J16-8), lavarropas (F26-6), masa con cuerda y resorte (J17-4, D22-3).

**Fórmulas**
$$\sum F_{radial} = m\omega^2 r = \frac{mv^2}{r}\ (\text{hacia el centro})$$
$$\text{Péndulo cónico:}\ \tan\theta = \frac{\omega^2 r}{g},\quad \omega^2 = \frac{g}{L\cos\theta}$$
$$\text{Plataforma:}\ \mu_s g \ge \omega^2 r \qquad \text{Peralte:}\ v_{max}^2 = Rg\,\frac{\sin\theta + \mu\cos\theta}{\cos\theta - \mu\sin\theta}$$

**Trampa:** el radio del círculo es la distancia al eje ($r = L\sin\theta$, más el brazo si hay), no el largo del hilo.

---

## 6. Trabajo y potencia (T6) ★

**La idea**
- El trabajo es "fuerza por distancia en la dirección del movimiento".
- **El trabajo de todas las fuerzas es igual al cambio de energía cinética.** Esto permite saltear el tiempo: si piden velocidades o distancias sin tiempo, el trabajo suele ser más rápido que Newton.
- La potencia es trabajo por segundo: $P = Fv$.

**Ejemplo resuelto — A20a-3.** Un cuerpo baja desde el reposo un plano de $30°$ y sigue por un piso horizontal hasta frenar. Recorre la misma distancia $d$ en cada tramo, con el mismo $\mu$. ¿Cuánto vale $\mu$?
1. Empieza y termina quieto, así que $W_{total} = 0$.
2. La gravedad aporta $mg\,d\sin30°$. El rozamiento resta $\mu mg\cos30°\,d$ en el plano y $\mu mg\,d$ en el piso.
3. $\sin30° = \mu(\cos30° + 1) \Rightarrow \mu = 0{,}5/1{,}866 = 0{,}27$. Respuesta **e** ✔.

**Qué preguntan:** distancia de frenado (J25-1: con el doble de velocidad, la distancia es 4 veces mayor), plano inclinado y después piso con el mismo $\mu$ (A20a-3, F22-3), trabajo del resorte (F24-5), potencia (J16-9, D20-9, F21-5), trabajo de $F$ a velocidad constante (D25-3).

**Fórmulas**
$$W = \int \vec F\cdot d\vec r \qquad W_{neto} = \Delta K \qquad W_{roz} = -\mu N d \qquad W_{resorte} = -\tfrac12 k(x_f^2 - x_i^2)$$
$$P = \vec F\cdot\vec v \qquad \text{velocidad límite con } F = -bv:\ v_L = mg/b$$

**Dato útil:** un resorte de longitud natural nula que se mueve entre dos puntos tiene $W = -\tfrac12 k(r_f^2 - r_i^2)$, donde $r$ es la distancia al punto fijo. Solo importan las posiciones inicial y final (F24-5).

---

## 7. Conservación de la energía (T7) ★★

**La idea**
- La energía se transforma entre movimiento ($K$), altura ($U_g$) y resortes ($U_e$) sin perderse, mientras no haya rozamiento que la disipe.
- Se aplica comparando **dos fotos**, el inicio y el punto que interesa: $E_A = E_B$. Si hay rozamiento: $E_B = E_A + W_{roz}$, y $W_{roz}$ es negativo.
- **En problemas de pistas circulares** se combinan dos cosas:
  - la energía da la velocidad en un punto;
  - Newton radial en ese punto da la normal, o la condición de no despegarse ($N \ge 0$).

**Ejemplo resuelto — D22-5.** Una bola cuelga de un hilo $L$ y se suelta desde la altura de $O$. Abajo, el hilo se engancha en una clavija $P$ a distancia $d$ debajo de $O$ y la bola gira en un círculo de radio $r = L - d$. ¿Cuánto vale el $d$ mínimo para que dé la vuelta?
1. Energía hasta abajo: $v_{abajo}^2 = 2gL$.
2. Para completar la vuelta, arriba del círculo chico $T \ge 0$, o sea $v_{arriba}^2 \ge gr$.
3. Energía de abajo hasta arriba del círculo chico, que está a $2r$ de altura: $v_{arriba}^2 = 2gL - 4gr$.
4. $2gL - 4gr \ge gr \Rightarrow r \le \tfrac25 L \Rightarrow d = L - r \ge \tfrac35 L$. Respuesta **a** ✔.

**Qué preguntan**
- **Rizo o loop:** compresión mínima del resorte o altura mínima, para partícula (D16-5, J20-5) y para cuerpo que rueda (J17-10, J23-6, J24-6).
- **Desprendimiento** de una pista o esfera (A20a-5, A20b-5), **normal** en un punto de una pista circular (F21-2, J18-10, D25-4), péndulo con clavija (D22-5).
- **Energía con rodadura:** yo-yo (D16-8, F22-7), cilindro que sube un plano (J22-6), sistemas con resortes y bloques (F18-6, D23-7, J25-6).

**Fórmulas**
$$E = K + U_g + U_e \qquad W_{nc} = \Delta E \qquad U_g = mgh \qquad U_e = \tfrac12 k x^2$$
$$K_{rígido} = \tfrac12 M v_{cm}^2 + \tfrac12 I_{cm}\omega^2 = \tfrac12 M v^2(1+\beta) \quad \text{si rueda sin deslizar, con } \beta = \frac{I_{cm}}{MR^2}$$

$\beta$ vale: aro 1, disco o cilindro 1/2, esfera maciza 2/5, esfera hueca 2/3.

**Resultados que conviene saber de memoria**

| Situación | Resultado |
|---|---|
| Arriba de un loop (partícula) | $v_{top}^2 \ge gR$ |
| Altura mínima para un loop desde el reposo | $h = \tfrac52 R$ |
| Loop rodando (cuerpo de radio $r$) | $v_{top}^2 \ge g(R - r)$, $h_{min} = 2R + \tfrac12(1+\beta)R$ (esfera: $2{,}7R$) |
| Se suelta desde arriba de una esfera | se despega en $\cos\theta = 2/3$ |
| Despegue en general | $N = 0$ con $mg\cos\theta = mv^2/R$ |
| Yo-yo (cuerda fija) | $v = \sqrt{2gh/(1+\beta)}$; disco: $\sqrt{4gh/3}$ |
| Rodar subiendo una altura | $h = \dfrac{(1+\beta)v^2}{2g}$ |

**Qué fuerzas no trabajan** (se pregunta como teoría):
- El rozamiento **estático** en rodadura sin deslizar (el punto de contacto está quieto).
- La tensión de una cuerda fija que se desenrolla (yo-yo).
- La normal.
- La tensión de un péndulo.

**Practicar:** J24-6, D22-5, D25-4, J23-6, F22-7, J25-6.

---

## 8. Choques y centro de masa (T8) ★★

**La idea**
- En un choque o una explosión, las fuerzas internas son enormes y duran un instante. Las de afuera (peso, rozamiento) no llegan a hacer nada en ese instante.
- Por eso **la cantidad de movimiento total $\sum m\vec v$ es la misma justo antes y justo después.**
- La energía cinética **no** tiene por qué conservarse: solo se conserva si el choque es elástico.
- **Centro de masa.** Es el "promedio pesado" de las posiciones. Si nada externo empuja al sistema, el CM no se mueve, aunque las partes se muevan (bote: si el pescador camina hacia adelante, el bote va hacia atrás).

**Ejemplo resuelto — F20-6.** $m_1 = 20$ kg a $2{,}0$ m/s choca con $m_2 = 12$ kg en reposo. Después, $m_1$ sale a $1{,}0$ m/s a $30°$. ¿Rapidez de $m_2$?
1. No se sabe si es elástico, así que **solo** se usa $\vec p$.
2. Eje $x$: $20\cdot2 = 20\cdot1\cdot\cos30° + 12\,v_{2x} \Rightarrow v_{2x} = (40 - 17{,}3)/12 = 1{,}89$.
3. Eje $y$: $0 = 20\cdot1\cdot\sin30° + 12\,v_{2y} \Rightarrow v_{2y} = -0{,}83$.
4. $|v_2| = \sqrt{1{,}89^2 + 0{,}83^2} = 2{,}1$ m/s. Respuesta **d** ✔.

**Qué preguntan**
- **Choques 2D:** con ángulos dados (F18-5, F20-6, J24-5, J25-4), choque elástico de masas iguales (D20-6), posibilidad energética (D16-6).
- **Explosiones:** D18-5, F20-2, J20-6, D21-5, F26-4.
- **Choque inelástico y después rozamiento o resorte:** F17-2, J18-1, A20b-4, J21-1, D24-6.
- **Centro de masa de un sistema aislado:** bote, vagón, plataforma (F16-4, D17-6, F19-2, J20-4). Disco con agujeros (D19-5).
- **Péndulo balístico:** J21-5, F19-5, D17-3.

**Fórmulas**
$$\vec P = \sum m_i\vec v_i \ \text{se conserva si } \sum \vec F_{ext} = 0 \ (\text{o durante el choque, que es instantáneo})$$
$$\vec r_{cm} = \frac{\sum m_i \vec r_i}{M} \qquad \text{agujero = masa negativa} \qquad \text{sistema aislado en reposo: } \sum m_i\,\Delta x_i = 0$$
$$\text{Elástico 1D, } m_2 \text{ en reposo:}\ v_1' = \frac{m_1-m_2}{m_1+m_2}v_1,\quad v_2' = \frac{2m_1}{m_1+m_2}v_1$$
$$\text{Totalmente inelástico:}\ v' = \frac{m_1v_1 + m_2 v_2}{m_1+m_2},\quad \Delta K = -\tfrac12\frac{m_1m_2}{m_1+m_2}v_{rel}^2$$
$$\text{Péndulo balístico:}\ v = \frac{m+M}{m}\sqrt{2gh}$$

- **Elástico con masas iguales y una en reposo (2D):** las dos salen a 90°.
- **Explosión desde el reposo:** $\sum m_i\vec v_i = 0$. Con 3 fragmentos, los vectores $m_i\vec v_i$ forman un triángulo cerrado.

**Cómo se resuelve un choque 2D**
1. Plantear $p_x$ y $p_y$ por separado.
2. Si es elástico, agregar la conservación de $K$.
3. Usar $\sin^2 + \cos^2 = 1$ para eliminar el ángulo que no se conoce.

**Trampa:** en un choque con rozamiento, $\vec p$ se conserva solo durante el instante del choque. Antes y después hay que usar $W_{roz} = \Delta K$.

**Practicar:** J24-5, J25-4, F26-4, D24-6, D23-5, F24-6.

---

## 9. Cinemática del rígido y momento de inercia (T9) ★

**La idea**
- Un rígido que se mueve es "trasladar el CM + girar alrededor del CM". Todos los puntos giran con el mismo $\omega$.
- **Rodar sin deslizar** quiere decir que el punto que toca el piso está quieto en ese instante. De ahí sale $v_{cm} = \omega R$.
- El **momento de inercia** $I$ es la "masa de la rotación": cuánto cuesta hacer girar al cuerpo. Depende de qué tan lejos del eje está la masa.
  - Con Steiner se cambia de eje: $I_O = I_{cm} + Md^2$.
  - Los momentos se suman y se restan como las masas, siempre que estén calculados respecto al **mismo eje**.

**Ejemplo resuelto — J16-1.** Un disco de radio $R$ tiene un agujero de radio $R/2$ cuyo borde pasa por el centro, así que el centro del agujero está a $R/2$. ¿Cuánto vale $I$ respecto al centro del disco?
1. Disco entero: $M = \sigma\pi R^2$, $I_1 = \tfrac12\sigma\pi R^4$.
2. Pedazo que falta: $m = \sigma\pi R^2/4$. Su $I$ respecto al centro del disco sale por Steiner: $\tfrac12 m(R/2)^2 + m(R/2)^2 = \tfrac38 mR^2 = \tfrac{3}{32}\sigma\pi R^4$.
3. $I = \tfrac{16}{32}\sigma\pi R^4 - \tfrac{3}{32}\sigma\pi R^4 = \tfrac{13}{32}\pi\sigma R^4$. Respuesta **a** ✔.

**Qué preguntan:** momento de inercia de una figura compuesta o con agujero (J16-1, F18-7), velocidad de un punto de una rueda (F16-5, J17-3, F21-7), engranajes y correas (D18-7), rulemán (J23-5).

**Fórmulas**
$$\vec v_P = \vec v_{cm} + \vec\omega\times\vec r_{P/cm} \qquad \text{rodadura sin deslizar: } v_{cm} = \omega R,\ a_{cm} = \alpha R$$
$$\text{En rodadura: } v_{contacto} = 0,\quad v_{arriba} = 2v_{cm},\quad \vec a_{contacto} = \omega^2 R\ \text{hacia el centro}$$
$$\textbf{Steiner: } I_O = I_{cm} + Md^2 \qquad \text{correa: } \omega_1R_1 = \omega_2R_2$$

| Cuerpo | $I_{cm}$ | Útil |
|---|---|---|
| Barra | $ML^2/12$ | por un extremo: $ML^2/3$ |
| Disco / cilindro | $MR^2/2$ | por el borde: $\tfrac32 MR^2$ |
| Aro | $MR^2$ | por el borde: $2MR^2$ |
| Esfera maciza | $\tfrac25MR^2$ | por la superficie: $\tfrac75 MR^2$ |
| Masa puntual | — | $md^2$ |

**Disco con agujero:** $I = I_{disco} - (I_{agujero,cm} + m_a d^2)$, con $m_a = \sigma\pi r^2$.

---

## 10. Dinámica del rígido (T10) ★★★ — el tema que más pesa

**La idea**
- Un rígido obedece **dos** leyes de Newton al mismo tiempo:
  - la de traslación del CM, $\sum F = Ma$;
  - la de rotación, $\sum\tau = I\alpha$.
  El torque $\tau$ = fuerza × brazo es "cuánto hace girar" una fuerza.
- Si rueda sin deslizar, las dos leyes quedan atadas por $a = \alpha R$.
- **El rozamiento estático en rodadura es una incógnita más.** No vale $\mu N$: vale lo que haga falta para que se cumpla $a = \alpha R$. Recién al final se compara con $\mu_s N$ para saber si de verdad rueda.
- **Receta universal:** 3 ecuaciones (fuerza, torque, vínculo) para 3 incógnitas ($a$, $\alpha$, $f$). Si hay bloques, se agregan más ecuaciones $F = ma$ y vínculos de cuerda.

**Ejemplo resuelto — D22-6.** Una esfera maciza de $M = 5$ kg rueda sin deslizar. Una fuerza horizontal $F = 10$ N actúa a $h = R/2$ por encima del centro. ¿Cuánto vale $a_{cm}$?
1. Incógnitas: $a$, $\alpha$, $f$. Se supone $f$ hacia adelante.
2. Traslación: $F + f = Ma$.
3. Rotación respecto al CM: $F$ hace torque $Fh$ y $f$ hace torque $-fR$. Entonces $Fh - fR = I\alpha = \tfrac25MR^2\cdot\tfrac aR$, o sea $F\tfrac hR - f = \tfrac25 Ma$.
4. Sumando 2 y 3: $F(1 + \tfrac hR) = \tfrac75 Ma \Rightarrow a = \dfrac{10\cdot1{,}5}{5\cdot1{,}4} = 2{,}14$ m/s². Respuesta **a** ✔.

F26-8 es el mismo problema al revés: con $F = 14$ N, $M = 7$ kg y $a = 2$ m/s², $1 + h/R = 1{,}4$, así que $h = 0{,}4R = 0{,}10$ m (respuesta **c** ✔).

**Qué preguntan**

| Problema típico | Ejercicios |
|---|---|
| **Rodadura con una fuerza aplicada:** aceleración, fuerza máxima sin deslizar, altura de la fuerza | F17-5, D22-6, F26-9, D25-6, J18-9 |
| **Paso de deslizar a rodar:** tiempo, posición, velocidad final | J16-4, J20-7, F20-8, F19-6, F25-8, J18-8 |
| **Rodadura en un plano inclinado:** rozamiento, $\mu$ mínimo | J18-6/7, J19-6, J22-7, D21-7 |
| **Poleas con inercia y carretes:** bloques, cuerdas enrolladas en distintos radios | D17-7, D19-7, J24-7, D24-8, J25-8, F26-7, D21-6 |
| **Disco que rueda atado a bloques** | F17-8, D23-8, F24-9, F22-8 |
| **$\tau = I\alpha$ con eje fijo:** frenado, barra soltada | J17-2, J23-7, F26-8, D24-9, J19-5 |
| **Yo-yo con el centro quieto, moneda que no gira** | F21-9, F21-10 |

**Fórmulas**
$$\sum \vec F_{ext} = M\vec a_{cm} \qquad \sum \tau_{cm} = I_{cm}\,\alpha \qquad (\text{eje fijo } O:\ \sum\tau_O = I_O\,\alpha)$$
$$\tau = rF\sin\phi = F \times \text{brazo} \qquad \text{rodadura: } a = \alpha R,\ f \text{ estático y desconocido (plantearlo con signo)}$$

**Resultados clave** (con $\beta = I_{cm}/MR^2$)

| Situación | Resultado | Disco ($\beta = \tfrac12$) | Esfera ($\beta = \tfrac25$) |
|---|---|---|---|
| Rueda bajando un plano | $a = \dfrac{g\sin\theta}{1+\beta}$ | $\tfrac23 g\sin\theta$ | $\tfrac57 g\sin\theta$ |
| Rozamiento en el plano | $f = \dfrac{\beta}{1+\beta}Mg\sin\theta$ | $\tfrac13 Mg\sin\theta$ | $\tfrac27 Mg\sin\theta$ |
| $\mu_s$ mínimo para rodar | $\mu \ge \dfrac{\beta}{1+\beta}\tan\theta$ | $\tfrac13\tan\theta$ | $\tfrac27\tan\theta$ |
| $F$ horizontal a altura $h$ sobre el centro | $a = \dfrac{F(1 + h/R)}{M(1+\beta)}$ | | |
| ... con $F$ en el punto de arriba ($h = R$) | $a = \dfrac{2F}{M(1+\beta)}$, $f = F\dfrac{1-\beta}{1+\beta}$ | $a = \tfrac{4F}{3M}$, $f = \tfrac F3$ | |
| ... con $F$ en el centro ($h = 0$) | $a = \dfrac{F}{M(1+\beta)}$ | | |
| Altura para que $f = 0$ | $h = \beta R$ | $R/2$ | $\tfrac25R$ |
| Yo-yo con la cuerda fija | $a = \dfrac{g}{1+\beta}$, $T = \dfrac{\beta}{1+\beta}Mg$ | $\tfrac23 g$, $\tfrac13 Mg$ | |

**Paso de deslizar a rodar** (en horizontal, con rozamiento cinético $\mu$):
- El rozamiento frena al CM, $a = -\mu g$, y hace girar al cuerpo, $\alpha = \mu g/(\beta R)$.
- Sin rotación inicial: $v_f = \dfrac{v_0}{1+\beta}$ (disco $\tfrac23 v_0$, esfera $\tfrac57 v_0$) y $t = \dfrac{\beta\,v_0}{(1+\beta)\mu g}$.
- **Atajo:** el $L$ respecto al punto de contacto se conserva, porque el rozamiento pasa por ese punto: $Mv_0R + I\omega_0 = (MR^2 + I)\,\omega_f$.
- Para que quede en reposo (F25-8): $Mv_0R = I\omega_0$ con signos opuestos ($v_0 = \beta\omega_0 R$).

**Cómo se resuelve**
1. Diagrama de cuerpo libre del rígido con el rozamiento $f$ en un sentido supuesto.
2. Plantear $\sum F = Ma$ y $\sum\tau_{cm} = I\alpha$.
3. Agregar el vínculo $a = \alpha R$.
4. Si hay bloques, $F = ma$ de cada bloque y el vínculo de las cuerdas. **Si la cuerda está enrollada en un radio $r$, el bloque se mueve con $a = \alpha r$.** Si la cuerda está atada al centro, se mueve con $a_{cm}$. Si sale del punto de arriba de un cuerpo que rueda, se mueve con $2a_{cm}$.
5. Si da $f < 0$, el rozamiento apunta para el otro lado (no es un error).

**Trampas**
- **El carrete (cuerda en el radio interno $r$):** puede rodar hacia donde tirás o al revés, según el ángulo. Los torques se toman respecto al punto de contacto.
- En una polea con inercia, la tensión es distinta a cada lado: $(T_1 - T_2)R = I\alpha$.

**Practicar (orden sugerido):** J22-7, D22-6, F26-9, J25-8, F26-7, D24-8, F25-8, J20-7, D23-8, D25-6.

---

## 11. Momento angular (T11) ★★★

**La idea**
- El momento angular $L$ es la "cantidad de giro". Para un rígido vale $L = I\omega$. Para una partícula vale $L = m\,v\,d_\perp$, donde $d_\perp$ es la distancia del eje a la recta por donde va la partícula.
- **Si nada externo hace torque, $L$ no cambia.** Por eso la patinadora gira más rápido cuando cierra los brazos: baja $I$ y sube $\omega$.
- Se usa como $\vec p$ en los choques: comparar **antes** y **después**. Con eje fijo, se toma $L$ **respecto al eje**, porque la fuerza del eje no hace torque ahí.

**Ejemplo resuelto — D25-9.** Un carrusel (disco, $M = 150$ kg, $R = 2$ m) gira a $\omega_0 = 0{,}5$ rad/s con un conejo de $5$ kg en el borde. El conejo salta tangencialmente y queda con $v = 2{,}5$ m/s **respecto al suelo**. ¿Cuánto vale $\omega_f$?
1. $I_{disco} = \tfrac12\cdot150\cdot4 = 300$ kg m². El conejo en el borde aporta $mR^2 = 20$.
2. Antes: $L = (300 + 20)\cdot0{,}5 = 160$.
3. Después: $L = 300\,\omega_f + m v R = 300\,\omega_f + 5\cdot2{,}5\cdot2 = 300\,\omega_f + 25$.
4. $\omega_f = 135/300 = 0{,}45$ rad/s. Respuesta **a** ✔.

**Qué preguntan**

| Problema típico | Ejercicios |
|---|---|
| **Persona o insecto que camina, salta o cae** sobre una plataforma o disco que gira libre | J17-7, D21-9, D23-9, D25-9, F26-10, J20-9 |
| **Discos o cuerpos que se acoplan:** $\omega$ final, energía perdida | F19-8, D19-8, F20-9, A20a-9 |
| **Partícula que choca con una barra o disco pivotado:** $\omega$ después, altura o ángulo máximo | D16-7, D18-6, J19-10, F21-6, D20-8, J24-8, F25-9, A20a-8, A20b-8 |
| **Cuentas que se deslizan por una varilla que gira** | J21-2, J22-8, D22-8, F22-9 |
| **Qué se conserva** (teoría) | J16-3, J16-10, F17-4, F18-2, F19-10, J25-10 |
| **Bala que roza un disco** | F24-8 |

**Fórmulas**
$$\vec L = \vec r\times m\vec v \ (\text{partícula: } L = m\,v\,d_\perp) \qquad L = I\omega \ (\text{rígido, eje fijo})$$
$$\frac{d\vec L_O}{dt} = \sum\vec\tau_O^{ext} \ \Rightarrow\ \text{si } \tau_{ext} = 0:\ I_1\omega_1 = I_2\omega_2$$
$$\text{Acople:}\ \omega_f = \frac{I_1\omega_1 + I_2\omega_2}{I_1 + I_2},\quad \Delta K = -\tfrac12\frac{I_1I_2}{I_1+I_2}(\omega_1-\omega_2)^2$$
$$\text{Partícula que se pega a una barra pivotada en } O:\ m v d = (I_O + md^2)\,\omega$$
$$\text{Elástico contra una barra pivotada: conservar } L_O \text{ y } K \ (\text{dos ecuaciones})$$

**Qué se conserva en un choque contra un cuerpo pivotado**

| Magnitud | ¿Se conserva? | Por qué |
|---|---|---|
| $L$ respecto al pivote $O$ | **sí** | la reacción del pivote no hace torque respecto a $O$ |
| $\vec p$ lineal | **no** | la reacción del pivote es una fuerza externa impulsiva |
| $E$ mecánica | solo si el choque es elástico | |
| $L$ respecto a otro punto (el CM) | **no** | |

**Después de un choque** (barra que sube o péndulo que oscila):
- $L$ ya no se conserva, porque la gravedad hace torque.
- La energía sí se conserva.
- Para hallar la altura o el ángulo máximo, usar $\tfrac12 I_O\omega^2 = Mg\,\Delta h_{cm}$.

**Persona que camina hacia el centro:** $I$ baja, $\omega$ sube y $K$ **aumenta** (la persona hace trabajo). Variación porcentual: $\Delta K/K = I_i/I_f - 1$.

**Trampa:** cuando la persona salta, su $L$ es $m\,v_{suelo}R$ y se calcula con la velocidad **respecto al suelo**, no respecto a la plataforma.

**Practicar:** D25-9, F26-10, F25-9, J24-8, D22-8, D23-9, J25-10.

---

## 12. Equilibrio del rígido (T12) ★★

**La idea**
- Que un rígido esté quieto exige dos cosas: que no se traslade ($\sum F = 0$) y que no gire ($\sum\tau = 0$).
- **El truco es elegir el punto de torques.** Las fuerzas que pasan por ese punto no aparecen en la ecuación. Conviene elegir el punto donde hay más incógnitas.
- En los problemas de "a punto de...", una de las fuerzas llega a su límite:
  - deslizar: $f = \mu_s N$;
  - volcar o separarse de un apoyo: la normal de ese apoyo se hace cero.

**Ejemplo resuelto — D24-7.** Una tabla de largo $L$ está hecha de dos trozos de $L/2$ con $m_1 = 2m_2$, apoyada sobre una mesa. ¿Cuánto tiene que estar apoyado, como mínimo, desde el borde izquierdo del trozo 1?
1. Mientras el CM esté sobre la mesa, la tabla no vuelca. En el límite, la normal se va toda al borde de la mesa.
2. CM desde el borde izquierdo: $x_{cm} = \dfrac{2m\cdot\tfrac L4 + m\cdot\tfrac{3L}4}{3m} = \dfrac{5L}{12}$.
3. $d_{min} = 5L/12$. Respuesta **a** ✔.

**Qué preguntan**
- **Barra apoyada:** en pared y piso con rozamiento (F22-6, D21-8 esfera), barra con cable y articulación (F18-3, A20b-9, D25-5, J24-9), tablón con cuerda (F26-5).
- **Disco contra un escalón** (J17-6, J23-9) o contra una pared con fuerza (J21-3, J22-9).
- **Tabla que sobresale de la mesa** (D22-9, D24-7), banco con macetas (J25-7), sube y baja (F25-6), barras articuladas (D23-6).
- **Vuelco de un bloque** (J16-7), barra colgada de dos cuerdas (J18-4), disco en una cuña (D17-5, F24-7).

**Fórmulas**
$$\sum\vec F = 0 \qquad \sum\tau_P = 0 \ \text{respecto a cualquier punto } P$$

**Cómo se resuelve**
1. Diagrama de cuerpo libre. En una articulación hay dos componentes de reacción desconocidas.
2. **Tomar torques respecto al punto por donde pasan más fuerzas desconocidas** (la articulación o el punto de contacto con rozamiento).
3. Para el caso "a punto de deslizar", poner $f = \mu_s N$.

**Casos límite que conviene saber**

| Caso | Condición |
|---|---|
| Vuelco | la normal se va al borde. Bloque con reborde: $\tan\phi \le L/H$ |
| Tabla que sobresale | a punto de caer, la normal está en el borde de la mesa: $x_{cm} = $ borde |
| Disco por subir el escalón | $N_{piso} = 0$. Torques respecto a la esquina: $F(R-h) = Mg\sqrt{2Rh - h^2}$ (con $F$ horizontal en el centro) |
| Esfera con contactos lisos | todas las normales pasan por el centro |

**Practicar:** F26-5, D25-5, J25-7, D24-7, J24-9, F22-6.

---

## 13. Oscilaciones (T13) ★★★ — casi siempre el ej. 10

**La idea**
- Si al apartar algo del equilibrio aparece una fuerza (o un torque) **proporcional al apartamiento y en contra**, el movimiento es un MAS: una oscilación senoidal.
- Siempre se llega a una ecuación de la forma $\ddot q = -\omega^2 q$, y ese $\omega$ es todo lo que piden.
- Para sacar $\omega$ hay dos caminos:
  1. Newton o torque, que da directamente $-\omega^2 q$.
  2. Energía: $\omega^2 = k_{ef}/m_{ef}$, donde $k_{ef}$ es "la rigidez" y $m_{ef}$ "la inercia" del movimiento.
- Para "pequeñas oscilaciones" se usa $\sin\theta \approx \theta$.

**Ejemplo resuelto 1 — D25-8.** Masa-resorte con $m = 0{,}5$ kg y $k = 50$ N/m. En $t = 0$: $x = 0$, $v = -1$ m/s. Piden $\omega$, $A$ y $\phi$.
1. $\omega = \sqrt{k/m} = 10$ rad/s.
2. $A = v_{max}/\omega = 0{,}10$ m, porque pasa por $x = 0$ a máxima velocidad.
3. $x(0) = A\cos\phi = 0 \Rightarrow \phi = \pm\pi/2$. $v(0) = -A\omega\sin\phi = -1 < 0 \Rightarrow \sin\phi > 0 \Rightarrow \phi = \pi/2$. Respuesta **a** ✔.

**Ejemplo resuelto 2 — F25-10 (péndulo físico).** Una barra $m$, $L$ cuelga de $O$, con una masa $m$ en el medio y otra en el extremo. ¿Período?
1. $I_O = \tfrac13 mL^2 + m(L/2)^2 + mL^2 = \tfrac{19}{12}mL^2$.
2. CM total: $d = \dfrac{m\tfrac L2 + m\tfrac L2 + mL}{3m} = \tfrac23 L$.
3. $\omega^2 = \dfrac{(3m)\,g\,d}{I_O} = \dfrac{2mgL}{\tfrac{19}{12}mL^2} = \dfrac{24g}{19L} \Rightarrow T = 2\pi\sqrt{\dfrac{19L}{24g}}$. Respuesta **c** ✔.

**Qué preguntan**

| Problema típico | Ejercicios |
|---|---|
| **Péndulo físico:** barra, barra con disco, barra con masas, barra con bala | D16-10, J16-2, J19-8, J22-10, D22-10, F25-10, J25-9 |
| **Disco que rueda con resortes** en el centro o arriba | F16-7, D18-10, J21-8, J23-10, D23-10, J24-10, A20b-10 |
| **Masa-resorte:** $x(t)$, $v_{max}$, fase, resortes en paralelo | D19-10, F18-8, F21-8, D25-8 |
| **Resortes con poleas** | F22-10, F24-10 |
| **Torsión, barra con resortes** | J17-8, F20-10, A20a-10, D21-10, F19-7 |
| **No deslizar durante el MAS** | D20-10 (disco), D24-10 (bloque sobre plataforma) |

**Fórmulas**
$$\ddot x + \omega^2 x = 0 \ \Rightarrow\ x = A\cos(\omega t + \phi),\quad v = -A\omega\sin(\omega t + \phi),\quad a = -\omega^2 x$$
$$T = \frac{2\pi}{\omega} = \frac1f \qquad v_{max} = A\omega \qquad a_{max} = A\omega^2 \qquad E = \tfrac12 kA^2$$
$$A = \sqrt{x_0^2 + (v_0/\omega)^2} \qquad \tan\phi = -\frac{v_0}{\omega x_0}$$

**Método por energía** (sirve para cualquier sistema):
1. Escribir $E = \tfrac12 m_{ef}\,\dot q^2 + \tfrac12 k_{ef}\,q^2$.
2. Entonces $\omega^2 = k_{ef}/m_{ef}$.

| Sistema | $\omega^2$ |
|---|---|
| Masa-resorte | $k/m$ (la gravedad solo corre el punto de equilibrio) |
| Resortes en paralelo, o a los dos lados del bloque | $k_{ef} = k_1 + k_2$ |
| Resortes en serie | $k_{ef} = \dfrac{k_1k_2}{k_1+k_2}$ |
| Péndulo simple | $g/L$ |
| **Péndulo físico** | $\dfrac{M_{tot}\,g\,d}{I_O}$, con $d$ = distancia de $O$ al CM total, $I_O$ por Steiner |
| Barra colgada de un extremo | $\dfrac{3g}{2L}$ |
| Barra colgada a distancia $l$ del centro | $\dfrac{gl}{L^2/12 + l^2}$ |
| Esfera colgada de un punto de su superficie | $\dfrac{g}{\tfrac75 R}$ |
| Torsión | $\kappa/I$ |
| Torsión + gravedad | $\dfrac{\kappa + Mgd}{I_O}$ |
| **Disco que rueda con resorte en el centro** | $\dfrac{k}{M(1+\beta)} = \dfrac{2k}{3M}$ |
| Disco que rueda con resorte en el punto de arriba (se estira $2x$) | $\dfrac{4k}{\tfrac32 M} = \dfrac{8k}{3M}$ |
| Polea móvil con resorte (el bloque baja $x$, el resorte se estira $2x$) | $4k/m$ |
| Barra con resorte en un extremo, oscilando en horizontal | $\dfrac{kL^2}{I_O}$ (con $\sin\theta \approx \theta$) |

**Condiciones para no deslizar en un MAS**
- Bloque sobre una plataforma que oscila: $\mu_s \ge \dfrac{\omega^2 A}{g}$.
- Disco que rueda con resorte: $f_{max} = \beta M\,a_{max}/(1+\beta) \le \mu_s Mg$. Para el disco: $\dfrac{kA}{3} \le \mu_s Mg$.

**Teoría que se pregunta**
- En un MAS sin rozamiento, la $E$ se conserva.
- $L$ **no** se conserva cuando hay gravedad o resorte con torque.
- La masa no cambia el período de un péndulo simple, pero sí el de un péndulo físico si cambia la distribución de masa.

**Practicar:** D25-8, J25-9, F25-10, J24-10, F24-10, D23-10, D22-10.

---

## 14. Hoja de fórmulas (repaso en 10 min antes del examen)

| | |
|---|---|
| **Tiro** | $y = x\tan\theta - \dfrac{gx^2}{2v_0^2\cos^2\theta}$ · $R = v_0^2\sin2\theta/g$ · $v^2 = v_0^2 + 2a\Delta x$ |
| **Relativo** | $\vec v_{A/T} = \vec v_{A/B} + \vec v_{B/T}$ |
| **Circular** | $a_c = v^2/r = \omega^2 r$ · péndulo cónico: $\omega^2 = g/(L\cos\theta)$ |
| **Newton** | $\sum F = ma$ · $f_k = \mu_kN$ · $f_s \le \mu_sN$ · vínculo de cuerdas derivando el largo |
| **Energía** | $W_{nc} = \Delta E$ · $P = F\cdot v$ · loop: $v_{top}^2 \ge gR$ · despegue: $N = 0$ |
| **Choques** | $\sum m\vec v$ se conserva · inelástico: $\Delta K = -\tfrac12\mu v_{rel}^2$ · masas iguales elástico 2D: salen a 90° |
| **CM** | $x_{cm} = \sum mx/M$ · aislado: $\sum m\Delta x = 0$ |
| **Inercia** | Steiner: $I_O = I_{cm} + Md^2$ · $\beta$: aro 1, disco ½, esfera ⅖ |
| **Rígido** | $\sum F = Ma_{cm}$ · $\tau_{cm} = I\alpha$ · $a = \alpha R$ · plano: $a = g\sin\theta/(1+\beta)$ |
| **Rodar ↔ deslizar** | $v_f = v_0/(1+\beta)$ · $L$ respecto al contacto se conserva |
| **Momento angular** | $L = I\omega$, $L = mvd_\perp$ · $\tau = 0 \Rightarrow I_1\omega_1 = I_2\omega_2$ · con pivote, se conserva $L_O$ pero no $p$ |
| **Equilibrio** | $\sum F = 0$, $\sum\tau = 0$ en el punto con más incógnitas |
| **MAS** | $\omega^2 = k_{ef}/m_{ef}$ · péndulo físico: $Mgd/I_O$ · disco con resorte: $2k/3M$ · $v_{max} = A\omega$ · no deslizar: $\mu g \ge \omega^2A$ |
