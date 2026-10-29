## Question 1 [3 marks]{.marks}

**Given:** $p$: "Eric reads Newsweek" · $q$: "Eric reads the New Yorker" · $r$: "Eric reads Times"

**a)** Eric reads Newsweek and the New Yorker but not Times
$$p \land q \land \neg r$$

**b)** Eric reads Newsweek and the New Yorker, or he does not read Newsweek and Time
$$(p \land q) \lor \neg(p \land r)$$

**c)** It is not true that Eric reads Time and the New Yorker but not Newsweek
$$\neg\big((r \land q) \land \neg p\big)$$

## Question 2 [8 marks]{.marks}

**a)** Truth table for $p \land \neg q$

| $p$ | $q$ | $\neg q$ | $p \land \neg q$ |
|:---:|:---:|:---:|:---:|
| T | T | F | **F** |
| T | F | T | **T** |
| F | T | F | **F** |
| F | F | T | **F** |

**b)** Truth table for $\neg p \lor \neg q$

| $p$ | $q$ | $\neg p$ | $\neg q$ | $\neg p \lor \neg q$ |
|:---:|:---:|:---:|:---:|:---:|
| T | T | F | F | **F** |
| T | F | F | T | **T** |
| F | T | T | F | **T** |
| F | F | T | T | **T** |

**c)** Truth table for $\neg(\neg p \land q)$

| $p$ | $q$ | $\neg p$ | $\neg p \land q$ | $\neg(\neg p \land q)$ |
|:---:|:---:|:---:|:---:|:---:|
| T | T | F | F | **T** |
| T | F | F | F | **T** |
| F | T | T | T | **F** |
| F | F | T | F | **T** |

**d)** Truth table for $\neg(\neg p \land \neg q)$

| $p$ | $q$ | $\neg p$ | $\neg q$ | $\neg p \land \neg q$ | $\neg(\neg p \land \neg q)$ |
|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | F | F | F | **T** |
| T | F | F | T | F | **T** |
| F | T | T | F | F | **T** |
| F | F | T | T | T | **F** |

## Question 3 [5 marks]{.marks}

**Proposition:** $\sim(p \land q) \land (p \lor q)$

| $p$ | $q$ | $p \land q$ | $\sim(p \land q)$ | $p \lor q$ | $\sim(p \land q) \land (p \lor q)$ |
|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | T | F | T | **F** |
| T | F | F | T | T | **T** |
| F | T | F | T | T | **T** |
| F | F | F | T | F | **F** |

**Conclusion:** For the proposition as written, the final column yields $(\text{F}, \text{T}, \text{T}, \text{F})$. Therefore, it is a **contingency** (equivalent to exclusive-OR, $p \oplus q$).

## Question 4 [4 marks]{.marks}

**Proof of the printed identity:** $p \lor (q \lor r) \equiv (p \lor q) \lor r$

| $p$ | $q$ | $r$ | $q \lor r$ | $\mathbf{p \lor (q \lor r)}$ | $p \lor q$ | $\mathbf{(p \lor q) \lor r}$ |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| T | T | T | T | **T** | T | **T** |
| T | T | F | T | **T** | T | **T** |
| T | F | T | T | **T** | T | **T** |
| T | F | F | F | **T** | T | **T** |
| F | T | T | T | **T** | T | **T** |
| F | T | F | T | **T** | T | **T** |
| F | F | T | T | **T** | F | **T** |
| F | F | F | F | **F** | F | **F** |

**Conclusion:** Since the columns $p \lor (q \lor r)$ and $(p \lor q) \lor r$ have identical truth values for all combinations, the equivalence is proven.

*Note:* For the distributive law described in words, $p \lor (q \land r) \equiv (p \lor q) \land (p \lor r)$, both sides evaluate identically to $\text{T}, \text{T}, \text{T}, \text{T}, \text{T}, \text{F}, \text{F}, \text{F}$.

## Question 5 [4 marks]{.marks}

**Normalized form**

| Number | Normalized form (fractional: $0.1 \le \lvert m\rvert < 1$) | Normalized form (scientific: $1 \le \lvert m\rvert < \text{base}$) |
|:---|:---|:---|
| **a)** $1001.1010_2$ | $\mathbf{0.10011010_2 \times 2^4}$ | $1.0011010_2 \times 2^3$ |
| **b)** $0.007633$ | $\mathbf{0.7633 \times 10^{-2}}$ | $7.633 \times 10^{-3}$ |
| **c)** $444.222$ | $\mathbf{0.444222 \times 10^3}$ | $4.44222 \times 10^2$ |
| **d)** $11011.1100_2$ | $\mathbf{0.110111100_2 \times 2^5}$ | $1.10111100_2 \times 2^4$ |

## Question 6 [4 marks]{.marks}

**a)** $\big|\,|2 - 5| - |4 - 11|\,\big|$
$$= \big|\,|-3| - |-7|\,\big| = |3 - 7| = |-4| = \mathbf{4}$$

**b)** $|2 - 7| - |4 - 1|$
$$= |-5| - |3| = 5 - 3 = \mathbf{2}$$

## Question 7 [6 marks]{.marks}

Given true value $A = 55.777$.

**a)** $A$ is rounded to $55.78$

- Absolute error:
$$e = |55.777 - 55.78| = |-0.003| = \mathbf{0.003}$$
- Relative error:
$$e_r = \frac{e}{|A|} = \frac{0.003}{55.777} \approx \mathbf{0.000053786} \quad (5.38 \times 10^{-5})$$

**b)** $A$ is truncated to $55.77$

- Absolute error:
$$e = |55.777 - 55.77| = \mathbf{0.007}$$
- Relative error:
$$e_r = \frac{e}{|A|} = \frac{0.007}{55.777} \approx \mathbf{0.00012550} \quad (1.26 \times 10^{-4})$$

