Yes — let’s write down the **typical current–voltage (Id–Vg, Id–Vd) relations** for 2D-material FET-based photodetectors. These usually combine **FET transport equations** with **photocurrent terms**.

---

## **1. Dark Current (No Illumination)**

For a **2D FET channel** (like MoS₂, WSe₂):

* **Linear regime (small Vd):**

$$
I_d = \mu C_{ox} \frac{W}{L} \left[ (V_g - V_{th}) V_d - \frac{V_d^2}{2} \right]
$$

* **Saturation regime (large Vd):**

$$
I_d = \frac{1}{2} \mu C_{ox} \frac{W}{L} (V_g - V_{th})^2
$$

where:

* $\mu$ = carrier mobility
* $C_{ox}$ = gate capacitance per unit area
* $W, L$ = channel width, length
* $V_g$ = gate voltage
* $V_{th}$ = threshold voltage
* $V_d$ = drain voltage

These are the **standard MOSFET-like Id–Vg and Id–Vd relations** adapted to 2D semiconductors.

---

## **2. Under Illumination (Photodetector Behavior)**

Illumination generates extra carriers → additional **photocurrent component**:

$$
I_{ph} = q \eta \frac{P_{opt}}{h\nu} G
$$

where:

* $q$ = electron charge
* $\eta$ = quantum efficiency
* $P_{opt}$ = incident optical power
* $h\nu$ = photon energy
* $G$ = photoconductive gain (can be >>1 in 2D materials due to trap-assisted long lifetime).

Thus, the **total current** becomes:

$$
I_d^{\text{total}} = I_d^{\text{dark}} + I_{ph}
$$

---

## **3. Typical Id–Vg Curve (Transfer Curve)**

$$
I_d(V_g) = \frac{1}{2} \mu C_{ox} \frac{W}{L} (V_g - V_{th})^2 + I_{ph}(V_g)
$$

* The dark term gives the usual quadratic (or exponential in subthreshold) dependence.
* The photocurrent term shifts the curve upward under illumination.
* This is how **photoresponsivity** and **switching ratio** are extracted.

---

## **4. Typical Id–Vd Curve (Output Curve)**

$$
I_d(V_d) = \mu C_{ox} \frac{W}{L} \left[ (V_g - V_{th}) V_d - \frac{V_d^2}{2} \right] + I_{ph}(V_d)
$$

* At low Vd: linear increase (Ohmic region).
* At high Vd: saturation.
* Illumination increases current across all Vd, sometimes introducing asymmetry due to built-in fields in heterostructures.

---

✅ **In short:**

* **Dark Id–Vg, Id–Vd** follow standard FET equations.
* **Illumination adds a photocurrent term** proportional to optical power and gain.
* This modification explains the “light on/off” shift in transfer and output curves of 2D-material photodetectors.

---