# Límites: estimación por tabla y cómo graficarlos en Desmos

## Ejemplo 1 — f(x) = (x² − 1) / (x − 1), límite cuando x → 1

f(1) no está definida (da 0/0), pero podemos estimar el límite construyendo una tabla con valores de x cada vez más cercanos a 1, desde ambos lados.

**Por la izquierda (x < 1):**

| x | f(x) |
|---|------|
| 0.5 | 1.5 |
| 0.9 | 1.9 |
| 0.99 | 1.99 |
| 0.999 | 1.999 |
| → 1 | → 2 |

**Por la derecha (x > 1):**

| x | f(x) |
|---|------|
| 1.5 | 2.5 |
| 1.1 | 2.1 |
| 1.01 | 2.01 |
| 1.001 | 2.001 |
| → 1 | → 2 |

Como ambos lados se acercan al mismo valor, el límite existe:

**lím (x²−1)/(x−1) = 2, aunque f(1) no exista.**

### Cómo mostrarlo en Desmos

1. **Grafica la función:**
   ```
   f(x) = (x^2-1)/(x-1)
   ```
   Notarás un "hueco" en x = 1, porque ahí f(1) no está definida.

2. **Marca el punto vacío en x = 1:**
   ```
   (1, 2)
   ```
   Dale clic al punto en la lista izquierda y elige el estilo de círculo **abierto** (open point), ya que es un hueco, no un punto real de la función.

3. **Tabla de valores** (botón "+" → *table*):
   - Columna x₁: `0.5, 0.9, 0.99, 0.999, 1.001, 1.01, 1.1, 1.5`
   - Columna x₂: `f(x_1)`

4. **Punto deslizable (slider) para animar el acercamiento:**
   ```
   x_1 = 0.5
   ```
   Esto crea automáticamente un control deslizante. Ajusta su rango mínimo a `0` y máximo a `2` (clic en los números del slider para cambiarlos), y el paso a `0.01` para que se mueva suavemente.

   Luego agrega:
   ```
   (x_1, f(x_1))
   ```
   Mueve el slider y verás el punto deslizarse sobre la curva acercándose al hueco en (1, 2), sin nunca tocarlo — la idea central del límite.

5. **Opcional — restringir el dominio:**
   ```
   f(x) = (x^2-1)/(x-1) \{x \neq 1\}
   ```

---

## Ejemplo 2 — lím (3x + 5) cuando x → 2

A diferencia del ejemplo anterior, f(x) = 3x + 5 es **continua** en x = 2 (no hay hueco ni indefinición), así que el límite coincide directamente con f(2) = 11.

### Cómo mostrarlo en Desmos

1. **Grafica la función:**
   ```
   f(x) = 3x + 5
   ```

2. **Marca el punto límite:**
   ```
   (2, 11)
   ```
   Aquí el punto puede quedar **relleno** (no abierto), porque f(2) sí existe y sí vale 11.

3. **Tabla de acercamiento** (botón "+" → *table*):
   - Columna x₁: `1.5, 1.9, 1.99, 1.999, 2.001, 2.01, 2.1, 2.5`
   - Columna x₂: `f(x_1)`

4. **Slider animado:**
   ```
   x_1 = 1.5
   ```
   Ajusta su rango a mínimo `1`, máximo `3`, y el paso a `0.01`.

   Luego:
   ```
   (x_1, f(x_1))
   ```
   Mueve el slider hacia 2 y verás el punto deslizarse sobre la recta, acercándose a (2, 11) — y en este caso sí puede "tocarlo" exactamente, porque la función es continua ahí.

---

## Cómo crear un slider en Desmos, paso a paso

1. Haz clic en un renglón vacío del panel izquierdo.
2. Escribe una variable con un valor numérico, por ejemplo:
   ```
   x_1 = 1.5
   ```
   (para el subíndice: escribe `x`, luego `_1`, Desmos lo convierte en x₁ chiquito).
3. Al presionar Enter, Desmos detecta que es un número suelto y muestra automáticamente un control deslizante debajo, con un botón de reproducción ▶️.
4. Si no aparece solo, busca el ícono azul a la derecha de esa línea y dale clic para agregarlo.
5. Ajusta el rango del slider:
   - Clic en el valor mínimo (por defecto -10) y cámbialo según el ejemplo.
   - Clic en el valor máximo (por defecto 10) y cámbialo según el ejemplo.
   - Opcional: cambia el "paso" (step) a `0.1` o `0.01` para un movimiento más suave.
6. Agrega un punto que dependa de esa variable, por ejemplo:
   ```
   (x_1, f(x_1))
   ```
7. Arrastra el círculo del slider o dale al botón ▶️ para que se mueva solo, y observa cómo el punto se desliza sobre la curva acercándose al valor del límite.

