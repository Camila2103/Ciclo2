# Práctica 02

## Enunciado

**Estadística para Economistas I — Práctica de Ejercicios**
Universidad Nacional Mayor de San Marcos — Facultad de Ciencias Económicas
**PRÁCTICA: TEORÍA DE CONJUNTOS Y LEYES DE PROBABILIDAD**
Profesor: MSc. Wilfredo Bacilio Alarcón · Curso: Estadística para Economistas I · Ciclo: 2026-II

### Instrucciones

Lea cuidadosamente cada bloque. En el Bloque I, si la afirmación es verdadera escriba V; si
es falsa escriba F y justifique brevemente. En los Bloques II y III, realice los cálculos
necesarios en su hoja de desarrollo y marque con un círculo la alternativa correcta.

> ⚠️ **Fuentes**: las preguntas 1–8, 17–20, 21–24 y el ítem 1 del caso integrador se basan en
> `clases/03. ConjuntosProbabilidades.pdf` (conjuntos, espacio muestral, axiomas de Kolmogorov
> y propiedades derivadas). Las preguntas 9–16, 25–30 y los ítems 2–4 del caso integrador son
> **material del libro base** (`LibroBase-STATS1-Estadística Básica.pdf`, Cap. 5 §5.3–§5.4:
> probabilidad condicionada, independencia, Teorema de la Probabilidad Total, Teorema de Bayes
> y análisis combinatorio), **no visto en las diapositivas de clase**. Verifica con el profesor
> si estos subtemas serán parte de su programación antes de tomarlos como examinables.

---

## Bloque I: Verdadero o Falso (20 puntos)

Instrucciones: Lea cuidadosamente cada afirmación. Si es verdadera, escriba V; si es falsa,
escriba F. Justifique brevemente su respuesta.

1. Un experimento aleatorio es aquel cuyo resultado no puede predecirse con certeza, aunque
   se conoce el conjunto de resultados posibles.
2. El espacio muestral $\Omega$ es siempre un conjunto finito.
3. Un suceso elemental puede descomponerse en sucesos más simples.
4. Si $A\cap B=\emptyset$, se dice que $A$ y $B$ son incompatibles o mutuamente excluyentes.
5. La primera ley de De Morgan establece que $(A\cup B)^c = A^c \cap B^c$.
6. Una familia de eventos que forma una partición de $\Omega$ puede tener intersección no
   vacía entre sus elementos.
7. El axioma de normalización de Kolmogorov establece que $P(\Omega)=1$.
8. Según los axiomas de Kolmogorov, la probabilidad de un evento puede ser negativa si el
   evento es poco probable.
9. Se cumple que $P(\emptyset)=0$ como consecuencia de los tres axiomas de Kolmogorov.
10. Si $A\subseteq B$, entonces $P(A) \ge P(B)$.
11. La Desigualdad de Boole proporciona una cota **inferior** para la probabilidad de la
    unión de una sucesión de eventos.
12. Dos eventos $A$ y $B$ son independientes si $P(A\cap B) = P(A)\cdot P(B)$.
13. La probabilidad condicionada $P(A|B)$ solo está definida cuando $P(B) > 0$.
14. Si dos eventos son incompatibles ($A\cap B=\emptyset$), entonces también son
    independientes.
15. El Teorema de la Probabilidad Total requiere que los eventos $A_i$ formen una partición
    del espacio muestral.
16. El Teorema de Bayes permite calcular $P(A_j|B)$ a partir de $P(B|A_j)$ y $P(A_j)$.
17. En las variaciones, el orden de colocación de los elementos no importa.
18. El número de permutaciones de $n$ elementos distintos es $n!$.
19. Las combinaciones con repetición permiten que un mismo elemento aparezca más de una vez
    en un mismo subconjunto.
20. Si se extraen bolas de una urna **con reemplazo**, las extracciones sucesivas son eventos
    dependientes entre sí.

---

## Bloque II: Desarrollo y resolución de casos (30 puntos)

Instrucciones: Para cada pregunta, realice los cálculos necesarios en su hoja de desarrollo
y marque con un círculo la alternativa correcta. Cada pregunta vale 3 puntos.

