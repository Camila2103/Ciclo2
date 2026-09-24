# Clase de Reforzamiento — Conceptos Previos y Medidas Características de una Distribución

*Basada en el desempeño en la Guía 01 (nota 09) · Estadística para Economistas · Repo: Cam_Est1*

---

## Cómo usar esta clase

Esta no es una clase nueva: es un **repaso dirigido** a los temas donde la Guía 01 mostró
dificultad. Cada bloque tiene: (1) el recordatorio teórico con la notación de Clase 01/02,
(2) un ejemplo resuelto paso a paso con números **distintos** a los de la guía (para que no
sea memorizar la respuesta), y (3) un mini-ejercicio para practicar sola, con la respuesta al
final del documento.

Dos bloques (E y F) tratan temas que **no aparecen en las diapositivas del profesor**, solo en
el libro base — se marcan explícitamente como *"Material del libro"* porque fue justamente ahí
donde la Guía 01 detectó los mayores vacíos.

---

## A. Sensibilidad y robustez de las medidas ante valores atípicos

**Recordatorio (Clase 02, tablas comparativas):**

| Medida | Sensibilidad a outliers |
|---|---|
| Media $\bar{x}$ | Alta |
| Mediana $\tilde{x}$ | Baja |
| Moda | Moderada |
| Rango | Alta |
| Varianza / Desv. estándar | Alta |
| Coeficiente de Variación | Moderada |
| Índice de Gini | Relativamente robusto |

La idea clave: una medida es **robusta** cuando casi no cambia si quitas o modificas un dato
extremo. La mediana y el IQR (bloque F) son las más robustas porque dependen del **orden**
de los datos, no de su magnitud exacta.

**Ejemplo resuelto:**

Sueldos de 6 trabajadores (en soles): 1500, 1600, 1700, 1800, 1900, 9000.

- Media = $\frac{1500+1600+1700+1800+1900+9000}{6} = \frac{17\,500}{6} \approx 2916.7$
- Mediana = promedio del 3.º y 4.º dato ordenados = $\frac{1700+1800}{2} = 1750$

La media (2916.7) está muy por encima de casi todos los datos individuales — el sueldo de
9000 la "jala" hacia arriba. La mediana (1750) sí refleja el sueldo típico del grupo.
**Conclusión:** con outliers, la mediana es más representativa que la media.

**Practica tú:** Datos: 10, 12, 11, 13, 60. Calcula media y mediana, y di cuál representa
mejor al grupo. *(Respuesta al final, Ejercicio A)*

---

## B. Media, mediana, moda y tipo de asimetría

**Recordatorio (Clase 02):** cuando la distribución NO es simétrica, la posición relativa de
media, mediana y moda indica el tipo de sesgo:

- $\bar{x} > \tilde{x}$ → **sesgo positivo** (cola a la derecha, causada por valores altos atípicos)
- $\bar{x} < \tilde{x}$ → **sesgo negativo** (cola a la izquierda, causada por valores bajos atípicos)
- $\bar{x} = \tilde{x} = Mo$ → distribución simétrica

Este fue el patrón exacto de las preguntas 21 y 31 de la guía — vale la pena dominarlo.

**Ejemplo resuelto** (n = 7): 5, 8, 9, 10, 11, 12, 40

- Media = $\frac{95}{7} \approx 13.57$
- Mediana (dato central, posición 4) = 10
- Moda = no tiene (todos distintos)
- Como $\bar{x}(13.57) > \tilde{x}(10)$ → **sesgo positivo**, causado por el valor atípico 40.

**Practica tú:** Datos (n=7): 2, 4, 5, 6, 7, 8, 9. ¿Qué tipo de simetría tiene? Ahora cambia el
último dato por 50 y vuelve a calcular. ¿Cambió el tipo de sesgo? *(Ejercicio B)*

---

## C. Varianza, desviación estándar y transformaciones lineales

**Recordatorio (Clase 02):**

$$s^2 = \frac{1}{n-1}\sum_{i=1}^n (x_i-\bar{x})^2 \qquad s = \sqrt{s^2}$$

⚠️ El error más común (pregunta 4 de la guía, marcada F): usar $n$ en vez de $n-1$ en datos
**muestrales**. El $n-1$ es la corrección de Bessel — solo se usa $n$ cuando trabajas con la
**población completa** ($\sigma^2$).

