# Banco de Preguntas — Práctica Adicional (Unidades 1 y 2)

*Estadística para Economistas · Repo: Cam_Est1*
*Pensado como práctica adicional tras la Guía 01 (nota 09) — mismos temas, datos nuevos.*

## Cómo usarlo

Resuelve primero **sin mirar la clave**. Al final del documento está la clave de respuestas,
solo con los resultados finales (no el procedimiento) — así puedes autoevaluarte con
honestidad. Si algo no te cuadra, revisa el bloque correspondiente en la
*Clase de Reforzamiento* antes de ver el procedimiento completo.

---

## Bloque I — Verdadero o Falso (20 preguntas)

1. Un estudio que recolecta datos de una parte representativa de la población (no de toda
   ella) se llama censo.
2. El conjunto de todos los estudiantes matriculados en una universidad en un semestre
   específico es un ejemplo de población finita.
3. La mediana es más sensible a valores atípicos que la media.
4. Para datos muestrales, la varianza se calcula dividiendo la suma de cuadrados entre $n$.
5. La moda es el valor que divide a los datos ordenados en dos partes iguales.
6. En una distribución simétrica, se cumple que $\gamma_1 = 0$.
7. Una distribución platicúrtica tiene colas más gruesas que la distribución normal.
8. En el Índice de Gini, $G=1$ representa la máxima desigualdad posible.
9. La escala ordinal permite sumar y restar las categorías, además de ordenarlas.
10. El Coeficiente de Variación es útil para comparar la dispersión de dos grupos con medias
    muy distintas.
11. Para datos positivos, siempre se cumple que la media armónica es menor o igual que la
    media geométrica.
12. La curtosis mide qué tan simétrica es una distribución.
13. Comparado con el rango, el rango intercuartílico (IQR) es más sensible a valores atípicos.
14. Un censo recolecta datos de una muestra representativa, no de toda la población.
15. "Marca del carro" (Toyota, Kia, Hyundai, etc.) es un ejemplo de variable cuantitativa
    discreta.
16. Para datos positivos, se cumple $H \le G \le \bar{x}$.
17. Si en una distribución se cumple $\bar{x} < \tilde{x} < Mo$, la distribución tiene sesgo
    negativo.
18. El CV permite comparar la dispersión relativa entre datos con unidades distintas (por
    ejemplo, soles vs. dólares).
19. La Curva de Lorenz es la base gráfica para construir el Índice de Gini.
20. La moda de un conjunto de datos siempre es un valor único.

---

## Bloque II — Desarrollo y resolución de casos

**Pregunta 21 — Media, mediana, moda y tipo de asimetría**
Datos (n=8, soles): 1400, 1700, 1900, 2100, 2300, 2600, 3100, 11000.
Calcula media, mediana y moda, y determina el tipo de asimetría.

**Pregunta 22 — Varianza y desviación estándar muestral**
Datos: 7, 10, 8, 6, 9. Calcula $s^2$ y $s$.

**Pregunta 23 — Transformación lineal $Y = 0.8X - 5$**
Si $\bar{x}=60$ y $s_x^2=225$, calcula $\bar{y}$ y $s_y^2$.

**Pregunta 24 — Coeficiente de asimetría de Fisher**
Datos: 3, 5, 6, 9, 14, 20. Calcula $\gamma_1$ e interpreta el resultado.

**Pregunta 25 — Coeficiente de Variación comparado**
Grupo A: $\bar{x}=80$, $s=12$. Grupo B: $\bar{x}=45$, $s=9$. ¿Cuál tiene mayor dispersión
relativa?

**Pregunta 26 — Datos agrupados en intervalos** *(material del libro)*
Ingreso mensual de 50 personas (soles):

| Intervalo | $n_i$ |
|---|---|
| 1000–1400 | 6 |
| 1400–1800 | 14 |
| 1800–2200 | 18 |
| 2200–2600 | 9 |
| 2600–3000 | 3 |

Calcula la marca de clase de cada intervalo, la media y la varianza.

**Pregunta 27 — Curtosis**
Datos: 2, 3, 4, 5, 6, 25. Calcula $\gamma_2$ e indica si la distribución es leptocúrtica,
platicúrtica o normal.

