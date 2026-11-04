# Roadmap — Examen Física 1, Diciembre 2026

Basado en los 27 exámenes de `examenes/` (feb 2016 → feb 2025).

## Supuestos

- Examen a mediados de diciembre (históricamente entre el 14 y el 23). El plan arranca de cero el **jueves 05/11** y termina el **sábado 12/12**.
- Presupuesto (desde el 04/11): **2 h por día de lunes a viernes, 3 h el sábado. El domingo es libre.** El reparto con Arquitectura de Computadoras está acordado con la sesión que planifica Arqcom y es igual todas las semanas:

| Física 1 | Arqcom |
|---|---|
| Mar, Jue, Sáb | Lun, Mié, Vie |

- Son 17 sesiones: 11 de 2 h (mar/jue) y 6 de 3 h (sáb), ≈ 40 h.
- **Pendiente:** si el examen de Arqcom cae antes (por ejemplo, alrededor del 13/12), Arqcom se queda con los días de Física del 07–12/12. Física recupera todos los días entre ese examen y el suyo. Hay que ajustar cuando salgan las fechas.
- Temas 1–6 ya están trabajados en el repo. Temas 7–13 se vieron, pero la base está floja, así que el plan les da la mayor parte del tiempo.

## Cómo es el examen

- 10 preguntas múltiple opción, 5 opciones, 3 h (≈ 18 min por pregunta).
- +10 si es correcta, −2.5 si es incorrecta, 0 en blanco. **Se aprueba con 50.**
- Te dan los momentos de inercia (barra, disco, esfera, aro), así que no hace falta memorizarlos.
- El orden de los temas es casi fijo desde 2016:

| Pregunta | Tema típico | Temas del repo | Por examen |
|---|---|---|---|
| 1–2 | Cinemática: tiro oblicuo / encuentro, movimiento relativo | 2, 3 | ~2 |
| 3–4 | Dinámica: poleas, rozamiento, movimiento circular | 4, 5 | ~2 |
| 5 | Energía (resorte + rozamiento + rizo), potencia | 6, 7 | ~1 |
| 5–6 | Choques, explosiones, centro de masa | 8 | ~1 |
| 6–9 | Rígido: rodadura, estática, momento angular | 9–12 | ~3–4 |
| 10 | Oscilaciones | 13 | ~1 (siempre) |

## Estrategia para llegar a 50

- Responder al azar entre 5 opciones vale 0 en promedio. **Si podés descartar al menos una opción, conviene responder** (+0.6 en promedio). Si no, dejala en blanco.
- Usá análisis dimensional y casos límite para descartar opciones en las preguntas simbólicas.
- Objetivo: **asegurar 7 preguntas**.
  - P1–P4: lo que ya estudiaste.
  - P10 (oscilaciones): casi siempre sale con fórmula. Si ω² = k_ef / m_ef y el disco rueda, m_ef = 3m/2.
  - Choques.
  - Una de estática o de rodadura.
- Con 6 bien y 4 mal ya llegás a 50.

## Formato de sesión

- **Mar/Jue (2 h):** 10–15 min de formulario o teoría del tema (Resnick, según las secciones del `summary.md` de cada tema). Después, 5–6 problemas cronometrados a ~18 min cada uno.
- **Sáb (3 h):** un simulacro completo en condiciones de examen, o una tanda de 7–8 problemas + re-hacer lo marcado ✗.
- Corregí con la tabla de respuestas al final de cada PDF (Versión 1).
- Si un problema no sale en 25 min, mirá la solución, anotá **qué idea faltaba** y marcalo ✗ para re-hacerlo después.
- Los simulacros se hacen sin apuntes y con el reloj corriendo.
- **Reservados para simulacros:** Feb 2022, Jul 2022, Dic 2023, Jul 2023, Feb 2024, Jul 2024 y Feb 2025 (ej. 7–10). Todo lo demás es banco de práctica.

## Calendario

