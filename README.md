# The-Geometry-of-Pythagorean-Incircle
<div align="center">
  <img src="https://img.shields.io/badge/Math-Geometry-blueviolet?style=for-the-badge" alt="Math Badge">
  <img src="https://img.shields.io/badge/Property-Unique__3--4--5-orange?style=for-the-badge" alt="Unique Property Badge">
  
  <br><br>
  <h1>📐 The Geometry of Pythagorean Incircles</h1>
  <p><i>An exploration of the unique relationship between integer-sided right triangles and their inscribed circles.</i></p>
</div>

<hr>

## 🔮 The Core Phenomenon

Did you know that the **3-4-5 triangle** is the **only** primitive Pythagorean triple where the inscribed circle has an exact area of **&pi;**? For all other primitive triples, the area is a larger multiple of &pi;.

### 🧮 The Formula Cheat Sheet

Here is how the metrics map out using standard side lengths $(a, b, c)$ versus Euclid's parameters $(m, n)$ where $a = m^2-n^2$, $b = 2mn$, and $c = m^2+n^2$:

<table width="100%">
  <thead>
    <tr>
      <th align="left">Metric</th>
      <th align="left">Using Sides (a, b, c)</th>
      <th align="left">Using Euclid's Generators (m, n)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Inradius (r)</b></td>
      <td><code>r = (a + b - c) / 2</code></td>
      <td><code>r = n(m - n)</code></td>
    </tr>
    <tr>
      <td><b>Incircle Area</b></td>
      <td><code>Area = &pi; &times; r&sup2;</code></td>
      <td><code>Area = &pi; &times; [n(m - n)]&sup2;</code></td>
    </tr>
    <tr>
      <td><b>Triangle Area</b></td>
      <td><code>Area = (a &times; b) / 2</code></td>
      <td><code>Area = mn(m&sup2; - n&sup2;)</code></td>
    </tr>
  </tbody>
</table>

<br>

## 🧪 Quick Reference Examples

| Pythagorean Triple | Inradius ($r$) | Incircle Area | Triangle Area |
| :--- | :---: | :---: | :---: |
| **3 - 4 - 5** | **1** | **&pi;** | **6** |
| 5 - 12 - 13 | 2 | 4&pi; | 30 |
| 8 - 15 - 17 | 3 | 9&pi; | 60 |
| 7 - 24 - 25 | 3 | 9&pi; | 84 |

<br>

<details>
  <summary><b>🔍 Click to expand the Uniqueness Proof</b></summary>
  <br>
  <p>To prove why the 3-4-5 triangle is completely unique in having an incircle area of &pi;, we look at the simplified generator formula for the radius:</p>
  <pre>r = n(m - n)</pre>
  <p>For the area to equal &pi;, the radius <code>r</code> must equal 1:</p>
  <pre>1 = n(m - n)</pre>
  <p>Because <code>m</code> and <code>n</code> must be positive integers (where <code>m > n</code>), the only two whole numbers that multiply together to make 1 are 1 and 1. This gives us:</p>
  <ul>
    <li><code>n = 1</code></li>
    <li><code>m - n = 1 &rArr; m = 2</code></li>
  </ul>
  <p>Plugging <code>m = 2</code> and <code>n = 1</code> back into Euclid's triple generator yields exactly <b>3, 4, and 5</b>. Q.E.D.!</p>
</details>

<hr>