**Pregunta 21 (3 puntos)**
Enunciado: Sea $\Omega=\{1,2,3,4,5,6,7,8\}$, $A=\{1,2,3,4\}$ y $B=\{3,4,5,6\}$. Calcule
$(A\cup B)^c$ usando la primera ley de De Morgan.
A) $\{7,8\}$
B) $\{5,6,7,8\}$
C) $\{1,2,7,8\}$
D) $\{1,2,5,6\}$
E) $\emptyset$

**Pregunta 22 (3 puntos)**
Enunciado: Sea $\Omega=\{1,2,3,4,5,6\}$. ¿Cuál de las siguientes familias es una partición
de $\Omega$?
A) $\{1,2,3\}, \{3,4,5,6\}$
B) $\{1,2\}, \{3,4\}, \{5,6\}$
C) $\{1,2,3\}, \{4,5\}$ (sin incluir a 6)
D) $\{1,2,3,4,5,6\}, \emptyset$
E) $\{1,2\}, \{2,3,4\}, \{5,6\}$

**Pregunta 23 (3 puntos)**
Enunciado: Sean $P(A)=0.3$, $P(B)=0.5$ y $P(A\cap B)=0.1$. Calcule $P(A\cup B)$ por
inclusión-exclusión.
A) $0.9$
B) $0.7$
C) $0.8$
D) $0.3$
E) $0.6$

**Pregunta 24 (3 puntos)**
Enunciado: Sea $A\subseteq B$, con $P(A)=0.25$ y $P(B)=0.55$. Usando que
$B=A\cup(B\cap A^c)$ con ambos disjuntos, calcule $P(B\cap A^c)$.
A) $0.80$
B) $0.25$
C) $0.55$
D) $0.30$
E) $0.20$

**Pregunta 25 (3 puntos)** *(material del libro)*
Enunciado: Una urna contiene 5 bolas rojas y 7 azules. Se extraen 2 bolas sucesivamente
**sin reemplazo**. Calcule la probabilidad de que ambas sean rojas.
A) $5/33 \approx 0.152$
B) $25/144 \approx 0.174$
C) $5/12 \approx 0.417$
D) $4/11 \approx 0.364$
E) $1/3 \approx 0.333$

**Pregunta 26 (3 puntos)** *(material del libro)*
Enunciado: Sean $A$ y $B$ dos sucesos con $P(A)=0.4$, $P(B)=0.5$ y $P(A\cap B)=0.2$.
¿Son $A$ y $B$ independientes?
A) Sí, porque $P(A)\cdot P(B) = 0.2 = P(A\cap B)$
B) No, porque $P(A\cap B) \ne P(A)+P(B)$
C) No, porque $A$ y $B$ son incompatibles
D) Sí, porque $P(A|B)=P(B)$
E) No se puede determinar con estos datos

**Pregunta 27 (3 puntos)** *(material del libro)*
Enunciado: Tres máquinas $A_1$, $A_2$ y $A_3$ producen el 30 %, 45 % y 25 % del total de
piezas de una fábrica, con tasas de defecto de 2 %, 3 % y 5 % respectivamente. Usando el
Teorema de la Probabilidad Total, calcule la probabilidad de que una pieza elegida al azar
sea defectuosa.
A) $0.100$
B) $0.032$
C) $0.0125$
D) $0.045$
E) $0.320$

**Pregunta 28 (3 puntos)** *(material del libro)*
Enunciado: Con los datos de la Pregunta 27, si se sabe que una pieza es defectuosa,
calcule (Teorema de Bayes) la probabilidad de que provenga de la máquina $A_3$.
A) $0.250$
B) $0.156$
C) $0.391$
D) $0.500$
E) $0.125$

**Pregunta 29 (3 puntos)** *(material del libro)*
Enunciado: En una carrera con 8 corredores, ¿de cuántas formas distintas se pueden asignar
los podios de oro, plata y bronce (importa el orden)?
A) $56$
B) $336$
C) $512$
D) $24$
E) $40320$

**Pregunta 30 (3 puntos)** *(material del libro)*
Enunciado: De un grupo de 10 estudiantes, ¿de cuántas formas distintas se puede elegir un
comité de 4 integrantes (sin importar el orden ni los roles dentro del comité)?
A) $5040$
B) $210$
C) $40$
D) $10000$
E) $2520$

---

## Bloque III: Caso Práctico Integrador (15 puntos)

