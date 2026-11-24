# 3D Solids of Revolution Templates (Desmos 3D)

Direct calculator link: [desmos.com/3d](https://www.desmos.com/3d)

When graphing solids of revolution in Desmos 3D, you use parametric surfaces of the form \((x(u,v), y(u,v), z(u,v))\).

---

## 1. General Rotation Templates

### Rotation About the \(y\)-Axis

Let the boundary curve be \(x = g(y)\) for \(y \in [c, d]\). Rotating around the \(y\)-axis yields:

```latex
(g(u)\cos(v),\ u,\ g(u)\sin(v))
```

- **`u` domain:** min = `c`, max = `d` (along the rotation axis)
- **`v` domain:** min = `0`, max = `2\pi` (full revolution)

### Rotation About the \(x\)-Axis

Let the boundary curve be \(y = f(x)\) for \(x \in [a, b]\). Rotating around the \(x\)-axis yields:

```latex
(u,\ f(u)\cos(v),\ f(u)\sin(v))
```

- **`u` domain:** min = `a`, max = `b`
- **`v` domain:** min = `0`, max = `2\pi`

---

## 2. Worked Example: Piecewise Region Around \(y\)-Axis

Consider the region bounded by:
- \(y = x^2 \implies x = \sqrt{y}\) for \(0 \le y \le 4\)
- \(y = 6 - x \implies x = 6 - y\) for \(4 \le y \le 6\)

### Surface 1 (Parabolic base):
```latex
(\sqrt{u}\cos(v),\ u,\ \sqrt{u}\sin(v))
```
- `u` from `0` to `4`
- `v` from `0` to `2\pi`

### Surface 2 (Conical top):
```latex
((6 - u)\cos(v),\ u,\ (6 - u)\sin(v))
```
- `u` from `4` to `6`
- `v` from `0` to `2\pi`

### Profile cross-section curves (in the \(xy\) or \(xz\) plane):
```latex
(\sqrt{u},\ u,\ 0)
```
- `u` from `0` to `4`

```latex
(6 - u,\ u,\ 0)
```
- `u` from `4` to `6`

---

## 3. Washer Method (Hollow Solids)

If rotating a region between outer radius \(R(u)\) and inner radius \(r(u)\):

1. **Outer Surface:**
   ```latex
   (R(u)\cos(v),\ u,\ R(u)\sin(v))
   ```
2. **Inner Bore:**
   ```latex
   (r(u)\cos(v),\ u,\ r(u)\sin(v))
   ```
3. **End Caps (Disk Washers at \(u = c\) and \(u = d\)):**
   ```latex
   (t\cos(v),\ c,\ t\sin(v))
   ```
   - `t` from `r(c)` to `R(c)`
   - `v` from `0` to `2\pi`

---

*For more calculus walkthroughs and solved practice exams, check out [Pretty Good Prep](https://prettygoodprep.com).*
