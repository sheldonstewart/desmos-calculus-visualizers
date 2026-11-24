# Riemann Sums & Numerical Integration (Desmos 2D)

Direct calculator link: [desmos.com/calculator](https://www.desmos.com/calculator)

---

## 1. Dynamic Left, Right, & Midpoint Riemann Sums

In single-variable calculus, understanding how step size \(\Delta x\) converges to \(\int_a^b f(x)\,dx\) is central to integration theory.

### Desmos Expressions:

1. **Target function:**
   ```latex
   f(x) = \frac{1}{1 + x^2}
   ```
2. **Integration bounds and partitions:**
   ```latex
   a = 0
   b = 4
   n = 10
   \Delta = \frac{b - a}{n}
   ```
3. **Partition index:**
   ```latex
   I = [1...n]
   ```
4. **Left Riemann Sum rectangles:**
   ```latex
   x_L = a + (I - 1)\Delta
   ```
   *Polygon rectangles in Desmos:*
   ```latex
   \operatorname{polygon}\left((x_L, 0), (x_L, f(x_L)), (x_L + \Delta, f(x_L)), (x_L + \Delta, 0)\right)
   ```
5. **Sum computation:**
   ```latex
   S_L = \sum_{k=1}^n f(a + (k-1)\Delta)\Delta
   ```
6. **Exact Integral Comparison:**
   ```latex
   S_{\text{exact}} = \int_a^b f(x)\,dx
   ```

---

## 2. Trapezoidal Rule Visualization

```latex
x_i = a + (I - 1)\Delta
x_{i+1} = a + I\Delta
\operatorname{polygon}\left((x_i, 0), (x_i, f(x_i)), (x_{i+1}, f(x_{i+1})), (x_{i+1}, 0)\right)
```

---

*Explore more single-variable calculus problem walkthroughs and exams at [Pretty Good Prep](https://prettygoodprep.com).*