**Pregunta 31 (15 puntos)**
Caso: Control de calidad en una fábrica de componentes electrónicos

Una empresa fabrica componentes electrónicos en tres líneas de producción, $L_1$, $L_2$ y
$L_3$, que aportan el 40 %, 35 % y 25 % del total fabricado, respectivamente. Las tasas de
defecto de cada línea son 3 %, 2 % y 4 % respectivamente. Sea $D$ el evento "el componente
es defectuoso".

1) *(3 puntos, clase)* Defina, usando notación de conjuntos, el espacio muestral $\Omega$ y
   los eventos $L_1$, $L_2$, $L_3$ y $D$. ¿La familia $\{L_1,L_2,L_3\}$ forma una partición
   de $\Omega$? Justifique con la definición vista en clase.
2) *(3 puntos, libro)* Calcule $P(D)$ usando el Teorema de la Probabilidad Total.
3) *(3 puntos, libro)* Si se selecciona un componente al azar y resulta defectuoso, calcule
   $P(L_2|D)$ usando el Teorema de Bayes. Interprete el resultado.
4) *(3 puntos, libro)* Para el control de calidad se seleccionan al azar 5 componentes de un
   lote de 20 (sin reemplazo, sin importar el orden de selección). ¿Cuántas muestras
   distintas de 5 componentes son posibles?
5) *(3 puntos, clase + libro)* Explique, en el contexto de este problema, la diferencia entre
   que los eventos $L_1$, $L_2$, $L_3$ sean **incompatibles** ($L_i\cap L_j=\emptyset$) y que
   sean **independientes** ($P(L_i\cap L_j)=P(L_i)P(L_j)$). ¿Cuál de las dos propiedades
   cumplen $L_1$, $L_2$ y $L_3$ entre sí, y por qué la otra no aplica aquí?

---

## Solución

> Leyenda de fuentes: **[Clase]** = `clases/03. ConjuntosProbabilidades.pdf`;
> **[Libro]** = `libros/LibroBase-STATS1-Estadística Básica.pdf`, Capítulo 5 *"Leyes de
> probabilidad"*. Se repite el enunciado de cada pregunta antes de su respuesta para no
> tener que ir y venir al Bloque original.

### Bloque I — Verdadero o Falso

**1.** *Un experimento aleatorio es aquel cuyo resultado no puede predecirse con certeza,
aunque se conoce el conjunto de resultados posibles.*
**Respuesta: V.** Coincide textualmente con la definición de experimento aleatorio.
**[Clase]** diapositiva "Experimento aleatorio y espacio muestral" (p. 15). **[Libro]**
§5.1, p. 47: *"se dice que un experimento es aleatorio si puede dar lugar a varios
resultados sin que se pueda predecir con certeza el resultado concreto [...] al repetir
el experimento [...] se obtendrán resultados que [...] serán diferentes"*.

**2.** *El espacio muestral $\Omega$ es siempre un conjunto finito.*
**Respuesta: F.** El espacio muestral puede ser finito, infinito numerable o infinito no
numerable. **[Libro]** §5.1, p. 47, clasifica $\Omega$ en las tres categorías (ej. tirada
de un dado = finito; vida de un componente electrónico = infinito numerable; números
reales en $[0,1]$ = infinito no numerable). La clase solo trabaja con ejemplos
finitos/discretos pero no afirma que sea la única posibilidad.

**3.** *Un suceso elemental puede descomponerse en sucesos más simples.*
**Respuesta: F.** Es justo lo contrario: el suceso elemental es el que **no** puede
descomponerse; el que sí puede descomponerse en sucesos más simples es el suceso
**compuesto**. **[Clase]** p. 16 ("Evento elemental: $\{\omega\}$, un único resultado").
**[Libro]** §5.1, p. 47: los sucesos elementales verifican que siempre ocurre alguno de
ellos y son mutuamente excluyentes; el suceso compuesto es el que se construye a partir
de la unión de sucesos elementales.

**4.** *Si $A\cap B=\emptyset$, se dice que $A$ y $B$ son incompatibles o mutuamente
excluyentes.*
**Respuesta: V.** Es la definición estándar de sucesos disjuntos/incompatibles.
**[Clase]** p. 16 ("Eventos disjuntos: $A\cap B=\emptyset$"). **[Libro]** §5.1, p. 48
("incompatibles, o mutuamente excluyentes, si nunca pueden ocurrir a la vez").