**Propiedades ante transformaciones $Y = aX + b$** (clave para la pregunta 23 de la guía):

- Media nueva: $\bar{y} = a\bar{x} + b$
- Varianza nueva: $s_y^2 = a^2 s_x^2$ (el cambio de origen $b$ **no** afecta la varianza; el
  factor de escala $a$ se eleva al cuadrado)

**Ejemplo resuelto:** Si $\bar{x} = 40$ y $s_x^2 = 64$, y se aplica $Y = 2X - 5$:

- $\bar{y} = 2(40) - 5 = 75$
- $s_y^2 = 2^2 \times 64 = 256$, entonces $s_y = 16$

**Practica tú:** Datos: 2, 4, 6, 8, 10. Calcula $\bar{x}$ y $s^2$. Luego aplica $Y = 3X + 1$ y
encuentra $\bar{y}$ y $s_y^2$ usando las propiedades (sin recalcular todo desde cero).
*(Ejercicio C)*

---

## D. Coeficiente de asimetría de Fisher ($\gamma_1$) y curtosis ($\gamma_2$)

**Recordatorio (Clase 02):**

$$\gamma_1 = \dfrac{\frac{1}{n}\sum (x_i-\bar{x})^3}{\left(\frac{1}{n}\sum (x_i-\bar{x})^2\right)^{3/2}} \qquad
\gamma_2 = \dfrac{\frac{1}{n}\sum (x_i-\bar{x})^4}{\left(\frac{1}{n}\sum (x_i-\bar{x})^2\right)^{2}} - 3$$

Interpretación (memorizar en pares, así se pregunta en V/F):

| $\gamma_1$ | Significa | | $\gamma_2$ | Significa |
|---|---|---|---|---|
| $=0$ | simétrica | | $=0$ | curtosis normal |
| $>0$ | sesgo positivo (derecha) | | $>0$ | **leptocúrtica** → pico alto, colas **más gruesas** |
| $<0$ | sesgo negativo (izquierda) | | $<0$ | **platicúrtica** → pico bajo, colas **más delgadas** |

⚠️ Es fácil confundir leptocúrtica/platicúrtica (pregunta 7 de la guía, marcada F por esto
exactamente). Truco mnemotécnico: "lepto" suena a algo alto y afilado → pico alto, colas gordas.

**Ejemplo resuelto:** Datos: 1, 2, 3, 4, 15 → $\bar{x} = 5$

- Desviaciones: $-4,-3,-2,-1,10$
- $\sum(x_i-\bar{x})^2 = 16+9+4+1+100 = 130$ → $m_2 = 130/5 = 26$
- $\sum(x_i-\bar{x})^3 = -64-27-8-1+1000 = 900$ → $m_3 = 900/5 = 180$
- $\gamma_1 = \dfrac{180}{26^{3/2}} = \dfrac{180}{132.66} \approx 1.36$ → sesgo positivo fuerte
  (coherente con el dato atípico 15).

**Practica tú:** Con los mismos datos (1, 2, 3, 4, 15), calcula $\gamma_2$ (necesitas
$\sum(x_i-\bar{x})^4$) e interpreta si la distribución es leptocúrtica o platicúrtica.
*(Ejercicio D)*

---

## E. Coeficiente de Variación (CV) para comparar dispersión relativa

**Recordatorio (Clase 02):** $CV = \dfrac{s}{\bar{x}} \times 100$. Sirve quando quieres comparar
la dispersión de dos grupos con **medias distintas o unidades distintas** — la desviación
estándar sola no permite esa comparación directa.

**Ejemplo resuelto:** Dos secciones rinden un examen.
Sección A: $\bar{x}=14$, $s=2$. Sección B: $\bar{x}=11$, $s=2$.

- $CV_A = 2/14 \times 100 \approx 14.3\%$
- $CV_B = 2/11 \times 100 \approx 18.2\%$

Aunque ambas tienen la MISMA desviación estándar, la Sección B tiene mayor dispersión
**relativa** (sus notas varían más en proporción a su propio promedio, que es más bajo).

**Practica tú:** Grupo X: $\bar{x}=200$, $s=20$. Grupo Y: $\bar{x}=50$, $s=8$. ¿Cuál tiene
mayor dispersión relativa? *(Ejercicio E)*

---

## F. Datos agrupados en intervalos — *Material del libro (no está en las diapositivas)*

