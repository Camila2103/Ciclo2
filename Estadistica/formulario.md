# Formulario y notación — Estadística 1

> Notación y fórmulas confirmadas en `clases/01-Introducción-ConceptosPrevios.pdf` y
> `clases/02-MedidasCaracetristicasDistribución.pdf`. Completar/ajustar si el profesor
> introduce notación distinta en unidades futuras.

## Notación general
| Símbolo | Significado |
|---------|-------------|
| $\bar{x}$ | Media muestral |
| $\mu$ | Media poblacional |
| $s$, $s^2$ | Desviación estándar / varianza muestral |
| $\sigma$, $\sigma^2$ | Desviación estándar / varianza poblacional |
| $\tilde{x}$ | Mediana |
| $Mo$ | Moda |
| $G$ (media) | Media geométrica — ⚠️ el profesor reutiliza $G$ también para el Índice de Gini; el contexto aclara cuál es |
| $H$ | Media armónica |
| $n$ | Tamaño de muestra |
| $N$ | Tamaño de población (o número total de datos en tablas de frecuencia) |
| $\gamma_1$ | Coeficiente de asimetría (sesgo) de Fisher |
| $\gamma_2$ | Curtosis |
| $CV$ | Coeficiente de Variación |
| $p$, $\hat{p}$ | Proporción poblacional / muestral |
| $P_i$, $Q_i$ | Proporciones acumuladas de población / de la variable de interés (Gini) |

## Unidad 1 — Conceptos Previos
### Notas sobre el método del profesor
- Distingue explícitamente estadística **descriptiva** (organizar, resumir, presentar) de
  **inferencial** (generalizar resultados de una muestra a la población).
- Población finita vs. infinita: finita = número limitado y contable de elementos (se puede
  estudiar sin muestreo); infinita = no se puede enumerar todos los elementos.
- Censo = recolecta datos de **toda** la población. Encuesta = recolecta datos de una
  **muestra**.
- Escalas de medición (4): nominal (sin orden), ordinal (con orden, sin operaciones
  aritméticas), de intervalo (sin cero absoluto — ej. temperatura en °C), de razón (con cero
  absoluto — ej. peso, altura, ingreso).

## Unidad 2 — Medidas Características de una Distribución
### Fórmulas clave — Centralización
- Media aritmética: $\bar{x} = \dfrac{1}{n}\sum_{i=1}^n x_i$
- Mediana (n impar): $\tilde{x} = x_{(n+1)/2}$ · (n par): $\tilde{x} = \dfrac{x_{n/2} + x_{n/2+1}}{2}$
- Media geométrica: $G = \left(\prod_{i=1}^n x_i\right)^{1/n}$, $x_i > 0$
- Media armónica: $H = \dfrac{n}{\sum_{i=1}^n 1/x_i}$, $x_i > 0$
- Propiedad: $H \le G \le \bar{x}$ (datos positivos)

### Fórmulas clave — Dispersión
- Rango: $\text{Rango} = \max(X) - \min(X)$
- Varianza **poblacional**: $\sigma^2 = \dfrac{1}{n}\sum_{i=1}^n (x_i-\mu)^2$
- Varianza **muestral** (cuasivarianza): $s^2 = \dfrac{1}{n-1}\sum_{i=1}^n (x_i-\bar{x})^2$
  — ⚠️ el profesor siempre pide el denominador $n-1$ para datos muestrales (corrección de
  Bessel), no $n$.
- Desviación estándar: $s=\sqrt{s^2}$ (muestral) / $\sigma=\sqrt{\sigma^2}$ (poblacional)
- Coeficiente de Variación: $CV = \dfrac{s}{\bar{x}} \times 100$ (muestral)

### Propiedades de la media y la varianza ante transformaciones
- $\sum (x_i - \bar{x}) = 0$
- Si $x'_i = x_i + c$: $\bar{x}' = \bar{x}+c$ ; $\sigma'^2 = \sigma^2$ (no cambia)
- Si $x'_i = k \cdot x_i$: $\bar{x}' = k\bar{x}$ ; $\sigma'^2 = k^2 \sigma^2$
- Combinación lineal $aX+b$: $\text{Var}(aX+b) = a^2 \text{Var}(X)$

### Fórmulas clave — Forma (asimetría y curtosis)
- Coef. de asimetría de Fisher: $\gamma_1 = \dfrac{\frac{1}{n}\sum (x_i-\bar{x})^3}{\left(\frac{1}{n}\sum (x_i-\bar{x})^2\right)^{3/2}}$
  — $\gamma_1=0$ simétrica, $\gamma_1>0$ sesgo positivo (derecha), $\gamma_1<0$ sesgo
  negativo (izquierda).
- Curtosis: $\gamma_2 = \dfrac{\frac{1}{n}\sum (x_i-\bar{x})^4}{\left(\frac{1}{n}\sum (x_i-\bar{x})^2\right)^{2}} - 3$
  — $\gamma_2=0$ normal, $\gamma_2>0$ **leptocúrtica** (pico alto, colas gruesas),
  $\gamma_2<0$ **platicúrtica** (pico bajo, colas delgadas).

### Fórmulas clave — Concentración
- Índice de Gini (áreas): $G = \dfrac{A}{A+B}$
- Índice de Gini (proporciones acumuladas): $G = 1 - 2\sum_{i=1}^n (P_i \cdot Q_i)$
  — ⚠️ **tal cual** esta fórmula, aplicada directo a datos agrupados, puede dar un resultado
  fuera de $[0,1]$. El método correcto con datos agrupados (trapezoidal) no está en las
  diapositivas ni en el libro; ver `generado/resumenes/Clase_Refuerzo_Unidad1y2.md` (Bloque H)
  para el desarrollo completo: $G = 1-\sum (Q_i+Q_{i-1})(P_i-P_{i-1})$, con $P_0=Q_0=0$.
- Propiedades: $G=0$ igualdad perfecta, $G=1$ desigualdad máxima.

### Temas del libro NO cubiertos en las diapositivas de clase
- Agrupamiento en intervalos de clase / marca de clase (libro §2.2.2): $\bar{x} = \dfrac{\sum f_i c_i}{N}$, $s^2 = \dfrac{\sum f_i (c_i-\bar{x})^2}{N}$
- Cuartiles, deciles y percentiles / IQR (libro §3.1.5 y §3.2.1): $IQR = Q_3 - Q_1$

## Unidad 3 — [nombre]
### Fórmulas clave
- *(sin contenido todavía — no hay clase subida para esta unidad)*