**5.** *La primera ley de De Morgan establece que $(A\cup B)^c = A^c \cap B^c$.*
**Respuesta: V.** Es exactamente la primera ley de De Morgan.
**[Clase]** p. 9 ("Leyes de De Morgan — Primera ley"). **[Libro]** p. 48, nota al pie
("Ley de Morgan #1").

**6.** *Una familia de eventos que forma una partición de $\Omega$ puede tener
intersección no vacía entre sus elementos.*
**Respuesta: F.** Por definición de partición, los elementos deben ser disjuntos dos a
dos ($A_i\cap A_j=\emptyset$ si $i\ne j$), no pueden tener intersección no vacía.
**[Clase]** p. 12 ("Particiones del espacio"). **[Libro]** §5.3.3, p. 55 ("conjunto
completo de sucesos": $A_i\cap A_j=\emptyset$ para $i\ne j$).

**7.** *El axioma de normalización de Kolmogorov establece que $P(\Omega)=1$.*
**Respuesta: V.** Es el segundo axioma de Kolmogorov tal cual.
**[Clase]** p. 21 ("2. Normalización: $P(\Omega)=1$"). **[Libro]** §5.2.2, ecuación (5.4),
p. 62.

**8.** *Según los axiomas de Kolmogorov, la probabilidad de un evento puede ser negativa
si el evento es poco probable.*
**Respuesta: F.** El primer axioma (no negatividad) exige $P(A)\ge 0$ para todo evento,
sin excepción — nunca puede ser negativa.
**[Clase]** p. 21 ("1. No negatividad: $P(A)\ge 0,\ \forall A\in\mathcal{F}$"). **[Libro]**
§5.2.2, ecuación (5.3), p. 62.

**9.** *Se cumple que $P(\emptyset)=0$ como consecuencia de los tres axiomas de
Kolmogorov.*
**Respuesta: V.** Se demuestra a partir de $\Omega\cap\emptyset=\emptyset$,
$\Omega\cup\emptyset=\Omega$ y el axioma 3, obteniendo
$1=1+P(\emptyset)\Rightarrow P(\emptyset)=0$.
**[Clase]** p. 20 ("Propiedad 1: $P(\emptyset)=0$"). **[Libro]** ecuación (5.7), p. 63.

**10.** *Si $A\subseteq B$, entonces $P(A) \ge P(B)$.*
**Respuesta: F.** La relación correcta (monotonía) es $A\subseteq B \Rightarrow P(A)\le
P(B)$, no $\ge$.
**[Clase]** p. 26 ("Propiedad 3: monotonía"). **[Libro]** ecuación (5.9), p. 63.

**11.** *La Desigualdad de Boole proporciona una cota **inferior** para la probabilidad de
la unión de una sucesión de eventos.*
**Respuesta: F.** La Desigualdad de Boole da una cota **superior**:
$P\left(\bigcup_i A_i\right)\le\sum_i P(A_i)$.
**[Clase]** p. 32 ("Desigualdad de Boole").

**12.** *Dos eventos $A$ y $B$ son independientes si $P(A\cap B) = P(A)\cdot P(B)$.*
**Respuesta: V.** Es la condición necesaria y suficiente de independencia.
**[Libro]** §5.3.2, ecuación (5.15), p. 54: *"la probabilidad de la intersección de dos
sucesos independientes [...] es el producto de sus probabilidades"*. No se ve en clase.

**13.** *La probabilidad condicionada $P(A|B)$ solo está definida cuando $P(B) > 0$.*
**Respuesta: V.** La probabilidad condicionada se define como $P(A|B)=P(A\cap B)/P(B)$,
cociente que solo tiene sentido si el denominador es positivo.
**[Libro]** §5.3.1, ecuación (5.11) y texto siguiente, p. 53. No se ve en clase.

**14.** *Si dos eventos son incompatibles ($A\cap B=\emptyset$), entonces también son
independientes.*
**Respuesta: F.** Son conceptos distintos: si $A\cap B=\emptyset$ y ambos tienen
probabilidad positiva, entonces $P(A\cap B)=0\ne P(A)\cdot P(B)$, por lo que **no** son
independientes.
**[Libro]** §5.3.2, p. 54: *"es importante no confundir sucesos incompatibles [...] con
sucesos independientes"*. No se ve en clase.

**15.** *El Teorema de la Probabilidad Total requiere que los eventos $A_i$ formen una
partición del espacio muestral.*
**Respuesta: V.** El teorema exige que $\{A_i\}$ sea un "conjunto completo de sucesos"
(partición de $\Omega$, con $P(A_i)>0$).
**[Libro]** §5.3.3, p. 55–56, enunciado del Teorema de la Probabilidad Total. No se ve en
clase.

**16.** *El Teorema de Bayes permite calcular $P(A_j|B)$ a partir de $P(B|A_j)$ y
$P(A_j)$.*
**Respuesta: V.** Es la fórmula de Bayes:
$P(A_j|B)=\dfrac{P(A_j)P(B|A_j)}{\sum_i P(A_i)P(B|A_i)}$.
**[Libro]** §5.3.4, ecuación (5.17), p. 56. No se ve en clase.

**17.** *En las variaciones, el orden de colocación de los elementos no importa.*
**Respuesta: F.** En las variaciones el orden **sí** importa (dos subconjuntos son
distintos si difieren en algún elemento **o** en el orden); lo que no considera el orden
son las **combinaciones**.
**[Libro]** §5.4.1, p. 59. No se ve en clase.

**18.** *El número de permutaciones de $n$ elementos distintos es $n!$.*
**Respuesta: V.** $P_n=V_{n,n}=n(n-1)(n-2)\cdots 1=n!$.
**[Libro]** §5.4.2, ecuación (5.21), p. 60. No se ve en clase.

**19.** *Las combinaciones con repetición permiten que un mismo elemento aparezca más de
una vez en un mismo subconjunto.*
**Respuesta: V.** Es la definición misma de combinación con repetición, a diferencia de
la combinación simple.
**[Libro]** §5.4.3, p. 61. No se ve en clase.

**20.** *Si se extraen bolas de una urna **con reemplazo**, las extracciones sucesivas son
eventos dependientes entre sí.*
**Respuesta: F.** Es lo contrario: con reemplazo, la composición de la urna no cambia
entre extracciones, por lo que los sucesos son **independientes**; sin reemplazo sí son
dependientes.
**[Libro]** Ejemplo II-6, p. 55 (caso a: con reemplazo → independientes; caso b: sin
reemplazo → dependientes). No se ve en clase.

---

### Bloque II — Desarrollo y resolución de casos

**Pregunta 21.** *Sea $\Omega=\{1,2,3,4,5,6,7,8\}$, $A=\{1,2,3,4\}$ y $B=\{3,4,5,6\}$.
Calcule $(A\cup B)^c$ usando la primera ley de De Morgan.*
A) $\{7,8\}$ · B) $\{5,6,7,8\}$ · C) $\{1,2,7,8\}$ · D) $\{1,2,5,6\}$ · E) $\emptyset$

