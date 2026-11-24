# Slope Fields & Differential Equations in Desmos

Direct calculator template: [Desmos Slope Field Generator](https://www.desmos.com/calculator/p7vd3cdmei)

---

## 1. Using the Slope Field Generator Template

Desmos does not have a native slope field operator in blank graphs. The recommended workflow is:

1. Open [Desmos Slope Field Generator](https://www.desmos.com/calculator/p7vd3cdmei).
2. Click **Save Copy** to save it to your Desmos account.
3. On **Line 2**, replace `g(x,y) = ...` with your differential equation:
   ```latex
   g(x,y) = f(x,y)
   ```
   *(Where \(\frac{dy}{dx} = f(x,y)\))*

### Examples:

- **Logistic Growth:**
  ```latex
  g(x,y) = y(1 - y)
  ```
- **Linear First-Order:**
  ```latex
  g(x,y) = x - 2y
  ```
- **Autonomous Competing Species:**
  ```latex
  g(x,y) = \frac{y(0.5 - 0.25y - 0.75x)}{x(1 - x - y)}
  ```

---

## 2. Standalone 2-Line Slope Grid (Blank Graph)

If building inside a blank Desmos graph without the template, use this two-line list comprehension:

### Line 1: Define slope function
```latex
M(x,y) = x - y
```

### Line 2: Generate slope segments
```latex
y = \left[M(X,Y)(x - X) + Y \left\{\sqrt{(y - Y)^2 + (x - X)^2} < 0.1\right\} \operatorname{for} X = 0.5[-5...5], Y = 0.5[-5...5]\right]
```

---

## 3. Adding Nullclines & Critical Points

Once your slope field is active, overlay nullclines:

- **Horizontal Nullcline (\(dy/dx = 0\)):**
  Graph \(f(x,y) = 0\).
- **Vertical Nullcline (\(dy/dx \to \pm \infty\)):**
  Graph the denominator of \(f(x,y) = 0\).
- **Equilibria:**
  Add intersection points as `(x_0, y_0)`.

---

*Part of the [Desmos Calculus Visualizers](https://github.com/sheldonstewart/desmos-calculus-visualizers) collection by [Pretty Good Prep](https://prettygoodprep.com).*