## Question 8 [8 marks]{.marks}

Given $\mathbb{N} = \{1, 2, 3, \dots\}$.

**a)** $A = \{x : x \in \mathbb{N},\, 2 < x < 15\}$
$$A = \{3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14\}$$

**b)** $B = \{x : x \in \mathbb{N},\, x \text{ is odd},\, x < 15\}$
$$B = \{1, 3, 5, 7, 9, 11, 13\}$$

**c)** $C = \{x : x \in \mathbb{N},\, 4 - x = 2\}$
$$4 - x = 2 \implies x = 2, \qquad C = \{2\}$$

**d)** Venn diagram for $A \cap B$

- $A \cap B = \{3, 5, 7, 9, 11, 13\}$
- Only in $A$ ($A \setminus B$): $\{4, 6, 8, 10, 12, 14\}$
- Only in $B$ ($B \setminus A$): $\{1\}$

<div class="venn">
<svg viewBox="0 0 560 300" xmlns="http://www.w3.org/2000/svg" font-family="Helvetica, Arial, sans-serif">
  <rect x="2" y="2" width="556" height="296" rx="6" fill="none" stroke="#333" stroke-width="1.5"/>
  <text x="14" y="24" font-size="14" font-weight="bold">Universal set ℕ</text>
  <circle cx="215" cy="150" r="110" fill="#4a7fc1" fill-opacity="0.25" stroke="#2f5d94" stroke-width="2"/>
  <circle cx="345" cy="150" r="110" fill="#d9822b" fill-opacity="0.25" stroke="#a85f14" stroke-width="2"/>
  <text x="140" y="52" font-size="16" font-weight="bold" fill="#2f5d94">Set A</text>
  <text x="385" y="52" font-size="16" font-weight="bold" fill="#a85f14">Set B</text>
  <text x="165" y="135" font-size="14" text-anchor="middle">4, 6, 8,</text>
  <text x="165" y="155" font-size="14" text-anchor="middle">10, 12, 14</text>
  <text x="280" y="135" font-size="14" text-anchor="middle">3, 5, 7,</text>
  <text x="280" y="155" font-size="14" text-anchor="middle">9, 11, 13</text>
  <text x="280" y="178" font-size="12" text-anchor="middle" fill="#444">A ∩ B</text>
  <text x="400" y="150" font-size="14" text-anchor="middle">1</text>
  <text x="500" y="270" font-size="13" text-anchor="middle" fill="#444">2, 15, 16, 17, …</text>
</svg>
</div>

## Question 9 [12 marks]{.marks}

**a)** $(0.7125 \times 10^2) \times (0.8421 \times 10^3)$
$$= (0.7125 \times 0.8421) \times 10^{2+3} = \mathbf{0.59999625 \times 10^5} \quad (\text{or } 5.9999625 \times 10^4)$$

**b)** $(0.5451 \times 10^5) \times (7.342 \times 10^2)$
$$= (0.5451 \times 7.342) \times 10^{5+2} = 4.0021242 \times 10^7 = \mathbf{0.40021242 \times 10^8}$$

**c)** $0.1245 \times 10^3 + 0.2214 \times 10^5$

Align exponents to $10^5$: $0.1245 \times 10^3 = 0.001245 \times 10^5$. Then add the mantissas:
$$= (0.001245 + 0.2214) \times 10^5 = \mathbf{0.222645 \times 10^5} \quad (\text{or } 2.22645 \times 10^4)$$

**d)** $0.1101_2 \times 2^5 - 0.1010_2 \times 2^5$

Subtract the mantissas: $0.1101_2 - 0.1010_2 = 0.0011_2$. Then normalize:
$$0.0011_2 \times 2^5 = \mathbf{0.11_2 \times 2^3} \quad (\text{or } 1.1_2 \times 2^2)$$

## Question 10 [6 marks]{.marks}

### 1. $E_1 = xyz + xy'z' + xy'z + x'y'z'$

Minterms: $xyz = 111 = m_7$, $xy'z' = 100 = m_4$, $xy'z = 101 = m_5$, $x'y'z' = 000 = m_0$.

**Karnaugh map**

| $x \backslash yz$ | **00** | **01** | **11** | **10** |
|:---:|:---:|:---:|:---:|:---:|
| **0** | **1** ($m_0$) | 0 | 0 | 0 |
| **1** | **1** ($m_4$) | **1** ($m_5$) | **1** ($m_7$) | 0 |

**Grouping**

- Group 1: cells $\{m_0, m_4\} \implies \mathbf{y'z'}$
- Group 2: cells $\{m_5, m_7\} \implies \mathbf{xz}$

**Minimal sum:**
$$\mathbf{E_1 = y'z' + xz}$$

### 2. $E_2 = xy'z + x'yz' + xy'z' + x'yz + x'y'z' + x'y'z$

Minterms: $xy'z = m_5$, $x'yz' = m_2$, $xy'z' = m_4$, $x'yz = m_3$, $x'y'z' = m_0$, $x'y'z = m_1$.

**Karnaugh map**

| $x \backslash yz$ | **00** | **01** | **11** | **10** |
|:---:|:---:|:---:|:---:|:---:|
| **0** | **1** ($m_0$) | **1** ($m_1$) | **1** ($m_3$) | **1** ($m_2$) |
| **1** | **1** ($m_4$) | **1** ($m_5$) | 0 | 0 |

**Grouping**

- Group 1: entire top row $\{m_0, m_1, m_3, m_2\} \implies \mathbf{x'}$
- Group 2: quad block $\{m_0, m_1, m_4, m_5\} \implies \mathbf{y'}$

**Minimal sum:**
$$\mathbf{E_2 = x' + y'}$$
