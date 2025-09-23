
---

## **Summary of the Work**

**Title:** Observation of trap-assisted space charge limited conductivity in short channel MoS₂ transistor

**Authors:** Subhamoy Ghatak, Arindam Ghosh

**Journal:** *Applied Physics Letters* 103, 122103 (2013)

**Key Idea:**
The study investigates the **high-bias** transport in short-channel single-layer MoS₂ transistors to determine whether current conduction is limited by traps in the material. By analyzing **temperature-dependent I–V characteristics**, the authors show that conduction transitions from **ohmic** to t**rap-assisted space charge limited conduction (SCLC)**, revealing the presence of an exponential distribution of trap states intrinsic to MoS₂.

**Key Findings:**

* At low VDS, conduction is ohmic; at higher VDS, it becomes SCLC.
* The current follows $I \propto V^m$, with $m \approx 2$ at room T, increasing as temperature decreases, consistent with exponential trap distribution.
* A temperature-independent critical voltage $V_c$ is observed, where I–V curves at different T intersect.
* From $V_c$, trap densities were quantified: $N_t \sim 1.5 – 2.3 \times 10^{17} \, \text{cm}^{-3}$.
* Increasing gate voltage lowers $V_c$, showing that gate-induced carriers pre-fill traps.
* The trap states likely originate from bulk MoS₂ disorder (sulfur vacancies, oxidation, structural inhomogeneity) rather than just substrate effects.

---

## Materials, method and device Characterization
* [method.md](./docs/method.md)


## **Key Equations from the Paper**

1. **Trap-free space charge limited current (Child’s law, 1D channel):**

$$
J_{MG} = \frac{9}{8} \ \varepsilon_0 \varepsilon_r \ \mu \ \frac{V^2}{L^3}
$$

* Mott-Gurney relation

* $J$: current density
* $\varepsilon_0$: vacuum permittivity
* $\varepsilon_r$: relative dielectric constant of MoS₂
* $\mu$: carrier mobility
* $V$: applied voltage (drain–source bias)
* $L$: channel length

---

2. **Trap-limited SCLC with an exponential trap distribution:**

$$
J = \frac{\mu N_c}{q^{\,m-2}} \ (\frac{2m - 1}{m})^m (\frac{\varepsilon_0 \varepsilon_r (m-1)}{N_t m})^l \ \frac{V^m}{L^{\,2m-1}}
$$

* $N_c$: effective density of states in conduction band
* $q$: elementary charge
* $m = \frac{T_c}{T} + 1$, where $T_c$ is the characteristic temperature of the exponential trap distribution
* $T$: measurement temperature

This captures the steeper-than-quadratic current scaling ($I \propto V^m$) at lower T due to traps.

---

3. **Critical voltage for trap filling (temperature independent):**

$$
V_c = \frac{q N_t L^2}{2 \ \varepsilon_0 \varepsilon_r}
$$

* $V_c$: voltage where all trap states are filled (intersection point of I–V curves at different T)
* $N_t$: trap density (per unit volume)

This equation is central for extracting trap density from experiment.

---

4. **Ohmic conduction (low bias, trap-limited conduction not yet active):**

$$
J = \sigma V / L
$$

where $\sigma = q n \mu$ is the conductivity with carrier density $n$.

---

## **Figure-by-Figure Analysis**

**Figure 1**

* **(a)** Schematic of two-probe single-layer MoS₂ device on Si/SiO₂ with Au contacts.
* **(b)** Transfer curve (ID–VBG at VDS=10 mV). Mobility extracted (0.3–2 cm²/Vs). Inset: SEM image of short-channel device (\~80–200 nm).
* **(c)** I–V curves at room T for different VBG. Linear and symmetric at low VDS, showing quasi-ohmic contacts.
  * work function:
    * $MoS_2$: 5.1 eV
    * $Au$: 4.5 eV
* **(d)** I–V curves at VBG=0 V across different T. Nonlinearity increases as T decreases, eliminate the effect of Schottky/tunneling effects (direct or Fowler-Nordheim tunneling)

**Takeaway:** Contacts are not limiting; the observed nonlinearity arises from SCLC.

---

**Figure 2**

* **(a)** Log–log I–V curves (room T, VBG=0). At low VDS slope = 1 (ohmic), at higher VDS slope → 2 (SCLC).
* **(b)** Temperature dependence: slope increases from \~1.7 (285 K) → 2 (205 K) → 3 (105 K).
* **(c)** Extrapolation of I–V curves at low T yields a T-independent critical voltage $V_c \approx 4.3 \, \text{V}$, giving trap density $N_t \approx 2.3 \times 10^{17} \, \text{cm}^{-3}$.

**Takeaway:** Confirms exponential trap distribution and provides a method to quantify trap density.

---

**Figure 3**

* **(a–c)** I–V curves at VBG = 0, 20, 40 V for multiple T. Intersection points (critical voltage) decrease with gate bias:

  * VBG=0 V → $V_c = 2.8 \, \text{V}$
  * VBG=20 V → $V_c = 2.2 \, \text{V}$
  * VBG=40 V → $V_c = 1.4 \, \text{V}$
* High gate voltage fills more traps at equilibrium, reducing effective trap density and lowering $V_c$.

**Takeaway:** Gate control confirms trap filling effect and further supports trap-assisted SCLC.

---