Este es uno de los dos temas que la Guía 01 señaló como no cubierto en clase (afectó la
pregunta 26). Viene del libro base, §2.2.2.

**Idea:** cuando hay muchos valores distintos, se agrupan en intervalos de clase. A cada
intervalo se le asigna una **marca de clase** $c_i$ = punto medio del intervalo, y se trabaja
como si todos los datos de ese intervalo valieran $c_i$.

$$\bar{x} = \frac{\sum f_i \, c_i}{N} \qquad s^2 = \frac{\sum f_i (c_i - \bar{x})^2}{N}$$

**Ejemplo resuelto:** Edades de 40 personas agrupadas:

| Intervalo | $f_i$ | Marca $c_i$ | $f_i c_i$ |
|---|---|---|---|
| 10–20 | 8 | 15 | 120 |
| 20–30 | 15 | 25 | 375 |
| 30–40 | 12 | 35 | 420 |
| 40–50 | 5 | 45 | 225 |
| **Total** | **40** | | **1140** |

- $\bar{x} = 1140/40 = 28.5$
- $s^2 = \dfrac{8(15-28.5)^2+15(25-28.5)^2+12(35-28.5)^2+5(45-28.5)^2}{40}$
  $= \dfrac{8(182.25)+15(12.25)+12(42.25)+5(272.25)}{40} = \dfrac{1458+183.75+507+1361.25}{40}
  = \dfrac{3510}{40} = 87.75$

**Practica tú:** Con esta misma tabla, calcula la desviación estándar $s$ y el coeficiente de
variación $CV$. *(Ejercicio F)*

---

## G. Cuartiles y rango intercuartílico (IQR) — *Material del libro (no está en las diapositivas)*

El segundo tema que la guía marcó como faltante (afectó la pregunta 31.3). Libro §3.1.5 y §3.2.1.

**Idea:** los cuartiles generalizan la mediana — dividen los datos ordenados en 4 partes
iguales. $Q_2$ = mediana. Con datos individuales (no agrupados), se calcula igual que la
mediana pero usando $N/4$ y $3N/4$ en vez de $N/2$.

$$IQR = Q_3 - Q_1$$

El IQR es **robusto**: representa el 50% central de los datos y no se ve afectado por
valores extremos, a diferencia del rango total.

**Ejemplo resuelto:** Datos ordenados (n=8): 12, 15, 18, 20, 22, 25, 28, 90

- Mitad inferior (4 datos): 12,15,18,20 → $Q_1$ = mediana de estos = $(15+18)/2 = 16.5$
- Mitad superior (4 datos): 22,25,28,90 → $Q_3$ = mediana de estos = $(25+28)/2 = 26.5$
- $IQR = 26.5 - 16.5 = 10$

Compárese con el rango total: $90-12=78$. El IQR (10) muestra que, quitando el 25% más alto
y más bajo, los datos centrales están mucho menos dispersos — el 90 es un outlier que infla
el rango pero casi no afecta al IQR.

**Practica tú:** Datos ordenados (n=10): 5,6,7,8,9,10,11,12,13,50. Calcula $Q_1$, $Q_3$ e IQR.
Compáralo con el rango total y explica qué te dice eso. *(Ejercicio G)*

---

## H. Curva de Lorenz e Índice de Gini — el método correcto con datos agrupados

Este fue el tema **más problemático** de la guía (preguntas 27 y 31.4): la fórmula
$G = 1-2\sum(P_i \cdot Q_i)$ tal como aparece literalmente en la diapositiva **da un resultado
inválido** si se aplica directo a proporciones acumuladas agrupadas — puede salir fuera del
rango $[0,1]$. Ni la clase ni el libro explican el ajuste necesario, así que aquí se explica
paso a paso.

**El ajuste correcto — método trapezoidal:** cuando $P_i$ y $Q_i$ son proporciones
**acumuladas** (no valores individuales), hay que promediar cada $Q_i$ con el $Q_{i-1}$
anterior antes de multiplicar por el incremento de $P_i$:

$$G = 1 - \sum_{i=1}^{k} (Q_i + Q_{i-1})(P_i - P_{i-1}), \qquad P_0 = Q_0 = 0$$

Esta es la fórmula del **área bajo la curva de Lorenz calculada por trapecios**: en vez de
sumar rectángulos ($P_i \cdot Q_i$), se suma el área de cada trapecio entre dos puntos
consecutivos de la curva — por eso el resultado sí queda entre 0 y 1.

