# Multivariable Calculus & Tangent Planes (Desmos 3D)

Direct calculator link: [desmos.com/3d](https://www.desmos.com/3d)

---

## 1. Quadric Surfaces & Explicit Functions

Desmos 3D supports explicit functions \(z = f(x,y)\) as well as parametric surfaces \((x(u,v), y(u,v), z(u,v))\).

### Elliptic Paraboloid
```latex
z = \frac{x^2}{4} + \frac{y^2}{9}
```

### Hyperbolic Paraboloid (Saddle Surface)
```latex
z = x^2 - y^2
```
*Parametric form:*
```latex
(u,\ v,\ u^2 - v^2)
```
- `u` from `-2` to `2`
- `v` from `-2` to `2`

---

## 2. Dynamic Tangent Plane Visualizer

Given a surface \(z = f(x,y)\) and an evaluation point \((x_0, y_0)\):

1. **Define base function:**
   ```latex
   f(x,y) = x^2 - y^2
   ```
2. **Evaluation point (sliders):**
   ```latex
   x_0 = 1
   y_0 = 1
   z_0 = f(x_0, y_0)
   ```
3. **Point on surface:**
   ```latex
   (x_0, y_0, z_0)
   ```
4. **Partial derivatives (finite difference or formula):**
   ```latex
   f_x(x,y) = 2x
   f_y(x,y) = -2y
   ```
5. **Tangent Plane Expression:**
   ```latex
   z = z_0 + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)
   ```
   *Or in parametric form with local bounds:*
   ```latex
   (x_0 + u,\ y_0 + v,\ z_0 + f_x(x_0, y_0)u + f_y(x_0, y_0)v)
   ```
   - `u` from `-1` to `1`
   - `v` from `-1` to `1`

---

*Part of the [Desmos Calculus Visualizers](https://github.com/sheldonstewart/desmos-calculus-visualizers) collection by [Pretty Good Prep](https://prettygoodprep.com).*
