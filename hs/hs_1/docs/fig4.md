
---

### 1. **Fermi energy splitting under illumination**

In a semiconductor at equilibrium (no light, no bias), there’s a single **Fermi energy level (Ef)**, which represents the chemical potential of electrons—the energy level at which the probability of finding an electron is 50%.

When the device is illuminated:

* **Photons excite electrons from the valence band to the conduction band**, creating electron-hole pairs.
* This generates **nonequilibrium populations** of electrons and holes.
* Each type of carrier can now be described by its own **quasi-Fermi level**:

  * **Electron quasi-Fermi level (Efn):** describes the population of electrons in the conduction band.
  * **Hole quasi-Fermi level (Efp):** describes the population of holes in the valence band.

So, under illumination:

$$
E_f \rightarrow E_{fn} \text{ (electrons)}, \quad E_{fp} \text{ (holes)}
$$

This “splitting” essentially tells us that electrons and holes are no longer in equilibrium with each other—they are driven by the light-generated excess carriers.

---

### 2. **Return to equilibrium after illumination**

After the light is turned off:

* In an ideal, defect-free semiconductor, the electron-hole pairs would **recombine quickly**, and the Fermi energy would return to its original equilibrium value.
* In reality, the **channel materials (MoS2/WSe2) contain defects**, such as:

  * **Vacancy defects** (missing atoms)
  * **Interlayer traps** in the heterojunction
  * **Impurities**

These defects can **trap electrons or holes**, temporarily storing them. This leads to:

* **Extended relaxation time:** the carriers do not immediately recombine.
* **Persistent current (PSC not returning to initial level):** because some carriers remain trapped, the device maintains a higher conductance than before stimulation, effectively “remembering” the light pulse.

---

### 3. **Implications for synaptic behavior**

This extended relaxation time is crucial for mimicking **biological synapses**:

* The gradual decay of the **postsynaptic current (PSC)** is analogous to **short-term memory (STM) or long-term memory (LTM)** in a neural synapse.
* By controlling light intensity, pulse duration, or pulse number, the device can transition from **STM (fast decay)** to **LTM (slow decay)**.

---

### **In short:**

* **Light hits the device → Fermi level splits → electron and hole populations are out of equilibrium → current increases.**
* **Light off → carriers slowly recombine due to traps → current decays slowly, creating memory-like behavior.**

---

### 1. **Equilibrium carrier densities**

In thermal equilibrium, the electron and hole concentrations are determined by a single Fermi level $E_F$:

$$
n_0 = N_C e^{-(E_C - E_F)/k_BT}, \quad p_0 = N_V e^{-(E_F - E_V)/k_BT}
$$

Where:

* $n_0, p_0$ = equilibrium electron and hole densities
* $N_C, N_V$ = effective density of states for conduction/valence bands
* $E_C, E_V$ = conduction band minimum / valence band maximum
* $k_B$ = Boltzmann constant, $T$ = temperature

---

### 2. **Nonequilibrium carrier densities**

Under illumination or external bias, **electrons and holes are no longer in equilibrium**, so we define **quasi-Fermi levels** $E_{Fn}$ for electrons and $E_{Fp}$ for holes:

$$
n = N_C e^{-(E_C - E_{Fn})/k_BT}, \quad p = N_V e^{-(E_{Fp} - E_V)/k_BT}
$$

Notice the difference:

* At equilibrium: $E_{Fn} = E_{Fp} = E_F$
* Under illumination: $E_{Fn} - E_{Fp} = \text{quasi-Fermi level splitting} \neq 0$

The **splitting** is directly related to the number of photogenerated carriers:

$$
\Delta E_F = E_{Fn} - E_{Fp} = k_B T \ln \left( \frac{n p}{n_i^2} \right)
$$

Where $n_i$ is the intrinsic carrier density.

* If $n p > n_i^2$, the splitting is positive → carriers are in **nonequilibrium**.
* If $n p = n_i^2$, then $\Delta E_F = 0$ → equilibrium.

---

### 3. **Summary**

* Photons generate **equal numbers of electrons and holes**, but:

  * They disturb the **energy distribution** → electrons go up in energy, holes go down.
  * Recombination has not yet balanced generation → nonequilibrium.
* The **quasi-Fermi level splitting** is the direct measure of this nonequilibrium.

---
