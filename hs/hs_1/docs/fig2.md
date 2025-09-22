# 1.

### **Id–Vd Behavior in the MoS₂/WSe₂ Memtransistor**

1. **Low bias (Vd ≈ 0–2 V, exponent ≈ 2)**

   * Conduction is nearly **Ohmic or trap-free SCLC**.
   * Current grows quadratically with voltage: $I \propto V^2$.

2. **Intermediate bias (Vd ≈ 2–3 V, exponent ≈ 10)**

   * **Trap-controlled SCLC dominates**.
   * Deep traps start to capture carriers, so most injected carriers go into filling traps instead of contributing to current.
   * As voltage increases, more carriers fill traps rapidly → **steep rise in current**, hence the very high exponent.

3. **Higher bias (Vd ≈ 3–5 V, exponent ≈ 5.8)**

   * Many traps are saturated → additional carriers increasingly contribute directly to conduction.
   * Current still rises faster than quadratic, but less steeply than during the trap-filling onset.

---

### **Why deep traps give faster current increase**

* Deep traps initially **hold carriers**, preventing conduction.
* When enough voltage is applied, carriers **fill these traps rapidly**, suddenly freeing the path for more mobile carriers.
* This abrupt “trap-filling” leads to a **superlinear current rise** (very high slope in log–log plot).
* Once traps are partially filled, the effect diminishes → slope decreases.

---

✅ **Takeaway:**
The Id–Vd curve shows three regimes: Ohmic → trap-controlled steep increase (deep trap filling) → partially trap-saturated SCLC. The deep traps cause the current to increase faster because filling them suddenly allows many carriers to flow.

---

# 2.
**Child’s Law** (or the **Child–Langmuir law**) describes the **space-charge-limited current (SCLC)** in a vacuum diode or an insulating layer when the current is limited not by the material’s conductivity but by the **space charge of the injected carriers**.

---

### **Basic Form (1D case)**

For a planar diode of gap $d$ under voltage $V$, the current density $J$ is:

$$
J = \frac{9}{8} \varepsilon \mu \frac{V^2}{d^3}
$$

Where:

* $\varepsilon$ = permittivity of the material
* $\mu$ = carrier mobility
* $V$ = applied voltage
* $d$ = distance between electrodes

---

### **Key Points**

1. **Quadratic Voltage Dependence:** $J \propto V^2$ — this explains why, in low-bias regions of the MoS₂/WSe₂ memtransistor, the exponent is around 2.
2. **Trap-Free Assumption:** This simple law assumes no traps; all carriers contribute immediately to conduction.
3. **SCLC with Traps:** If traps exist (shallow or deep), the exponent becomes larger than 2 ($I \propto V^\alpha$, $\alpha > 2$) because the voltage must first fill traps before current can rise freely.

---