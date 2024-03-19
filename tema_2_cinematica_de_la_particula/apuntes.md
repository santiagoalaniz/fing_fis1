# Cinemática de la Partícula (1)

- Capítulo 2: secciones 2-1, 2-2, 2-3, 2-4, 2-5, 2-6 y 2-7.
- Capítulo 4: secciones 4-1, 4-2 y 4-3.

## 2-1 Cinemática de la Partícula

Introduce la cinemática, el estudio del movimiento sin considerar sus causas. Se enfoca en la descripción del movimiento de partículas, definiendo posición, velocidad y aceleración.

- **Posición**: La posición de una partícula se define como la ubicación de la partícula en el espacio. Se puede representar mediante un vector que va desde el origen de un sistema de coordenadas hasta la partícula.

- **Velocidad**: La velocidad de una partícula se define como la tasa de cambio de su posición con respecto al tiempo. Se puede representar mediante un vector que indica la dirección y magnitud del movimiento.

- **Aceleración**: La aceleración de una partícula se define como la tasa de cambio de su velocidad con respecto al tiempo. Se puede representar mediante un vector que indica la dirección y magnitud del cambio de velocidad.

## 2-2 Descripciones del Movimiento

Explica cómo describir el movimiento a través de ecuaciones y gráficas, incluyendo la posición en función del tiempo y la importancia de los marcos de referencia. Ambas herramientas son fundamentales para el análisis del movimiento. Destacamos algunas de las ecuaciones más importantes:

- Ningun movimiento: La particula esta en reposo, la velocidad y acelearacion son cero. Su funcion de posicion es constante.
$X(t) = C$
- Movimiento a velocidad constante: La particula se mueve a una velocidad constante. Su funcion de posicion es lineal.
$X(t) = C + Bt$
- Movimiento acelerado: La particula se mueve con velocidad variable. Su funcion de posicion es una curva.
$X(t) = C + Bt + At^2$

## 2-3 Velocidad Promedio

Define la velocidad promedio como el desplazamiento dividido por el tiempo transcurrido, destacando la diferencia entre velocidad promedio y velocidad instantánea.

$V_{prom} = \frac{\Delta X}{\Delta t} = \frac{X_f - X_i}{t_f - t_i}$

La velocidad promedio es una medida del cambio de posición en un intervalo de tiempo, mientras que la velocidad instantánea es la velocidad de un objeto en un instante específico.

## 2-4 Velocidad Instantánea

Podemos definir la velocidad instantánea como el límite de la velocidad promedio cuando el intervalo de tiempo tiende a cero.

$V = \lim_{\Delta t \to 0} \frac{\Delta X}{\Delta t} = \frac{dX}{dt}$

La velocidad instantánea es la derivada de la posición con respecto al tiempo, y es una medida de la rapidez y dirección del movimiento en un instante específico.

Para los casos planteados en la sección 2-2, las ecuaciones de velocidad instantánea son:

- Ningun movimiento: $V(t) = dX/dt = 0$ (no hay velocidad si la posición es constante).
- Movimiento a velocidad constante: $V(t) = dX/dt = B$ (la velocidad es constante).
- Movimiento acelerado: $V(t) = dX/dt = B + 2At$ (la velocidad cambia con el tiempo).

## 2-5 Movimiento Acelerado

De la misma forma que tenemos velocidad promedio e instantánea, podemos definir aceleración promedio e instantánea. La aceleración promedio se define como el cambio de velocidad dividido por el tiempo transcurrido, mientras que la aceleración instantánea es el límite de la aceleración promedio cuando el intervalo de tiempo tiende a cero.

$A_{prom} = \frac{\Delta V}{\Delta t} = \frac{V_f - V_i}{t_f - t_i}$

$A = \lim_{\Delta t \to 0} \frac{\Delta V}{\Delta t} = \frac{dV}{dt}$

La aceleración instantánea es la derivada de la velocidad con respecto al tiempo, y es una medida de la rapidez y dirección del cambio de velocidad en un instante específico.