**Respuesta: A) $\{7,8\}$**
$A\cup B=\{1,2,3,4,5,6\}$, por lo que $(A\cup B)^c=\Omega\setminus(A\cup B)=\{7,8\}$.
Verificación por De Morgan: $A^c=\{5,6,7,8\}$, $B^c=\{1,2,7,8\}$, $A^c\cap B^c=\{7,8\}$ ✓.
**[Clase]** p. 9, primera ley de De Morgan.

**Pregunta 22.** *Sea $\Omega=\{1,2,3,4,5,6\}$. ¿Cuál de las siguientes familias es una
partición de $\Omega$?*
A) $\{1,2,3\}, \{3,4,5,6\}$ · B) $\{1,2\}, \{3,4\}, \{5,6\}$ · C) $\{1,2,3\}, \{4,5\}$
(sin incluir a 6) · D) $\{1,2,3,4,5,6\}, \emptyset$ · E) $\{1,2\}, \{2,3,4\}, \{5,6\}$

**Respuesta: B) $\{1,2\},\{3,4\},\{5,6\}$**
Es la única familia que cumple las tres condiciones de partición: ningún subconjunto
vacío, disjuntos dos a dos, y su unión es todo $\Omega=\{1,...,6\}$. Las demás opciones
fallan: A) y E) tienen elementos repetidos entre subconjuntos (no son disjuntas); C) no
cubre el 6; D) incluye $\emptyset$, que no puede ser parte de una partición.
**[Clase]** p. 12, definición de partición.

