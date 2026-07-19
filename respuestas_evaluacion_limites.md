# Clave de respuestas — Evaluación de Límites
## Cálculo Diferencial | IEDEP | Unidad 2
### Mtro. José Armando Vera Rodríguez

> **Nota importante:** las preguntas de opción múltiple se presentan en orden aleatorio
> para cada alumno. Por esa razón esta clave indica la **respuesta por contenido exacto**,
> no por letra. El alumno puede haber visto esa opción como A, B, C o D dependiendo
> del orden que le tocó.

---

## Pregunta 1
**Enunciado:** ¿Cuál es el significado correcto de la expresión lím f(x) = L cuando x → c?

**Respuesta correcta (busca esta opción, sin importar qué letra tenga):**
> f(x) se acerca a L cuando x se acerca a c, sin importar si f(c) existe.

**Explicación detallada:**
El límite no pregunta qué vale la función *en* c, sino hacia dónde se *dirige* f(x)
cuando x se va aproximando a c. Estas son dos preguntas distintas con respuestas que
pueden ser diferentes.

- La opción "f(c) = L siempre que c exista" está mal porque confunde el límite con
  el valor de la función. Puede haber límite aunque f(c) no exista.
- La opción "f(x) llega exactamente a L en el punto c" está mal porque el límite
  describe el acercamiento, no la llegada. La función puede tener un hueco justo en c.
- La opción "x nunca puede valer c" está mal. x puede valer c; lo que dice el límite
  es que analizamos lo que pasa *cerca* de c, no necesariamente *en* c.

---

## Pregunta 2
**Enunciado:** Calcula lím (5x − 3) cuando x → 2.

**Respuesta correcta:** **7**

**Explicación detallada:**
Se aplica sustitución directa porque f(x) = 5x − 3 es una función lineal,
continua en todos los reales. No hay riesgo de obtener 0/0.

```
f(2) = 5(2) − 3
     = 10 − 3
     = 7
```

Como el resultado es un número definido, ese es el límite:

```
lím (5x − 3) = 7
x → 2
```

---

## Pregunta 3
**Enunciado:** Calcula lím (x² + 2x) cuando x → 3.

**Respuesta correcta:** **15**

**Explicación detallada:**
f(x) = x² + 2x es un polinomio. Los polinomios son continuos en todos los reales,
así que la sustitución directa siempre funciona con ellos.

```
f(3) = (3)² + 2(3)
     = 9 + 6
     = 15
```

```
lím (x² + 2x) = 15
x → 3
```

Para verificar: los valores cercanos a 3 deben acercarse a 15.
f(2.9) = 8.41 + 5.8 = 14.21, f(2.99) = 8.9401 + 5.98 = 14.9201,
f(3.1) = 9.61 + 6.2 = 15.81. Converge a 15 ✓

---

## Pregunta 4
**Enunciado:** Para f(x) = (x² − 9) / (x − 3), ¿qué ocurre cuando se intenta
calcular f(3) por sustitución directa?

**Respuesta correcta (busca esta opción, sin importar qué letra tenga):**
> La sustitución da 0/0, que es una forma indeterminada.

**Explicación detallada:**
Al sustituir x = 3 directamente:

```
f(3) = (3² − 9) / (3 − 3)
     = (9 − 9) / (9 − 9)  ← error: denominador es 3 − 3, no 9 − 9
     = (9 − 9) / (3 − 3)
     = 0 / 0
```

0/0 no es cero ni infinito: es una **forma indeterminada**. Matemáticamente no
tiene valor asignado. El error más común es pensar que 0/0 = 0 o que 0/0 = 1.
Ninguna de las dos es correcta.

Que la sustitución falle **no significa que el límite no exista**. Significa que
hay que usar otro método. En este caso, la tabla de valores muestra que el límite
sí existe y vale 6.

Las otras opciones están mal porque:
- "f(3) = 6 directamente" es falso; no se puede obtener 6 por sustitución directa.
- "f(3) = 0" es falso; el resultado es 0/0, no 0.
- "La sustitución da infinito" es falso; infinito aparecería si solo el denominador
  fuera 0, pero aquí tanto numerador como denominador dan 0.

