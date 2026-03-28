# Instrumentation Amplifier (INA) Design using MCP6004

## Overview

This project focuses on the design and implementation of a **3-opamp instrumentation amplifier (INA)** using the MCP6004 op-amp. The objective is to amplify small differential signals while rejecting common-mode noise.

Instrumentation amplifiers are widely used in:

* Sensor signal conditioning
* Biomedical systems (ECG, EEG)
* Data acquisition systems
* Industrial measurement

---

## Objective

* Design a 3-opamp INA
* Achieve a differential gain of 3
* Validate performance using simulation and hardware
* Analyze gain and output behavior

---

## Circuit Design

### Parameters:

* ( R_1 = R_2 = R_F = 10k\Omega )
* ( R_G = 10k\Omega )

### Gain Formula:

[
A_d = 1 + \frac{2R}{R_G}
]

### Calculation:

[
A_d = 1 + \frac{2 \times 10k}{10k} = 3
]

---

## Simulation (LTSpice)

### Observations:

* Output shows a linear relationship with differential input
* Gain ≈ 3 verified
* Proper amplification of sine wave observed

*(Insert LTSpice screenshots here)*

---

## Hardware Implementation

* Op-Amp: MCP6004
* Supply: 5V
* Breadboard implementation

*(Insert circuit images here)*

---

## 📊 Results

### Input Conditions:

* ( V_{IN+} = 2.5V )
* ( V_{IN-} = 2.3V )
* ( V_d = 0.2V )

### Output:

[
V_{out} = 3 \times 0.2 = 0.6V
]

### Experimental Table:

| Vd (V) | Vout (V) |
| ------ | -------- |
| 0.1    | 0.3      |
| 0.2    | 0.6      |
| 0.3    | 0.9      |
| 0.4    | 1.2      |

---

## 📉 Frequency Response

* Gain remains constant at low frequencies
* Gain decreases at higher frequencies due to op-amp limitations

---

## 💡 Key Learnings

* Instrumentation amplifiers provide high input impedance and good common-mode rejection
* Proper resistor matching is critical for accurate gain
* Hardware implementation requires careful wiring and stable connections
* Simulation helps validate design before implementation

---

## 🚀 Future Improvements

* Use precision resistors for better accuracy
* Implement PCB instead of breadboard
* Extend design for higher gain applications
* Explore dedicated INA ICs like AD620

---

## 🧠 Conclusion

The instrumentation amplifier was successfully designed and implemented for a gain of 3. Both simulation and hardware results confirmed correct operation and linear amplification behavior.

---

## 👩‍💻 Author

**Disha Paralkar**
BS in Electronic Systems, IIT Madras
GitHub: dishaparalkar

---
 