**Pregunta 23.** *Sean $P(A)=0.3$, $P(B)=0.5$ y $P(A\cap B)=0.1$. Calcule $P(A\cup B)$
por inclusión-exclusión.*
A) $0.9$ · B) $0.7$ · C) $0.8$ · D) $0.3$ · E) $0.6$

**Respuesta: B) $0.7$**
$P(A\cup B)=P(A)+P(B)-P(A\cap B)=0.3+0.5-0.1=0.7$.
**[Clase]** p. 28, inclusión-exclusión para 2 eventos (deducida de los axiomas). **[Libro]**
ecuación (5.10), p. 63.

**Pregunta 24.** *Sea $A\subseteq B$, con $P(A)=0.25$ y $P(B)=0.55$. Usando que
$B=A\cup(B\cap A^c)$ con ambos disjuntos, calcule $P(B\cap A^c)$.*
A) $0.80$ · B) $0.25$ · C) $0.55$ · D) $0.30$ · E) $0.20$

**Respuesta: D) $0.30$**
Como $A\subseteq B$, se cumple $B=A\cup(B\cap A^c)$ con ambos conjuntos disjuntos, luego
$P(B)=P(A)+P(B\cap A^c) \Rightarrow P(B\cap A^c)=P(B)-P(A)=0.55-0.25=0.30$.
**[Clase]** p. 26, demostración de monotonía. **[Libro]** deducción de la ecuación (5.9),
pp. 63–64.

**Pregunta 25.** *(material del libro)* *Una urna contiene 5 bolas rojas y 7 azules. Se
extraen 2 bolas sucesivamente **sin reemplazo**. Calcule la probabilidad de que ambas sean
rojas.*
A) $5/33 \approx 0.152$ · B) $25/144 \approx 0.174$ · C) $5/12 \approx 0.417$ ·
D) $4/11 \approx 0.364$ · E) $1/3 \approx 0.333$

**Respuesta: A) $5/33\approx 0.152$**
Sin reemplazo: $P(R_1)=5/12$; dada la primera roja, quedan 4 rojas de 11 bolas totales,
$P(R_2|R_1)=4/11$. Por la regla del producto,
$P(R_1\cap R_2)=P(R_1)\cdot P(R_2|R_1)=\frac{5}{12}\cdot\frac{4}{11}=\frac{20}{132}=\frac{5}{33}\approx 0.152$.
**[Libro]** §5.3.2, ecuación (5.12) y Ejemplo II-6 (caso sin reemplazo), pp. 54–55.

**Pregunta 26.** *(material del libro)* *Sean $A$ y $B$ dos sucesos con $P(A)=0.4$,
$P(B)=0.5$ y $P(A\cap B)=0.2$. ¿Son $A$ y $B$ independientes?*
A) Sí, porque $P(A)\cdot P(B) = 0.2 = P(A\cap B)$ · B) No, porque
$P(A\cap B) \ne P(A)+P(B)$ · C) No, porque $A$ y $B$ son incompatibles · D) Sí, porque
$P(A|B)=P(B)$ · E) No se puede determinar con estos datos

**Respuesta: A) Sí, son independientes**
$P(A)\cdot P(B)=0.4\times 0.5=0.2$, que coincide exactamente con $P(A\cap B)=0.2$. Como se
cumple la condición necesaria y suficiente de independencia, $A$ y $B$ son independientes.
**[Libro]** §5.3.2, ecuación (5.15), p. 54.

**Pregunta 27.** *(material del libro)* *Tres máquinas $A_1$, $A_2$ y $A_3$ producen el
30 %, 45 % y 25 % del total de piezas de una fábrica, con tasas de defecto de 2 %, 3 % y
5 % respectivamente. Usando el Teorema de la Probabilidad Total, calcule la probabilidad
de que una pieza elegida al azar sea defectuosa.*
A) $0.100$ · B) $0.032$ · C) $0.0125$ · D) $0.045$ · E) $0.320$