---

## Pregunta 5
**Enunciado:** Usando la tabla de valores de clase, ¿cuál es el valor de
lím (x² − 9)/(x − 3) cuando x → 3?

**Respuesta correcta (busca esta opción, sin importar qué letra tenga):**
> 6

**Explicación detallada:**
La tabla construida en clase con valores cercanos a x = 3 desde ambos lados:

| x        | 2.5 | 2.9 | 2.99 | → 3 ← | 3.01 | 3.1 | 3.5 |
|----------|-----|-----|------|--------|------|-----|-----|
| f(x)     | 5.5 | 5.9 | 5.99 | **→ 6** | 6.01 | 6.1 | 6.5 |

Por la izquierda: 5.5 → 5.9 → 5.99 → se acerca a 6.
Por la derecha: 6.5 → 6.1 → 6.01 → también se acerca a 6.

Como ambos lados convergen al mismo valor, el límite existe y vale 6.

Una forma de verificarlo algebraicamente (tema de la próxima clase):
(x² − 9)/(x − 3) = (x + 3)(x − 3)/(x − 3) = x + 3, para x ≠ 3.
Entonces lím (x + 3) cuando x → 3 = 3 + 3 = 6 ✓

Las otras opciones están mal porque:
- "0" sería el resultado de f(3) en el numerador solo, no del límite.
- "3" no aparece en ningún lado de la tabla.
- "No existe" es incorrecto: la tabla demuestra que sí existe.

---

## Pregunta 6
**Enunciado:** Calcula lím (2x² − 1) cuando x → 0.

**Respuesta correcta:** **−1**

**Explicación detallada:**
f(x) = 2x² − 1 es un polinomio cuadrático. Sustitución directa:

```
f(0) = 2(0)² − 1
     = 2(0) − 1
     = 0 − 1
     = −1
```

```
lím (2x² − 1) = −1
x → 0
```

Este punto es el **vértice** de la parábola. La parábola abre hacia arriba y su
punto más bajo es exactamente (0, −1). Cuando x se acerca a 0 desde cualquier lado,
la función converge suavemente a −1.

Error frecuente: pensar que el límite es 0 porque x → 0. La variable x tiende a 0,
pero f(x) tiende a −1. No confundas el valor de x con el valor de f(x).

---

## Pregunta 7
**Enunciado:** La memoria usada por un sistema es M(n) = n² + 3 MB, donde n es el
número de procesos. ¿Cuál es el límite de M(n) cuando n → 2?

**Respuesta correcta:** **7** (o 7 MB)

**Explicación detallada:**
M(n) = n² + 3 es un polinomio. Sustitución directa con n = 2:

```
M(2) = (2)² + 3
     = 4 + 3
     = 7 MB
```

```
lím M(n) = 7 MB
n → 2
```

**Interpretación en sistemas:** cuando el número de procesos activos se acerca a 2,
el consumo de memoria converge a 7 MB. Esto es útil para planificación de recursos:
si el sistema va a manejar cerca de 2 procesos simultáneos, se necesitan al menos
7 MB disponibles para ese proceso.

---

## Pregunta 8
**Enunciado:** ¿Cuándo es correcto usar la sustitución directa para calcular un límite?

**Respuesta correcta (busca esta opción, sin importar qué letra tenga):**
> Cuando al sustituir x = c se obtiene un número definido, sin formas del tipo 0/0.

**Explicación detallada:**
La sustitución directa es el método más rápido y debe intentarse primero. Es válida
cuando la función es continua en el punto c, lo que ocurre cuando:

1. No hay división entre cero (denominador ≠ 0 al sustituir).
2. No hay raíz de número negativo.
3. No hay logaritmo de cero o negativo.

Si al sustituir aparece 0/0, ∞/∞, 0·∞ u otras formas indeterminadas, la sustitución
directa falla y hay que usar otro método (tabla, factorización, etc.).