**Ejemplo resuelto:** 4 grupos de hogares (ordenados de menor a mayor ingreso), con
proporciones acumuladas de población $P_i$ y de ingreso $Q_i$:

| Grupo | $P_i$ | $Q_i$ | $Q_i+Q_{i-1}$ | $P_i-P_{i-1}$ | Producto |
|---|---|---|---|---|---|
| 1 | 0.25 | 0.10 | 0.10 | 0.25 | 0.0250 |
| 2 | 0.50 | 0.25 | 0.35 | 0.25 | 0.0875 |
| 3 | 0.75 | 0.45 | 0.70 | 0.25 | 0.1750 |
| 4 | 1.00 | 1.00 | 1.45 | 0.25 | 0.3625 |

$\sum = 0.0250+0.0875+0.1750+0.3625 = 0.6500$

$G = 1 - 0.65 = 0.35$

Interpretación: un Gini de 0.35 indica una desigualdad **moderada** en el ingreso de estos
hogares (recuerda: G=0 es igualdad perfecta, G=1 es desigualdad máxima).

**Practica tú:** 3 grupos con $P_i$ = 0.33, 0.67, 1.00 y $Q_i$ = 0.15, 0.40, 1.00. Calcula G
con el método trapezoidal e interprétalo. *(Ejercicio H)*

---

## I. Escalas de medición

**Recordatorio (Clase 01):**

| Escala | Permite | Ejemplo |
|---|---|---|
| Nominal | Solo categorizar, sin orden | Color de ojos |
| Ordinal | Categorizar **con orden**, pero sin sumar/restar | Nivel de satisfacción |
| De intervalo | Sumar/restar, sin cero absoluto | Temperatura en °C |
| De razón | Todas las operaciones, con cero absoluto | Peso, ingreso, altura |

⚠️ Error típico (pregunta 9 de la guía): pensar que la escala ordinal admite sumar o restar
categorías. No — ordinal solo dice "A es mayor que B", nunca "A menos B = tanto".

**Practica tú:** Clasifica (nominal/ordinal/intervalo/razón): (a) número de hijos, (b) medalla
obtenida (oro/plata/bronce), (c) año de nacimiento, (d) tiempo en segundos de una carrera.
*(Ejercicio I)*

---

## Respuestas a los ejercicios de práctica

- **A:** Media = 21.2, Mediana = 12. La mediana representa mejor al grupo (el 60 es outlier).
- **B:** Original: simétrica ($\bar{x}=\tilde{x}=6$). Con 50 en vez de 9: media sube a ~11.4,
  mediana sigue en 6 → aparece sesgo positivo.
- **C:** $\bar{x}=6$, $s^2=10$. Con $Y=3X+1$: $\bar{y}=3(6)+1=19$, $s_y^2=3^2(10)=90$.
- **D:** $\sum(x_i-\bar{x})^4 = 256+81+16+1+10000=10354$ → $m_4=2070.8$;
  $\gamma_2 = 2070.8/26^2 - 3 = 2070.8/676-3 \approx 3.06-3=0.06$ → prácticamente normal
  (muy ligeramente leptocúrtica).
- **E:** $CV_X=10\%$, $CV_Y=16\%$ → Grupo Y tiene mayor dispersión relativa.
- **F:** $s=\sqrt{87.75}\approx 9.37$; $CV = 9.37/28.5\times100\approx 32.9\%$.
- **G:** $Q_1=7$, $Q_3=12$, $IQR=5$. Rango total $=45$. El IQR muestra que el 50% central
  está poco disperso; el 50 es un outlier que infla mucho el rango pero casi no afecta al IQR.
- **H:** $\sum=0.15(0.33)+0.55(0.34)+1.40(0.33)=0.0495+0.187+0.462=0.6985$ → $G\approx0.30$,
  desigualdad moderada.
- **I:** (a) razón, (b) ordinal, (c) intervalo, (d) razón.

---

*Fuentes: Clase 01 (conceptos generales, escalas de medición), Clase 02 (medidas de
centralización, dispersión, forma y concentración) — Wilfredo Bacilio Alarcón, Estadística
para Economistas. Bloques F y G: Libro base, §2.2.2 y §3.1.5/§3.2.1. Bloque H: método
trapezoidal explicado como complemento, no aparece explícitamente en ninguna de las dos
fuentes del curso.*