**Respuesta: B) $0.032$**
Por el Teorema de la Probabilidad Total, con $\{A_1,A_2,A_3\}$ como partición del espacio
(las tres líneas cubren toda la producción y son excluyentes entre sí):
$P(D)=P(A_1)P(D|A_1)+P(A_2)P(D|A_2)+P(A_3)P(D|A_3)$
$=0.30\times0.02+0.45\times0.03+0.25\times0.05=0.006+0.0135+0.0125=0.032$.
**[Libro]** §5.3.3, ecuación (5.16), p. 56 (idéntico al Ejemplo II-7).

**Pregunta 28.** *(material del libro)* *Con los datos de la Pregunta 27, si se sabe que
una pieza es defectuosa, calcule (Teorema de Bayes) la probabilidad de que provenga de la
máquina $A_3$.*
A) $0.250$ · B) $0.156$ · C) $0.391$ · D) $0.500$ · E) $0.125$

**Respuesta: C) $0.391$**
Por el Teorema de Bayes:
$P(A_3|D)=\dfrac{P(A_3)P(D|A_3)}{P(D)}=\dfrac{0.25\times0.05}{0.032}=\dfrac{0.0125}{0.032}\approx 0.391$.
**[Libro]** §5.3.4, ecuación (5.17), p. 56 (continuación del Ejemplo II-7).

**Pregunta 29.** *(material del libro)* *En una carrera con 8 corredores, ¿de cuántas
formas distintas se pueden asignar los podios de oro, plata y bronce (importa el orden)?*
A) $56$ · B) $336$ · C) $512$ · D) $24$ · E) $40320$

**Respuesta: B) $336$**
Importa el orden de llegada (oro ≠ plata ≠ bronce) y no se repiten corredores, así que es
una **variación** de 8 elementos tomados de 3 en 3: $V_{8,3}=8\times7\times6=336$.
**[Libro]** §5.4.1, ecuación (5.18), p. 59.

**Pregunta 30.** *(material del libro)* *De un grupo de 10 estudiantes, ¿de cuántas
formas distintas se puede elegir un comité de 4 integrantes (sin importar el orden ni los
roles dentro del comité)?*
A) $5040$ · B) $210$ · C) $40$ · D) $10000$ · E) $2520$

**Respuesta: B) $210$**
No importa el orden dentro del comité y cada estudiante participa como máximo una vez, así
que es una **combinación** de 10 elementos tomados de 4 en 4:
$C_{10,4}=\dfrac{10!}{(10-4)!\,4!}=\dfrac{10\times9\times8\times7}{4\times3\times2\times1}=210$.
**[Libro]** §5.4.3, ecuación (5.24), p. 61.

---

### Bloque III — Caso Práctico Integrador (Pregunta 31)

*Caso: Control de calidad en una fábrica de componentes electrónicos. Una empresa fabrica
componentes electrónicos en tres líneas de producción, $L_1$, $L_2$ y $L_3$, que aportan
el 40 %, 35 % y 25 % del total fabricado, respectivamente. Las tasas de defecto de cada
línea son 3 %, 2 % y 4 % respectivamente. Sea $D$ el evento "el componente es
defectuoso".*

**1)** *(3 pts, clase) Defina, usando notación de conjuntos, el espacio muestral $\Omega$
y los eventos $L_1$, $L_2$, $L_3$ y $D$. ¿La familia $\{L_1,L_2,L_3\}$ forma una partición
de $\Omega$? Justifique con la definición vista en clase.*

**Respuesta — [Clase] p. 12, 15–16**
$\Omega$ = conjunto de todos los componentes fabricados por la empresa. $L_1,L_2,L_3
\subseteq\Omega$ son los subconjuntos de componentes que provienen de cada línea; $D
\subseteq\Omega$ es el subconjunto de componentes defectuosos (evento compuesto, ya que se
construye como unión de componentes defectuosos individuales).
$\{L_1,L_2,L_3\}$ **sí es una partición** de $\Omega$: cada componente proviene de
exactamente una línea (son disjuntos, $L_i\cap L_j=\emptyset$ para $i\ne j$) y entre las
tres cubren toda la producción ($L_1\cup L_2\cup L_3=\Omega$), cumpliendo la definición de
partición vista en clase (p. 12) y el "conjunto completo de sucesos" que exige el libro
(§5.3.3, p. 55) para poder aplicar el Teorema de la Probabilidad Total.

**2)** *(3 pts, libro) Calcule $P(D)$ usando el Teorema de la Probabilidad Total.*

