# Ejercicio 4, pendulo simple. Analisis dimensional.

Considera un pendulo simple de longitud $L$ y masa $M$. Utilizando el analisis dimensional, determina la relacion entre el periodo (esto es, el tiempo que tarda el pendulo en completar un ciclo) y los parametros del problema (masa M, logitud L y aceleracion de la gravedad G).

El analisis dimensional nos dice que el periodo $T$ debe ser una funcion de la forma:

$
    f(M, L, G) = M^a L^b G^c K \\
$

- $[L] = L$
- $[M] = M$
- $[G] = L T^{-2}$

f es una funcion de tiempo, por lo que debe tener dimensiones de tiempo. Por lo tanto, $[f] = T$.

Por lo tanto, la ecuacion dimensional es:

$
    [f] = [M^a L^b G^c K] = [M]^a [L]^b [G]^c [K]       \\
    T = M^a L^b (L T^{-2})^c                            \\
    T = M^a L^{b + c} T^{-2c}                           \\
$

De aqui, obtenemos las siguientes ecuaciones:

$
    a = 0, \quad b + c = 0, \quad -2c = 1
$

De la primera ecuacion, obtenemos que $a = 0$. De la segunda ecuacion, obtenemos que $c = -b$. Sustituyendo esto en la tercera ecuacion, obtenemos que $c = -1/2$ y $b = 1/2$. Por lo tanto, el analisis dimensional nos dice que el periodo del pendulo simple es una funcion de la forma:

$
    T = k M^0 L^{1/2} G^{-1/2} = k L^{1/2} G^{-1/2} = k \sqrt{\frac{L}{G}} \\
$

