# DC Power Supply Design 

## Project Overview
Designed and built a regulated DC power supply converting 120V RMS AC to 3V ± 0.1V DC at 10mA. The project involved theoretical calculation, PSpice simulation, and physical implementation with real-world component constraints.

---

## Technical Implementation

### Power Stages
- **Transformer:** Center-tapped design for dual-phase AC conversion
- **Rectifier:** Full-wave center-tapped topology using two diodes (0.72V drop)
- **Filter:** RC configuration with 100μF capacitor
- **Load:** 330Ω resistor (adapted from theoretical 300Ω due to availability)

### Key Specifications
- **Input:** 120V RMS, 1kHz AC
- **Output:** 3V ± 0.1V DC, 10mA target
- **Ripple:** < 0.1V peak-to-peak
- **Peak Voltage:** 3.1V accounting for diode losses

---

## Validation & Results

### Simulation (PSpice)
- **Output Range:** 2.99V - 3.03V (within specification)
- **Current:** Proportional to voltage as expected
- **Validation:** Confirmed design viability before physical build

### Physical Implementation
- **Output Achieved:** 2.92V - 3.08V
- **Current Delivered:** 8.85mA - 9.33mA (with 330Ω load)
- **Challenge:** Required input voltage adjustment from 3.77V to 4V due to component tolerances

---

## Key Skills
- **Circuit Design** - Power supply architecture and component selection
- **PSpice Simulation** - Transient analysis and performance prediction
- **Practical Adaptation** - Working with real component limitations
- **Measurement Techniques** - Oscilloscope operation and waveform analysis
- **Safety Analysis** - Component rating verification and hazard prevention

---

## Tools & Technologies
- **Simulation:** Cadence PSpice
- **Hardware:** Digilent Analog Discovery 3, breadboard prototyping
- **Components:** Discrete diodes, capacitors, resistors from lab kit

*Project completed for ELEC ENG 2EI4 at McMaster University*
