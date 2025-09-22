
---

## **1. EPSC – Excitatory Post-Synaptic Current**

* **Meaning:** Current **increases** in response to a stimulus (e.g., light pulse).
* **In a photodetector:**

  * When photons hit the channel, electron–hole pairs are generated.
  * The generated carriers increase the channel conductivity → **drain current rises**.
* **Characteristic:** Positive-going transient; sometimes decays slowly due to trap states.

**Equation (typical form, simplified):**

$$
I_{\rm EPSC}(t) = I_0 + \Delta I \, e^{-t/\tau}
$$

* $I_0$ = baseline current
* $\Delta I$ = photocurrent amplitude
* $\tau$ = relaxation/decay time

---

## **2. IPSC – Inhibitory Post-Synaptic Current**

* **Meaning:** Current **decreases** in response to a stimulus.
* **In a photodetector:**

  * Could occur if light induces **trapping of carriers** that reduces free carriers in the channel.
  * Or if a material has **photo-gating** effects that suppress conduction.
* **Characteristic:** Negative-going transient; current dips below baseline.

**Equation (simplified):**

$$
I_{\rm IPSC}(t) = I_0 - \Delta I \, e^{-t/\tau}
$$

---

## **Key Difference**

| Feature          | EPSC                                          | IPSC                                      |
| ---------------- | --------------------------------------------- | ----------------------------------------- |
| Current change   | Increases                                     | Decreases                                 |
| Sign of response | Positive                                      | Negative                                  |
| Mechanism        | Photogenerated carriers increase conductivity | Traps or photo-gating reduce conductivity |
| Analogy          | Excitatory neuron response                    | Inhibitory neuron response                |

---

💡 **In short:**

* EPSC → “light turns **on** current”
* IPSC → “light turns **off** current”

This is especially important in **photonic neuromorphic devices**, where light pulses emulate neural signaling.

---

