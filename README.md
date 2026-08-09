# Sanjay S.

**Final-year ECE student, Chennai Institute of Technology and Applied Research** · CGPA 9.16

I design, simulate, and optimize superconducting quantum hardware — from single transmons to
flip-chip multi-qubit processors — along with the control electronics and design tooling around them.

[Portfolio](https://sanjaysuresh05.github.io) · [LinkedIn](https://www.linkedin.com/in/sanjay-s1325) · [sanjaysuresh1302@gmail.com](mailto:sanjaysuresh1302@gmail.com)

Currently a Research Intern with the **Quantum Technology Group at C-DAC Bengaluru**, and a Research
Assistant at **CQST, Chennai Institute of Technology** under Dr. Md. Manirul Ali. Aiming next at
graduate research in superconducting quantum hardware, in a group pushing the
fabrication-to-characterization loop forward.

---

## Selected results

| Design | Result |
|---|---|
| Single transmon + CPW readout resonator | f₀₁ **5.51 GHz**, anharmonicity **−377 MHz**, E_J/E_C **41.2**, g **119 MHz**, χ **3.89 MHz**, charge dispersion 62 kHz, simulated T₁ **46.1 µs** |
| 4-qubit flip-chip processor | Crosstalk **−37 dB → −55 dB**, T₁ **2.69–4.94 µs**, Q > **1.2 × 10⁵**, qubit frequencies 4.13–4.29 GHz |
| Dispersive shift (χ) optimizer | Agreement with Keysight ADS QuantumPro to within **0.04–0.6%**; 206-test automated suite |
| RSAF randomness attribution | **81.21%** mean generator-level confidence, Brier **0.16** (from 0.21), ensemble F1 **73.2%**, 37 sources / ~4.15 GB |

---

## Projects

### [4-Qubit Flip-Chip Transmon Processor](https://github.com/Sanjaysuresh05/4qubit-flipchip-processor)
*VLSID Design Contest 2026 — Finalist*

A 3D-integrated Q-chip/C-chip architecture in Qiskit Metal that physically separates qubits from
control and readout routing, cutting crosstalk without adding routing congestion. EM-verified in
Ansys HFSS and exported to GDS for fabrication.

`Qiskit Metal` `Keysight ADS QuantumPro` `Ansys HFSS` `GDS Export`

### [Dispersive Shift (χ) Optimizer for Superconducting Qubit Design](https://github.com/Sanjaysuresh05/dispersive-shift-optimizer)
*RIT Quant-A-Thon 2026 — Finalist, Team Transmon Titans*

A closed-form inverse-design engine that converts a target (f_q, f_r, χ) directly into a fabricable
transmon + readout-resonator geometry, replacing the usual forward simulate-and-tweak loop.
Fabricability gates report out-of-range targets rather than silently clamping them. Multi-fidelity
Bayesian optimization (Optuna TPE) runs an analytic → Q3D/MoM → HFSS+EPR ladder, reserving full EM
solves for verification only.

`Python` `Streamlit` `Optuna` `NumPy/SciPy` `Ansys HFSS` `Ansys Q3D` `Keysight ADS QuantumPro`

### [RSAF — Randomness Source Attribution Framework](https://github.com/Sanjaysuresh05/rsaf-randomness-attribution)
*SparQ Internship Program, QNu Labs · May–Jul 2026*

Attributes a binary randomness stream to an algorithmic (PRNG) or physical (TRNG/QRNG) source with a
calibrated confidence score rather than a pass/fail verdict. A 64-dimensional statistical fingerprint
per 512 KB window feeds a five-model tree ensemble with isotonic calibration and hierarchical
window → file → generator voting. My contribution centred on the ensemble layer and its evaluation.

`Python` `CatBoost` `XGBoost` `LightGBM` `scikit-learn` `SHAP`

### [Single Transmon Qubit with Integrated Readout Resonator](https://github.com/Sanjaysuresh05/transmon-qubit-design)
*Sep 2025*

The first fully EM-verified qubit design in the pipeline, and the baseline everything else builds on:
a transmon coupled to a coplanar waveguide readout resonator, with full EM simulation, capacitance
extraction, EPR analysis, and parameter validation against target.

`Qiskit Metal` `Ansys HFSS` `Ansys Q3D` `EPR Analysis`

### In progress

- **6-Qubit Planar Transmon Processor** — CPW bus and individual readout resonators; full 3D EM simulation with adaptive mesh refinement, EPR analysis and GDS export. `Qiskit Metal` `Ansys HFSS`
- **Optical Mask Design — Multi-Transmon Device** — Purcell-filter optimization for improved T₁, with PhD-researcher collaborators. `Qiskit Metal` `Ansys HFSS`
- **RFSoC Control Electronics for Superconducting Qubits** — RF ADC/DAC IP on Xilinx ZCU111 using the Zynq UltraScale+ RF Data Converter IP, AXI SmartConnect fabric and BRAM capture for IQ readout. `Verilog` `Xilinx Vivado`
- **Low-Power Multi-Function ALU — Full ASIC Flow** — RTL → Xcelium → Genus → Innovus → Tempus → DRC/LVS-clean layout. `Verilog` `Cadence`

---

## Experience

**Research Intern — Quantum Technology Group, C-DAC Bengaluru** · *Jan 2026 – Aug 2026*
- Designed and simulated superconducting qubits using Qiskit Metal, scQubits, KQCircuits, Ansys HFSS, Ansys Q3D and Keysight ADS QuantumPro
- Developed RF ADC, RF DAC and RF data-converter IP; studied NCO/AWG signal generation for quantum control electronics
- Worked hands-on with DPS-QKD photonic lab systems — lasers, optical couplers, polarization beam splitters, single-photon detectors — running photonic coincidence experiments

**Project Intern, RNG Randomness Quality Detection (ML) — SparQ Internship Program, QNu Labs** · *May 2026 – Jul 2026*
- Trained and tuned the five-model ensemble (CatBoost, XGBoost, LightGBM, Random Forest, Extra Trees) at the core of RSAF
- Benchmarked accuracy, precision, recall and F1 across 37 binary randomness sources (~4.15 GB), including QNu Labs' proprietary photonic QRNG output
- Framework reached 81.21% mean generator-level attribution confidence and a calibrated Brier score of 0.16, down from 0.21

**Research Assistant — Centre for Quantum Science and Technology (CQST), CIT** · *Oct 2023 – Present*
- Design and EM simulation of transmon qubits and readout resonators (Qiskit Metal, Ansys HFSS/Q3D)
- Studied Cooper-pair physics, Hamiltonian modeling and circuit quantization under Dr. Md. Manirul Ali
- Working on flip-chip integrated processors and Josephson-junction engineering for higher coherence

**VLSI Engineer — ULOG3, Chennai** · *Oct 2023 – Present*
- Contributed to OLI, an on-chip-learning neuromorphic processor — front-end RTL design and synthesis (Cadence Genus), validated on ZCU102 FPGA
- Designed and launched the ULOG-3 CubeSat to the stratosphere (Sep 2024): circuit design, power management, payload integration

---

## Recognition

- **Winner, MSME Idea Hackathon 4.0** — ₹15 Lakh award for a neuromorphic EO payload small satellite concept
- **Finalist, VLSID Design Contest 2026** — 4-qubit flip-chip transmon processor
- **Finalist, RIT Quant-A-Thon 2026** — dispersive shift (χ) optimizer, Team Transmon Titans
- **Finalist, Amaravati Quantum Valley Hackathon** — quantum ML fraud-detection prototype
- **ULOG-3 CubeSat** — designed, built and launched to the stratosphere, Sep 2024

---

## Tools

**Quantum hardware design** — Qiskit Metal, scQubits, KQCircuits, QuTiP, Cirq
**EM & RF simulation** — Ansys HFSS, Ansys Q3D, Keysight ADS, Keysight QuantumPro
**Machine learning** — CatBoost, XGBoost, LightGBM, scikit-learn, SHAP, Optuna, Streamlit
**FPGA & RFSoC** — Xilinx Vivado, Vitis, ZCU102, ZCU111, RF Data Converter IP, AXI
**VLSI / ASIC** — Cadence Genus, Innovus, Tempus, Virtuoso, Xcelium · Synopsys Design Compiler, Custom Compiler, HSPICE, VCS, Verdi · OpenLane, Yosys, Magic, KLayout
**Languages** — Python, Verilog, C, MATLAB · Linux

---

## Currently learning

- Transmon Hamiltonian in the E_J ≫ E_C regime — flux sweet spot, charge dispersion suppression
- Dispersive readout — χ shift, Purcell decay rate, optimal resonator linewidth κ
- Fluxonium in the heavy-fluxonium regime, and its coherence trade-offs against the transmon
- Multi-fidelity Bayesian optimization for closed-form inverse qubit design
- ZCU111 NCO and AWG pulse shaping for qubit drive and readout timing
- Timing closure in Innovus — setup/hold fixing, useful skew, ECO flow
