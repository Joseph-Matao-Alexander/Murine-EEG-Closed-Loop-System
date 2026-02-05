# Murine Closed-Loop EEG & Automated Pharmacotherapy System

A specialized neural engineering project designed for real-time EEG monitoring and automated drug delivery in murine (mouse) models. The system detects specific brain wave patterns and triggers a thermal-release mechanism to administer medication.



## 🧠 System Logic: "The Closed-Loop"
1. **Signal Acquisition:** The system monitors EEG waves via electrodes attached to the murine subject.
2. **Analysis:** The onboard MCU processes the signal to identify target brain activity (e.g., seizure markers).
3. **Trigger:** Once the signal threshold is met, the MCU activates the heating component.
4. **Drug Delivery:** The heating element melts a specialized jelly-based medicine, releasing it to the subject.
5. **Feedback:** A temperature sensor ensures the heating remains within safe, biocompatible limits to prevent tissue damage.

## 🛠 Hardware Architecture
* **MCU:** Central processing unit for signal analysis and thermal control logic.
* **Heating Component:** Integrated PCB resistor/pad designed for controlled thermal release.
* **Temperature Sensor:** High-precision sensor for real-time feedback and safety cutoff.
* **EEG Analog Front-End:** Precision amplification and filtering for microvolt-level brain signals.

## 📂 Repository Contents
* `/Murine-EEG-Closed-Loop-System.pdf`: Full technical project report and design specifications.
* `/Mouse_Project.PcbDoc`: Altium Designer PCB layout files.
* `/Mouse_Project.SchDoc`: Schematic diagrams showing the MCU-to-Heater interface.
* `/Gerber/`: Manufacturing files for the PCB.

## 🔬 Safety & Biocompatibility
The system is designed to be head-mounted. The closed-loop algorithm includes a "Thermal Guard" feature: the MCU continuously polls the temperature sensor to ensure the heating element never exceeds the programmed safety threshold, protecting the subject while ensuring effective drug release.