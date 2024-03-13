# Trignometria y vectores.

- Capítulo 1: secciones 1-1, 1-2, 1-6 y 1-7.
- Capítulo 3: secciones 3-1, 3-2, 3-3, 3-4 y 3-5.

## 1-1 Las cantidades fisicas, patrones y unidades.

**Objetivo**: Identificar las cantidades fisicas, patrones y unidades.

- Tiempo, segundo, s
- Longitud, metro, m
- Masa, kilogramo, kg

## 1-2 El Sistema Internacional de Unidades.

- Giga $10^9$
- Mega $10^6$
- Kilo $10^3$
- Deci $10^{-1}$
- Centi $10^{-2}$
- Mili $10^{-3}$
- Micro $10^{-6}$
- Nano $10^{-9}$


## 1-6 Precisión y cifras significativas.

Las reglas para decidir cuántas cifras significativas incluir en los resultados de mediciones y cálculos son:

**Regla 1**: Al contar cifras significativas, empieza desde el primer dígito no cero a la izquierda. Conserva todos los dígitos hasta el primer dígito que es incierto.

**Regla 2**: Al multiplicar o dividir, el resultado no debe tener más cifras significativas que el factor con el menor número de cifras significativas.

**Regla 3**: Al sumar o restar, el resultado no debe tener más decimales que el factor con el menor número de decimales.

## 1-7 Analisis dimensional.

Las dimensiones son propiedades inherentes a las cantidades medidas o calculadas, como el área, y no dependen de las unidades específicas en las que se expresan, como metros cuadrados, pies cuadrados, acres, etc. Se pueden establecer dimensiones fundamentales basadas en patrones de medición independientes, como la masa **(M)**, la longitud **(L)** y el tiempo **(T)**, que son cruciales en mecánica.

Una regla fundamental es que las ecuaciones deben ser dimensionalmente consistentes, es decir, las dimensiones de ambos lados de una ecuación deben coincidir. Esto ayuda a evitar errores al escribir ecuaciones. 

Por ejemplo, para una distancia $x$ recorrida en un tiempo $t$ bajo aceleración constante $a$, la ecuación correcta es $x = \frac{1}{2}at^2$, ya que las dimensiones concuerdan (aceleración tiene dimensiones de longitud dividido por tiempo al cuadrado, $L/T^2$).

$L = (x) = (\frac{1}{2}at^2) = (a) (t^2) = (L/T^2) (T^2) = \frac{L}{T^2} T^2 = L$

El análisis dimensional es una herramienta útil para trabajar con ecuaciones, permitiendo verificar la coherencia dimensional y evitar errores comunes, como confundir las fórmulas para el cálculo de distancias o tiempos en contextos físicos.

## 3-1 Vectores y escalares.

Los vectores son cantidades que tienen tanto magnitud como dirección, y son esenciales para representar diversas cantidades físicas como el desplazamiento, la velocidad, la fuerza, el campo eléctrico y el campo magnético. Se ejemplifica con el desplazamiento, explicando cómo un vector puede representar el cambio de posición de una partícula.

## 3-2 Suma de vectores.

Los vectores se pueden sumar gráficamente mediante el método del polígono o el método del paralelogramo. Se resalta que la suma de vectores es conmutativa y asociativa, y que la resta de vectores puede verse como la suma del vector negativo correspondiente. Además, se introduce el concepto de componentes de un vector, facilitando su suma y resta mediante cálculos algebraicos, lo que es especialmente útil en contextos más complejos donde la representación gráfica es impráctica.

## 3-3 Componentes de un vector.

Usando las notaciones $i$ y $j$ para representar las direcciones en los ejes $x$ y $y$, respectivamente. Esta notación ayuda a simplificar la representación y cálculo de vectores en dos dimensiones. Por ejemplo, un vector con componentes en los ejes $x$ y $y$ se puede expresar como $v = v_x i + v_y j$, donde $v_x$ y $v_y$ son las magnitudes de las componentes en cada eje.

El texto explica que la suma de las componentes no significa una adición aritmética convencional, sino que representa la combinación de las magnitudes en cada dirección. Además, se detalla cómo calcular el módulo (o magnitud) de un vector a partir de sus componentes, utilizando el teorema de Pitágoras. Por ejemplo, para un vector $v$ con componentes $v_x$ y $v_y$, el módulo se calcula como $|v| = \sqrt{v_x^2 + v_y^2}$.

En el contexto de vectores en el espacio, se introduce una tercera componente, $k$, para representar la dirección en el eje $z$, ampliando el concepto a tres dimensiones. Sin embargo, se aclara que este tema se menciona solo para ofrecer una visión general y que no se profundizará en él.

También se discute el concepto de vector posición $r$, que indica la ubicación de un punto en el espacio en relación con un origen de coordenadas. La posición se puede describir usando las componentes del vector en los ejes $x$, $y$ y, si es necesario, $z$.

Ejemplo:

Un vector tri-dimensional $v$ con componentes $v_x$, $v_y$ y $v_z$ se puede expresar como $v = v_x i + v_y j + v_z k$. El módulo de este vector se calcula como $|v| = \sqrt{v_x^2 + v_y^2 + v_z^2}$.

Cada componente representa la magnitud del vector en una dirección específica, y el módulo es la magnitud total del vector en el espacio.

Se pueden calcular de la siguiente manera:

- $ v_x = |v| \sin(\theta) \cos(\phi)$
- $ v_y = |v| \sin(\theta) \sin(\phi)$
- $ v_z = |v| \cos(\theta) $

## 3-4 Suma de Vectores, metodo de las componentes.

Este método implica descomponer cada vector en sus componentes a lo largo de los ejes de un sistema de coordenadas, generalmente el sistema de coordenadas cartesianas (x, y, z).

La suma de $ \vec{A} $ y $ \vec{B} $ se realiza sumando sus **componentes** correspondientes.

Este enfoque permite calcular la suma de dos o más vectores de manera más sistemática y es especialmente útil cuando los vectores no están alineados a lo largo de los mismos ejes o cuando se trabaja con múltiples vectores.

## 3-5 Multiplicacion de vectores.

La multiplicacion de vectores se puede realizar de dos maneras: el producto escalar y el producto vectorial.

El producto escalar, también conocido como producto punto, es una operación que toma dos vectores y devuelve un escalar. Se calcula multiplicando las magnitudes de los vectores y el coseno del ángulo entre ellos.

$ \vec{A} \cdot \vec{B} = |A| |B| \cos(\theta) $

El producto vectorial, también conocido como producto cruz, es una operación que toma dos vectores y devuelve un vector. Se calcula utilizando la regla de la mano derecha y proporciona un vector perpendicular al plano definido por los dos vectores originales.

$ |\vec{A} \times \vec{B}| = |A| |B| \sin(\theta)  $

Dado dos vectores, el producto vectorial proporciona un vector perpendicular al plano definido por los dos vectores originales.

$ \vec{A} \times \vec{B} = (a_yb_z - a_zb_y)i - (a_xb_z - a_zb_x)j + (a_xb_y - a_yb_x)k $
