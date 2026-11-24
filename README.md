# Desmos Calculus Visualizers 📐✨

[![Website](https://img.shields.io/badge/Pretty%20Good%20Prep-Exam%20Prep-2563eb?style=flat-square)](https://prettygoodprep.com)
[![GitHub Discussions](https://img.shields.io/badge/Discussions-Join-10b981?style=flat-square)](https://github.com/sheldonstewart/desmos-calculus-visualizers/discussions)
[![License: MIT](https://img.shields.io/badge/License-MIT-gray?style=flat-square)](LICENSE)

A curated collection of copy-paste ready, verified **Desmos 2D and 3D interactive visualizers** for university single-variable calculus, multivariable calculus, and differential equations.

Created and maintained by [Pretty Good Prep](https://prettygoodprep.com) — university calculus and STEM exam preparation with solved past exams and guided walkthroughs.

---

## 🚀 Quick Links & Calculators

| Tool | Calculator Link | Description |
|---|---|---|
| **3D Solids of Revolution** | [Desmos 3D Calculator](https://www.desmos.com/3d) | Disk, washer, and shell methods rotated around the \(x\) or \(y\) axis |
| **Slope Fields (Phase-Plane)** | [Desmos Slope Field Template](https://www.desmos.com/calculator/p7vd3cdmei) | First-order ODE direction fields and nullclines |
| **2D Region Slicing** | [Desmos 2D Calculator](https://www.desmos.com/calculator) | Bounded regions with dynamic horizontal/vertical slice sliders |
| **Multivariable 3D Surfaces** | [Desmos 3D Calculator](https://www.desmos.com/3d) | Quadric surfaces, paraboloids, and tangent planes |

---

## 📚 Visualizer Library

### 1. 3D Solids of Revolution (Disk & Washer Method)

Rotating regions around axes is one of the most conceptually challenging topics in Integral Calculus (Calculus II). Desmos 3D supports full parametric surfaces:

#### Rotation around the \(y\)-axis
For a boundary curve \(x = g(y)\) over \(c \le y \le d\):
```latex
(g(u)\cos(v),\ u,\ g(u)\sin(v))
```
- **Surface parameter `u`:** min = `c`, max = `d` (vertical height)
- **Rotation parameter `v`:** min = `0`, max = `2\pi` (full \(360^\circ\) revolution)

**Example:** Paraboloid solid \(y = x^2\) from \(y = 0\) to \(y = 4\) (so \(x = \sqrt{y}\)):
```latex
(\sqrt{u}\cos(v),\ u,\ \sqrt{u}\sin(v))
```
*Under the expression, set `u` from `0` to `4`, and `v` from `0` to `2\pi`.*

👉 Full documentation and multi-curve washer templates: [`templates/solids-of-revolution-3d.md`](templates/solids-of-revolution-3d.md)

---

### 2. 2D Bounded Regions with Dynamic Slices

Visualizing the representative rectangle or slice before integrating:

1. **Boundary curves:**
   ```latex
   y = x^{2}
   y = 6 - x
   ```
2. **Shaded bounded region** (intersection at \(x = 2\)):
   ```latex
   0 \le x \le 2 \left\{x^{2} \le y \le 6 - x\right\}
   ```
3. **Representative slice at height `b`** (with dynamic slider \(0 \le b \le 6\)):
   ```latex
   R = \left\{b \le 4:\ \sqrt{b},\ 6 - b\right\}
   y = b \left\{0 \le x \le R\right\}
   ```

---

### 3. Slope Fields & Autonomous ODEs

Visualizing differential equations \( \frac{dy}{dx} = f(x,y) \):

1. Open the [Desmos Slope Field Generator](https://www.desmos.com/calculator/p7vd3cdmei) and click **Save Copy**.
2. On **Line 2**, define your derivative function:
   ```latex
   g(x,y) = \frac{y\left(\frac{1}{2} - \frac{y}{4} - \frac{3x}{4}\right)}{x(1 - x - y)}
   ```
3. The built-in grid handles segment normalization and slope rendering automatically.

👉 Detailed ODE templates & nullcline overlays: [`templates/slope-fields-differential-equations.md`](templates/slope-fields-differential-equations.md)

---

### 4. Multivariable Surfaces & Tangent Planes

In multivariable calculus (Calculus III), visualizing tangent planes touching 3D surfaces:

- **Surface \(z = f(x,y)\):**
  ```latex
  (u,\ v,\ u^{2} - v^{2})
  ```
- **Tangent plane at \((x_0, y_0)\):**
  ```latex
  (u,\ v,\ f(x_0, y_0) + f_x(x_0, y_0)(u - x_0) + f_y(x_0, y_0)(v - y_0))
  ```

👉 Complete quadric surfaces and vector fields: [`templates/multivariable-surfaces-3d.md`](templates/multivariable-surfaces-3d.md)

---

## ⚠️ Common Desmos Syntax Rules

| Rule | ✅ Correct | ❌ Incorrect |
|---|---|---|
| **Pi symbol** | `2\pi` | `2/\pi` (evaluates to \(2/\pi \approx 0.64\) radians) |
| **Roots** | `\sqrt{u}` | `root(u)` |
| **3D Domains** | Enter bounds in sub-fields below the expression | Do not write inline set bounds like `\{0 < v < 2\pi\}` |
| **Derivatives** | Define `g(x,y) = ...` | Do not write `dy/dx = ...` (Desmos treats `d` as a slider) |
| **3D Solids** | Select **Surface** if it defaults to a 1D curve | Leaving mode as curve |

---

## 🎓 About Pretty Good Prep

This repository is built and maintained by **[Pretty Good Prep](https://prettygoodprep.com)**.

Pretty Good Prep helps university STEM students ace their midterms and finals with:
- **Verified Past Exams & Solved Finals:** Real school-specific midterms and finals with step-by-step solutions.
- **Master Math Skill Catalog:** Targeted intuition, formula breakdowns, and interactive practice for Calculus I, II, III, Linear Algebra, and ODEs.
- **Exam Predictors:** Topic likelihood analysis based on past school syllabi and exam trends.

Explore courses and practice exams at **[prettygoodprep.com](https://prettygoodprep.com)**.

---

## 💬 Community & Discussions

Got a neat Desmos visualizer, formula preset, or question?
- Join the conversation in [GitHub Discussions](https://github.com/sheldonstewart/desmos-calculus-visualizers/discussions).
- Feel free to open an issue or pull request to add more university math templates!

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).