**Respuesta — [Libro] §5.3.3, ecuación (5.16), p. 56**
$P(D)=P(L_1)P(D|L_1)+P(L_2)P(D|L_2)+P(L_3)P(D|L_3)$
$=0.40\times0.03+0.35\times0.02+0.25\times0.04=0.012+0.007+0.010=\mathbf{0.029}$.

**3)** *(3 pts, libro) Si se selecciona un componente al azar y resulta defectuoso,
calcule $P(L_2|D)$ usando el Teorema de Bayes. Interprete el resultado.*

**Respuesta — [Libro] §5.3.4, ecuación (5.17), pp. 56–57**
$P(L_2|D)=\dfrac{P(L_2)P(D|L_2)}{P(D)}=\dfrac{0.35\times0.02}{0.029}=\dfrac{0.007}{0.029}
\approx \mathbf{0.241}$ (24.1 %).
Interpretación: aunque $L_2$ aporta el 35 % de la producción total, solo explica el 24.1 %
de los componentes defectuosos, porque su tasa de defecto (2 %) es la más baja de las tres
líneas — la información de que el componente es defectuoso hace **menos probable** que
provenga de $L_2$ en comparación con su peso en la producción total.

**4)** *(3 pts, libro) Para el control de calidad se seleccionan al azar 5 componentes de
un lote de 20 (sin reemplazo, sin importar el orden de selección). ¿Cuántas muestras
distintas de 5 componentes son posibles?*

**Respuesta — [Libro] §5.4.3, ecuación (5.24), p. 61**
No importa el orden de selección y no hay reemplazo (cada componente se elige una sola
vez), así que es una combinación: $C_{20,5}=\dfrac{20!}{15!\,5!}=\mathbf{15\,504}$
muestras distintas.

**5)** *(3 pts, clase + libro) Explique, en el contexto de este problema, la diferencia
entre que los eventos $L_1$, $L_2$, $L_3$ sean **incompatibles** ($L_i\cap L_j=\emptyset$)
y que sean **independientes** ($P(L_i\cap L_j)=P(L_i)P(L_j)$). ¿Cuál de las dos
propiedades cumplen $L_1$, $L_2$ y $L_3$ entre sí, y por qué la otra no aplica aquí?*

**Respuesta — [Libro] §5.3.2, p. 54**
$L_1$, $L_2$ y $L_3$ son **incompatibles** entre sí (por construcción, un componente
proviene de una sola línea, luego $L_i\cap L_j=\emptyset$ para $i\ne j$), pero **no son
independientes**: si fueran independientes se cumpliría $P(L_i\cap L_j)=P(L_i)\cdot
P(L_j)$, y como $P(L_i)>0$ y $P(L_j)>0$ para todas las líneas, el producto
$P(L_i)\cdot P(L_j)$ es positivo, mientras que $P(L_i\cap L_j)=P(\emptyset)=0$. Como
$0\ne P(L_i)\cdot P(L_j)$, la condición de independencia no se cumple. Este es justamente
el punto que advierte el libro (§5.3.2, p. 54): sucesos incompatibles con probabilidad
positiva **nunca** pueden ser independientes al mismo tiempo.

## Notas / dudas

- **Bloque I (V/F)** y las preguntas **21–24** del Bloque II combinan ambas fuentes cuando
  corresponde, pero el núcleo de conjuntos/axiomas viene de `clases/03. ConjuntosProbabilidades.pdf`.
- Las preguntas **25–30** del Bloque II y los ítems **2, 3 y 4** del caso integrador
  (Pregunta 31) son **material del libro base**, Capítulo 5 §5.3 (probabilidad condicionada,
  independencia, Teorema de la Probabilidad Total, Teorema de Bayes) y §5.4 (análisis
  combinatorio: variaciones, permutaciones, combinaciones). **No están en las diapositivas
  de clase.**
- Formato calcado de `practicas/STATS_I_Guía01.pdf` (Bloque I V/F 20 pts + Bloque II opción
  múltiple con cálculo 10×3 pts + Bloque III caso integrador 15 pts = 65 pts totales).
- `formulario.md` todavía no tiene la sección de Unidad 3 completada — se recomienda
  actualizarla con la notación de conjuntos, los axiomas y, si el profesor confirma que
  los verá, la notación de probabilidad condicionada/combinatoria del libro.
