
---

## **Summary of the Work**

**link**: [note.pptx](./note.pptx)

**Title:** *Emulation of Optoelectronic Synaptic Behavior in a MoS2/WSe2‑Based p−n van der Waals Heterostructure Memtransistor*

**Authors:** Xiaodong Wang, Fengxiang Chen, Xiaoli Li, Tao Xiang, Lisheng Wang

**Journal:** ACS Applied Electronic Materials, 2024

**Key Idea:**
This work reports a **MoS2/WSe2 p–n van der Waals heterostructure memtransistor** that mimics biological synaptic behavior under both electrical and optical stimuli. By combining the nonvolatile memory effects of memristors with transistor functionality, the device demonstrates tunable resistive switching and optoelectronic synaptic behaviors, making it promising for **neuromorphic visual computing**.

**Key Findings:**

1. **Device Fabrication and Characterization:**

   * MoS2 (10 nm) and WSe2 (6.5 nm) layers were exfoliated and stacked to form the heterostructure.
   * Raman and PL spectra confirmed the quality of the materials.
   * SEM and AFM revealed the surface morphology and thickness.

2. **Resistive Switching (RS):**

   * The device exhibits **bipolar RS** with a switching ratio of \~10³ over 30 cycles.
   * RS arises from **Schottky barrier modulation** and **trap saturation** in the 2D channel.
   * Space-charge-limited current (SCLC) behavior observed at higher biases.

3. **Electrical Synaptic Behavior:**

   * Emulated EPSC/IPSC, LTP/LTD, paired-pulse facilitation (PPF), and spike-rate-dependent plasticity (SRDP).
   * EPSC/IPSC amplitudes can be tuned via gate voltage.
   * PPF index shows decay characteristics similar to biological synapses (τ₁ = 0.23 s, τ₂ = 11.22 s).

4. **Optoelectronic Synaptic Behavior:**

   * Device responds to optical pulses at different wavelengths, power densities, and pulse widths.
   * Short-term to long-term memory transition simulated by modulating light pulse parameters.
   * Learning, forgetting, and relearning behaviors were mimicked.
   * Optical PPF index reached 180%, higher than electrical stimulation.

5. **Visual Neuromorphic Simulation:**

   * Simulated light adaptation by controlling device current via illumination and gate voltage.
   * High-frequency light pulses induce potentiation; low-frequency pulses cause depression (SRDP).
   * Experience-dependent SRDP demonstrated memory of previous stimulation frequencies.

6. **Conclusion:**

   * MoS2/WSe2 memtransistors are capable of **multifunctional synaptic emulation**.
   * They provide a platform for **visual neuromorphic computing**, combining electrical and optical inputs for flexible synaptic modulation.

---

## Materials, method and device Characterization
* [method.md](./docs/method.md)

---

## **Figure-by-Figure Analysis**

**Figure 1 – Device Characterization**

* **(a)** Schematic of the MoS2/WSe2 memtransistor. Shows the p–n heterojunction and three terminals (gate, source, drain).
* **(b)** Output curves under 5 V gate bias and 600 nm light. inset is the log scale plot.
* **(c)** SEM image of device structure. Confirms heterostructure stacking.
* **(d)** AFM image showing MoS2 (\~10 nm) and WSe2 (\~6.5 nm) thickness.
* **(e,f)** Raman spectra of MoS2 and WSe2 confirm characteristic vibrational modes ($E_{2g}^1$, $A_{1g}$, $B_{2g}^1$).
* **(g,h)** PL spectra: MoS2 peak at 680 nm, WSe2 at 780 nm, confirming optical activity.

---

**Figure 2 – Resistive Switching & Optoelectronic Characterization**

* **(a)** Ids–Vds curves over 30 cycles: shows bipolar switching (HRS↔LRS), stable over repeated cycles.
  * [bipolar vs ambipolar](./docs/fig2-2.md)
* **(b)** Log–log plot: HRS shows I ∼ V² (Child’s law), high-bias shows SCLC behavior.
  * [fig2.md](./docs/fig2.md)
  * [SCLC I-V relation](../../mos2/mos2_1/note.md)
    * *Observation of trap-assisted space charge limited conductivity in short channel MoS2 transistor*
* **(c,d)** Energy band diagrams before and after MoS2/WSe2 contact, showing Schottky barriers and trap states.
* **(e)** Band diagram under illumination: photogenerated carriers reduce barrier height, enhancing current.
* **(f)** Transfer characteristics at Vds = 1 V: increasing gate voltage range enhances hysteresis, confirming gate modulation.
* **(g)** Ids–Vds under various wavelengths: strong response at 400 and 600 nm due to optical absorption.

---

**Figure 3 – Electrical Synaptic Simulations**

* **(a)** Schematic of artificial synapse using the memtransistor.
* **(b)** EPSC/IPSC: EPSC increases with positive gate pulses, IPSC decreases with negative pulses.
  * explanation: [EPSC & IPSC](./docs/fig3.md)
* **(c)** LTP/LTD: sequential pulses modulate device conductance.
* **(d)** Endurance test: 10 consecutive LTP/LTD cycles show stable conductance changes.
* **(e)** PPF index vs pulse interval: shorter intervals enhance facilitation. Inset shows PSCs for two pulses.

---

**Figure 4 – Optical Synaptic Simulations**

* **(a)** EPSC response to light pulses of 400, 500, 600 nm: stronger response at shorter wavelengths.
* **(b,c)** EPSC under varying pulse intensity and width: higher intensity or longer width promotes STM → LTM transition.
* **(d,e,f)** EPSC for consecutive light pulses: more pulses or higher intensity yield stronger, longer-lasting responses.
* **(g)** Learning, forgetting, relearning: device mimics neural memory formation.
* **(h)** PPF index vs pulse interval for optical pulses: higher PPF (180%) than electrical pulses; decays with increasing interval.
* explanation of LTM
  * [fig4.md](./docs/fig4.md)
---

**Figure 5 – Light Adaptation Simulation**

* **(a)** Mild illumination: Ids < 40 nA, below threshold.
* **(b)** Strong illumination: Ids > 40 nA.
* **(c)** Negative gate voltage under strong illumination suppresses current below threshold, simulating eye light adaptation.
  * Light adaptation of human vision: adjusting the pupil size and controlling the light sensitivity of the retina
    To avoid damage from strong illumination, the optical sensitive cells in the visual system will self-regulate to adapt to the bright light environment

---

**Figure 6 – Spike Frequency & Experience-Dependent Plasticity**

* **(a)** SRDP: High-frequency pulses (10 Hz) cause potentiation; low-frequency (0.5 Hz) induce depression.
* **(b)** Experience-dependent SRDP: Synaptic weight depends on previous stimulation history; demonstrates memory retention of previous frequencies.

---