Las otras opciones están mal porque:
- "Siempre, para cualquier función" es falso: falla cuando aparece 0/0.
- "Solo cuando la función es un logaritmo" es falso; funciona con cualquier función
  continua, no exclusivamente con logaritmos.
- "Solo cuando x = 0" es falso; x puede ser cualquier valor. El criterio es si el
  resultado es un número definido, no si x vale 0.

---

## Pregunta 9
**Enunciado:** Calcula lím (x² − 25)/(x − 5) cuando x → 5.

**Respuesta correcta:** **10**

**Explicación detallada:**
Primero intento sustitución directa:

```
f(5) = (5² − 25) / (5 − 5)
     = (25 − 25) / (5 − 5)
     = 0 / 0
```

Forma indeterminada. Paso a la tabla:

| x    | 4.5  | 4.9  | 4.99  | → 5 ← | 5.01  | 5.1  | 5.5  |
|------|------|------|-------|--------|-------|------|------|
| f(x) | 9.5  | 9.9  | 9.99  | **→ 10** | 10.01 | 10.1 | 10.5 |

Ambos lados convergen a 10. El límite existe y vale 10.

**Verificación algebraica** (para el docente o alumno avanzado):
```
(x² − 25)/(x − 5) = (x + 5)(x − 5)/(x − 5) = x + 5   para x ≠ 5
lím (x + 5) = 5 + 5 = 10 ✓
x → 5
```

Este ejercicio es análogo al ejercicio 3 de clase (x² − 9)/(x − 3) = 6,
pero con valores distintos. El patrón es el mismo: diferencia de cuadrados en el
numerador, factor lineal en el denominador, hueco en el punto de análisis.

---

## Pregunta 10
**Enunciado:** Un programa calcula tiempos de respuesta según R(t) = 3t + 4 ms,
donde t es el número de tareas activas. ¿Cuál es el límite del tiempo de respuesta
cuando t → 2?

**Respuesta correcta:** **10** (o 10 ms)

**Explicación detallada:**
R(t) = 3t + 4 es una función lineal. Sustitución directa con t = 2:

```
R(2) = 3(2) + 4
     = 6 + 4
     = 10 ms
```

```
lím R(t) = 10 ms
t → 2
```

**Método utilizado:** sustitución directa, porque R(t) es una recta, continua en
todos los reales. No hay forma indeterminada posible.

**Interpretación en sistemas:** cuando el sistema se acerca a 2 tareas activas
simultáneamente, el tiempo de respuesta converge a 10 ms. Si el SLA (acuerdo de
nivel de servicio) del sistema exige respuesta menor a 10 ms, este punto es el
umbral crítico: con más de 2 tareas activas el sistema comienza a incumplirlo.

---

## Tabla resumen para revisión rápida

| # | Tema | Respuesta | Método |
|---|------|-----------|--------|
| 1 | Definición de límite | f(x) se acerca a L cuando x → c, sin importar f(c) | Conceptual |
| 2 | lím (5x − 3), x → 2 | 7 | Sustitución directa |
| 3 | lím (x² + 2x), x → 3 | 15 | Sustitución directa |
| 4 | ¿Qué pasa con f(3) en (x²−9)/(x−3)? | Forma indeterminada 0/0 | Conceptual |
| 5 | lím (x²−9)/(x−3), x → 3 | 6 | Tabla de valores |
| 6 | lím (2x²−1), x → 0 | −1 | Sustitución directa |
| 7 | lím M(n) = n²+3, n → 2 | 7 MB | Sustitución directa |
| 8 | ¿Cuándo usar sustitución directa? | Cuando no aparece 0/0 | Conceptual |
| 9 | lím (x²−25)/(x−5), x → 5 | 10 | Tabla de valores |
| 10 | lím R(t) = 3t+4, t → 2 | 10 ms | Sustitución directa |

---

*Cálculo Diferencial — IEDEP — Mtro. José Armando Vera Rodríguez*
*Unidad 2: Límites y Continuidad*
