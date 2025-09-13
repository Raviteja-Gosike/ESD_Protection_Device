# ESD Protection Device – D1Z1-D2 Diode Design for Automotive Applications

This repository contains the research work and supporting materials for designing a **low-capacitance, high-performance ESD protection device** tailored for 15V Local Interconnect Network (LIN) transceivers in automotive systems. The work was conducted as part of a research initiative at the **Department of Electrical Engineering, IIT Gandhinagar**.

---

## Project Overview

Electrostatic Discharge (ESD) events, resulting from sudden electrical surges, can permanently damage integrated circuits in electronic devices. Automotive systems, particularly LIN transceivers operating at 15V, require ESD protection devices that provide **low clamping voltage** and **low capacitance** to preserve signal integrity while ensuring device reliability.

This project presents a **3-diode D1Z1-D2 structure** that enables independent tuning of capacitance and dynamic resistance without compromising the required breakdown voltage. Through TCAD-based simulations, the design demonstrates:

✔ ~64% reduction in capacitance  
✔ ~38% reduction in dynamic resistance  
✔ Maintained 15V breakdown voltage for robust protection  

---

## Problem Statement

High capacitance in conventional ESD protection diodes causes significant insertion loss and limits frequency performance, degrading signal quality. Automotive communication networks such as LIN buses are particularly vulnerable to such disturbances.

**Key challenges addressed in this project:**
- Balancing low capacitance with effective ESD protection
- Achieving low clamping voltage without increasing device area
- Optimizing geometry through oxide width and P+ diffusion tuning

---

## Objectives

- Develop an ESD protection diode structure with minimal parasitic capacitance
- Maintain low clamping voltage to prevent device breakdown
- Use geometry optimization (oxide length and P+ diffusion) to independently tune capacitance and resistance
- Validate performance through TCAD simulations (TLP and CV analyses)

---

## Repository Structure

- **`SISPAD_3Diode.pdf`** – Research paper submitted to SISPAD 2025, detailing design methodology, simulation results, and conclusions.
- **`ESD_Poster.pdf`** – Visual presentation summarizing the key aspects of the project for conferences or workshops.
- **`README.md`** – This documentation outlining the project, methodology, and results.

---

## Technical Background

### Single Diode Limitations
A single PN junction diode with large area offers low clamping voltage but results in high junction capacitance, which degrades communication signals.

### D1Z1-D2 Structure
The proposed three-diode structure separates clamping and capacitance functions by:
- Using a small-area diode (D1) for forward current paths
- Enlarging Z1 area to improve ESD protection without increasing capacitance
- Using a lower breakdown diode (D3) to manage reverse stress events

### Geometry Optimization
- **Oxide Length Tuning**: Reduces junction capacitance by increasing the effective oxide area, thus lowering parasitic effects without compromising breakdown voltage.
- **P+ Diffusion Optimization**: Independently adjusts dynamic resistance while preserving current capacity and reliability.

---

## Simulation Results

✔ Achieved **6 fF/µm² capacitance**, compared to 16.5 fF/µm² in conventional designs  
✔ Reduced dynamic resistance to **282.5 Ω-µm**, compared to 455.56 Ω-µm  
✔ Maintained robust **15V breakdown** under stress conditions  
✔ Confirmed through **TCAD simulations** using TLP and CV analyses

---

## 📂 Figures & Diagrams

- Cross-sectional views of conventional and proposed diode structures  
- TLP I–V characteristics showing ESD event handling  
- Capacitance vs oxide length plots  
- Dynamic resistance vs P+ diffusion length results  
- Comparative analysis between conventional and optimized structures

*(Figures available in the PDF files attached to this repository.)*

---

## How to Reproduce

1. Use TCAD tools to model the D1Z1-D2 structure with tunable oxide width and P+ diffusion.
2. Validate breakdown behavior and extract capacitance through CV simulations.
3. Perform TLP simulations to study current stress and resistance under ESD events.
4. Analyze performance metrics such as clamping voltage, junction capacitance, and dynamic resistance.

---

## Tools & Technologies

- **TCAD (Technology Computer-Aided Design)** – Used for device simulation and performance extraction  
- **TLP (Transmission Line Pulse) Analysis** – For evaluating transient current response  
- **CV (Capacitance-Voltage) Analysis** – For extracting parasitic capacitance profiles  
- **IIT Gandhinagar Facilities** – Support from C2S project and MEITY, Government of India

---

## References

1. Oberti, Franco, et al. “LIN-MM: Message Authentication in Road Vehicles,” IEEE, 2022  
2. Kocon, Christopher, et al. “High-Current ESD Protection Devices,” U.S. Patent 17/855,105, 2023  
3. iFixit, "ESD Basics" [https://www.ifixit.com/Wiki/ESD]  
4. Toshiba, "Basics of TVS Diodes" [https://toshiba.semicon-storage.com/ap-en/semiconductor/knowledge/e-learning/basics-of-tvs-diodes.html]  
5. A. A. Rahman, "ESD Protection Methods," U.S. Patent US20230223395A1

---

## Future Work

- Extend design into **3D geometries** for advanced capacitance tuning  
- Explore applications in **CAN, USB, and IoT transceivers**  
- Investigate new diode shapes for **finer control over parasitic effects**  
- Explore material innovations for higher current capacity and thermal management

---

## Acknowledgments

This research was supported by:
- Faculty guidance by **Prof. Sandip Lashkare**  
- Research collaboration with **Navin Maheshwari and Sachin Kumar Jha from IIT Gandhinagar**

---

## Contact

**Gosike Raviteja**  
GitHub: [Raviteja-Gosike](https://github.com/Raviteja-Gosike)  
Email: *gosike.teja@iitgn.ac.in*

---

Feel free to explore the PDFs, understand the methodology, and contribute to advancing ESD protection solutions in modern automotive electronics.