Para los casos planteados en la sección 2-2, las ecuaciones de aceleración instantánea son:

- Ningun movimiento: $A(t) = dV/dt = 0$ (no hay aceleración si la posicion es constante).
- Movimiento a velocidad constante: $A(t) = dV/dt = 0$ (la velocidad es constante, no hay aceleración).
- Movimiento acelerado: $A(t) = dV/dt = 2A$ (la aceleración es constante).

## 2-6 Movimiento con Aceleración Constante

Es bastante comun encontrar movimientos con aceleracion constante en el dia a dia, veamos como se construyen las ecuaciones de movimiento para este caso.

Un dato a tener en cuenta es el siguiente:

**Si la aceleracion instantanea es constante entonces coincide con la aceleracion promedio para cualquier intervalo**.

Sea $A$ la aceleracion constante y $V_0$ $X_0$ la velocidad y posicion inicial en el tiempo $t_0 = 0$, la aceleracion promedio entre $t_0$ y $t$ es:

- $A = \frac{v - V_0}{t - t_0} = \frac{v - V_0}{t} \rightarrow v = V_0 + At$

**El promedio entre $V_0$ y $v$ es**.

- $V_{prom} = \frac{V_0 + v}{2} = \frac{V_0 + V_0 + At}{2} = V_0 + \frac{At}{2}$

**Pero tambien sabemos que**.

- $V_{prom} = \frac{\Delta X}{\Delta t} = \frac{X - X_0}{t - t_0} = \frac{X - X_0}{t}$

**Finalmente**.

- $X - X_0 = V_0t + \frac{1}{2}At^2 \rightarrow X = X_0 + V_0t + \frac{1}{2}At^2$

## 2-7 Cuerpos en Caída Libre

Trata sobre la caída libre como un caso particular de movimiento con aceleración constante (la gravedad), ignorando la resistencia del aire y aplicando las ecuaciones de movimiento.

La formula general para la posicion de un cuerpo en caida libre es:

- $X = X_0 + V_0t + \frac{1}{2}gt^2$

Donde $g$ es la aceleracion de la gravedad, $X_0$ la posicion inicial y $V_0$ la velocidad inicial.

### 4-1 Posición, Velocidad y Aceleración

Esta sección introduce cómo describir la posición, velocidad, y aceleración de una partícula en movimiento a través de un espacio tridimensional. Utiliza vectores para expresar estas cantidades, permitiendo un análisis más detallado del movimiento en cualquier dirección. La posición se define por el vector de posición $ \vec{r} $, la velocidad como la derivada de la posición respecto al tiempo $ \vec{v} = \frac{d\vec{r}}{dt} $, y la aceleración como la derivada de la velocidad respecto al tiempo $ \vec{a} = \frac{d\vec{v}}{dt} $ .

### 4-2 Movimiento con Aceleración Constante

Esta parte del texto extiende los conceptos de movimiento con aceleración constante a situaciones bidimensionales y tridimensionales. Se explica cómo las ecuaciones de movimiento aprendidas para el caso unidimensional también se aplican en contextos más complejos mediante la incorporación de vectores para describir las direcciones de movimiento. La sección enfatiza cómo la aceleración constante en una dirección afecta el movimiento en otras direcciones y cómo esto se representa mediante ecuaciones vectoriales .

### 4-3 Movimiento de Proyectiles

Aborda el estudio del movimiento de proyectiles como un ejemplo clásico de movimiento bidimensional bajo la acción de la gravedad. Esta sección describe cómo un proyectil lanzado al aire sigue una trayectoria parabólica, descomponiendo el movimiento en componentes horizontales y verticales. Se demuestra que, aunque el movimiento horizontal ocurre a una velocidad constante (si se ignora la resistencia del aire), la componente vertical está influenciada por la aceleración constante hacia abajo debido a la gravedad. Se presentan las ecuaciones para calcular el alcance, la altura máxima, y el tiempo total de vuelo del proyectil .