**Pregunta 28 — Cuartiles y rango intercuartílico** *(material del libro)*
Datos ordenados (n=9): 8, 10, 12, 14, 15, 18, 20, 24, 60. Calcula $Q_1$, $Q_3$, IQR y
compáralo con el rango total.

**Pregunta 29 — Índice de Gini con datos agrupados**
5 grupos con proporciones acumuladas: $P_i$ = 0.2, 0.4, 0.6, 0.8, 1.0 y
$Q_i$ = 0.05, 0.15, 0.30, 0.55, 1.00. Calcula $G$ usando el método trapezoidal e interprétalo.

**Pregunta 30 — Tipos de variable y escalas de medición**
Clasifica cada variable (nominal / ordinal / intervalo / razón):
(a) Tipo de sangre — (b) Posición final en una carrera (1°, 2°, 3°...) — (c) Año calendario —
(d) Distancia recorrida en km.

---

## Bloque III — Caso Práctico Integrador

**Pregunta 31 — Caso Integrador**
Ingreso mensual de 10 hogares (soles), ordenados:
1600, 1900, 2100, 2400, 2600, 2900, 3200, 3600, 4200, 9800.

1. Calcula media, mediana, moda y determina el tipo de asimetría.
2. Calcula varianza, desviación estándar y Coeficiente de Variación. Interpreta el CV
   obtenido.
3. Calcula $Q_1$, $Q_3$ e IQR. Compáralo con el rango total.
4. Calcula el Índice de Gini (usando las proporciones acumuladas de población e ingreso, con
   el método trapezoidal) e interpreta el resultado.
5. Explica qué tan sensibles son las medidas calculadas ante el valor atípico de 9800, y qué
   medida recomendarías usar para resumir el ingreso típico de estos hogares.

---

## Clave de respuestas (solo resultados finales)

**Bloque I (V/F):**
1-F · 2-V · 3-F · 4-F · 5-F · 6-V · 7-F · 8-V · 9-F · 10-V ·
11-V · 12-F · 13-F · 14-F · 15-F · 16-V · 17-V · 18-V · 19-V · 20-F

**Bloque II:**
- 21: Media = 3262.5, Mediana = 2200, Moda = no tiene → sesgo positivo.
- 22: $s^2 = 2.5$, $s \approx 1.58$.
- 23: $\bar{y} = 43$, $s_y^2 = 144$.
- 24: $\gamma_1 \approx 0.70$ → sesgo positivo moderado.
- 25: $CV_A = 15\%$, $CV_B = 20\%$ → Grupo B tiene mayor dispersión relativa.
- 26: Marcas: 1200, 1600, 2000, 2400, 2800. Media = 1912. Varianza = 181 056
  ($s \approx 425.5$).
- 27: $\gamma_2 \approx 1.01$ → leptocúrtica.
- 28: $Q_1 = 11$, $Q_3 = 22$, IQR = 11 (rango total = 52, mucho más afectado por el 60).
- 29: $G \approx 0.38$ → desigualdad moderada-alta.
- 30: (a) nominal, (b) ordinal, (c) intervalo, (d) razón.

**Bloque III (Pregunta 31):**
1. Media = 3430, Mediana = 2750, Moda = no tiene → sesgo positivo (por el 9800).
2. $s^2 \approx 5\,637\,889$, $s \approx 2374.4$, $CV \approx 69.2\%$ (dispersión relativa muy
   alta).
3. $Q_1 = 2100$, $Q_3 = 3600$, IQR = 1500 (rango total = 8200, mucho más distorsionado).
4. $G \approx 0.29$ → desigualdad moderada, explicada en gran parte por el hogar de 9800.
5. Media, varianza, $s$ y CV son muy sensibles al 9800; mediana e IQR son robustas. Se
   recomienda la mediana para resumir el ingreso típico.

---

*Fuentes: mismos temas y fórmulas que la Guía 01 — Clase 01 y Clase 02 (Wilfredo Bacilio
Alarcón) para los bloques con datos individuales; Libro base §2.2.2 y §3.1.5/§3.2.1 para
datos agrupados y cuartiles (preguntas 26 y 28, marcadas explícitamente); método trapezoidal
para el Gini con datos agrupados (preguntas 29 y 31.4) explicado en la Clase de Reforzamiento,
ya que no está desarrollado en ningún material original del curso.*