Código de problemas: ver el [banco](#banco-de-problemas-por-tema) (`D19-7` = Diciembre 2019, ejercicio 7).

### Semana del 02/11 — Repaso de P1–P2
- [ ] **Jue 05/11** · Cinemática: tiro oblicuo, movimiento relativo, circular · F16-1, D19-1, D16-2, F19-3, J17-3, D18-7
- [ ] **Sáb 07/11** · Dinámica: poleas, rozamiento, dinámica circular · D18-3, D21-4, J18-3, D19-3, F19-1, D16-4, J19-2

### Semana del 09/11 — Energía, choques y primer medio simulacro
- [ ] **Mar 10/11** · Energía (resorte + rozamiento + rizo) y potencia · D16-5, F18-4, A20-5, J20-5, F21-2, D20-9
- [ ] **Jue 12/11** · Choques, explosiones, desplazamiento del CM · F17-2, F18-5, D18-5, A20-4, D21-5, D17-6
- [ ] **Sáb 14/11** · **Medio simulacro:** Feb 2022 ej. 1–5 (90 min) + corrección. Después, teoría del rígido (Resnick caps. 11–12: I, Steiner, τ = Iα) · J16-1, F18-7 · puntaje: ___/50

### Semana del 16/11 — Rígido (temas 9–11)
- [ ] **Mar 17/11** · τ = Iα + rodadura: dinámica y fuerza aplicada · J17-2, F18-3, F17-5, F16-10, D19-7, D20-7
- [ ] **Jue 19/11** · Rodadura: energía (yo-yo, plano inclinado) + paso de deslizar a rodar · D16-8, F17-8, D19-9, J16-4, J18-8, F20-8
- [ ] **Sáb 21/11** · Conservación de L (teoría: Resnick cap. 14) + choque contra barra pivoteada · F16-9, J17-7, D17-9, D19-8, D16-7, F17-10, D18-6, A20-8

### Semana del 23/11 — Estática, oscilaciones y primer simulacro completo
- [ ] **Mar 24/11** · Estática (teoría: Resnick caps. 9–10, según el `summary.md` del tema 12) · F16-8, J17-6, D17-5, J18-4, F18-10, D19-6
- [ ] **Jue 26/11** · Oscilaciones: MAS, disco rodando con resorte, péndulo físico · D17-4, D19-10, F16-7, D18-10, D16-10, F20-10
- [ ] **Sáb 28/11** · **Simulacro completo:** Feb 2024 · puntaje: ___/100

### Semana del 30/11 — Corrección + segundo simulacro
- [ ] **Mar 01/12** · Corregir Feb 2024 + re-hacer lo marcado ✗ + rígido mixto · D21-6, A20-10
- [ ] **Jue 03/12** · Feb 2025 ej. 7–10 (completa el examen que ya empezaste en el repo) + re-hacer lo marcado ✗
- [ ] **Sáb 05/12** · **Simulacro completo:** Dic 2023 · puntaje: ___/100

### Semana del 07/12 — Cierre (*sujeto a la fecha de Arqcom*)
- [ ] **Mar 08/12** · Corregir Dic 2023 + re-hacer lo marcado ✗
- [ ] **Jue 10/12** · **Medio simulacro:** Jul 2024 ej. 6–10 (90 min, la mitad de rígido) + corrección · puntaje: ___/50
- [ ] **Sáb 12/12** · Liviano: formulario y los 2–3 tipos de problema más flojos. Nada nuevo.

**Si sobra tiempo** (o Física gana días después del examen de Arqcom): Jul 2023 completo, Jul 2022 completo, Feb 2022 ej. 6–10, y el resto del banco del tema más flojo.

## Banco de problemas por tema

Código: `F` = febrero, `J` = julio, `D` = diciembre, `A` = agosto, seguido de año y número de ejercicio. Por ejemplo, `D19-7` = Diciembre 2019, ejercicio 7.

**Cinemática**
- Tiro oblicuo / encuentro: F16-1, D16-1, F17-1, J17-1, D17-1, D18-1, J18-2, D19-1, F20-1, J20-1, A20-1, D20-1, D21-1, J21-7, F24-1, J24-1, J24-2, F25-1, F25-2
- Movimiento relativo: D16-2, F16-2, F17-9, D18-2, F19-3, D21-2, J21-4, F22-2, J22-2, D23-4, J23-3, F24-3, J24-3
- Movimiento circular / cinemática angular: J17-3, D18-7, F21-7, J21-6, J22-3, J23-5, F24-2

**Dinámica de la partícula**
- Poleas y vínculos de cuerda: D16-3, D18-3, D18-9, J19-2, F20-3, F20-4, D20-3, D21-3, D21-4, J22-4, J23-4, F24-4, F25-3
- Rozamiento / rango de equilibrio: J16-5, F17-7, D17-2, D18-4, J18-3, D19-2, D19-3, J20-2, J20-3, D20-4, F21-4, J24-4, F25-4
- Dinámica circular (peralte, cono, plataforma): F16-3, D16-4, J16-8, F17-3, J17-4, F19-1, J19-4, A20-2, A20-3, F22-4

**Energía**
- Resorte + rozamiento + rizo: D16-5, F18-4, J20-5, A20-5, A20-6, D20-5, F21-2, F21-3, J21-10, F22-3, D23-3
- Potencia: J16-9, J17-5, D20-9, F21-5

**Choques y sistemas de partículas**
- Choques y explosiones: D16-6, F17-2, F18-5, D18-5, J18-1, F20-2, F20-6, J20-6, A20-4, D20-2, D20-6, F21-1, J21-1, D21-5, F22-5, J22-5, D23-5, F24-6, J24-5, F25-5
- Desplazamiento del CM (bote, vagón): F16-4, D17-6, F19-2, J20-4, D19-5

**Rígido**
- Momento de inercia: J16-1, F18-7
- Rodadura (dinámica y energía): D16-8, F16-10, F17-5, F17-6, F17-8, J17-10, D17-7, F18-6, J18-6, J18-9, J19-6, D19-7, D19-9, A20-7, D20-7, F21-9, D21-6, D21-7, F22-7, F22-8, J22-7, J23-6, D23-7, D23-8, F24-9, J24-6, J24-7
- Paso de deslizar a rodar: J16-4, J18-8, F19-6, F20-8, J20-7, F21-10, F25-8
- Momento angular: F16-9, J17-7, D17-9, D17-10, F19-8, F19-9, D19-8, F20-9, J20-9, D21-9, F22-9, J22-8, J23-7, J23-8, D23-9, F24-8
- Choque contra barra pivoteada: D16-7, J16-3, F17-10, D18-6, J19-10, A20-8, D20-8, F21-6, J24-8, F25-9
- Estática: F16-8, J16-7, J17-6, D17-5, F18-10, J18-4, J19-9, D19-6, F20-5, A20-9, J21-3, D21-8, F22-6, J22-9, J23-9, D23-6, F24-7, J24-9, F25-6

**Oscilaciones**
- Disco que rueda con resorte: F16-7, D18-10, A20-10, D20-10, J21-8, J23-10, D23-10, J24-10
- Péndulo físico: D16-10, J16-2, J17-8, F19-7, F20-10, J20-10, D21-10, J22-10, F25-10
- Resortes y poleas / MAS: D17-4, F18-8, J18-5, F19-5, D19-10, J21-5, F21-8, F22-10, F24-10

## Notas

- `examenes/examenes_resueltos_2013-2021.pdf` es un escaneo. No se puede buscar texto, pero se puede leer.
- `examenes/resumen_examenes_resueltos_2017-2021.pdf` sirve como formulario.
- La numeración por tema sale del orden de cada PDF, y puede variar entre versiones del examen. La tabla de respuestas que se usa es la de la **Versión 1**.
