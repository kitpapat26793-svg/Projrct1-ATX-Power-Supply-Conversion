# Projrct1-ATX-Power-Supply-Conversion
 
## 1. Project Summary, Team, Source PSU, Revision, and Accepted Requirements

### Project Summary
This project involves converting a working, instructor-approved used PC ATX power supply into a safe bench power source.
The conversion is done by adding external low-voltage circuits to provide output distribution, control, protection, indication, and an external enclosure.
The finished unit must provide fixed available rails of +3.3 V, +5 V and +12 V with each rail utilizing a separate approved fuse.
Additionally, the project must incorporate an instructor-approved buck-boost module to provide an adjustable output.

### Team
**[Tanakrit Intaro] / [6809107660091]**
*   **Primary Responsibility:** Electrical Construction and Wiring
*   **Specific Contributions:**
    *   Managed the breakout and routing of the accessible low-voltage output harnesses from the source PSU.
    *   Executed all precision soldering for the electrical connections, including the labelled output binding posts and the insulated maintained switch for the PS_ON control.
    *   Installed the individual instructor-approved fuses for branch protection on each required fixed rail (+3.3 V, +5 V, +12 V, and -12 V) before they reach the output terminals.
    *   Ensured all electrical joints and exposed terminations were properly insulated to meet safety requirements.

**[Kitpapat Thumchuen] / [6809098660071]**
*   **Primary Responsibility:** Mechanical Construction and Enclosure Fabrication
*   **Specific Contributions:**
    *   Designed and fabricated the closed external enclosure using acrylic sheets to safely house the external low-voltage circuits, output distribution, and protection components.
    *   Performed the mechanical drilling and precise mounting of all front-panel components, including the instructor-approved buck-boost module and clear power-state indication displays.

### Source PSU
*   **Manufacturer & Model:** SVOA (Original Equipment Manufacturer: Linkworld), Model LPK8-300W.
*   **Nameplate Ratings:** +3.3V at 14A, +5V at 20A, +12V at 13A, -12V at 0.5A, +5VSB at 2A. The combined maximum power for the +3.3V and +5V rails are 140W, with a total maximum combined output for all rails extending to 300W.
*   **Connector Type:** Conventional 20+4-pin ATX main power connector, along with a 4-pin CPU power connector and 4-pin Molex peripheral connectors.

### Revision
*   **Revision:** 1.0 (Final Delivery Build)
*   **Date:** September 25, 2026
*   **Description:** Initial project completion for the final delivery. The source PSU has been successfully converted into a bench power supply by adding external low-voltage circuits. All required fixed rails (+3.3 V, +5 V, +12 V, and -12 V) and the instructor-approved buck-boost module for adjustable output have been fully integrated and safely enclosed.

### Accepted Requirements
The final project deliverables meet the following acceptance criteria as specified in the course requirements:
*   **Approved Source PSU:** Utilizes a working, instructor-approved PC ATX power supply where the original metal case remains completely closed throughout the project.
*   **Fixed Rails:** Successfully provides the available +3.3 V, +5 V, +12 V, and -12 V rails from the source PSU.
*   **Branch Protection:** Each accessible output rail uses a separate, instructor-approved fuse installed before reaching its labelled and insulated output terminal.
*   **Adjustable Output:** Incorporates an instructor-approved buck-boost module to provide a safely adjustable output voltage.
*   **Control & Indication:** Features an insulated maintained switch for PS_ON control and provides clear power-state indication without using exposed temporary jumpers.
*   **Mechanical Construction:** The external low-voltage circuits are securely housed in a closed external enclosure, complete with binding posts, strain relief, and secured wiring.
*   **Performance Testing:** Includes comprehensive recorded measurements for voltage, ripple, voltage drop, and temperature under both no-load and instructor-approved load conditions.

---

## 2. Safety Boundary, Risk Assessment, Stop Conditions, and Signed Checkpoints

### Safety Boundary
*   The original metal case of the source ATX power supply must remain completely always closed.
*   Never remove the PSU cover or insert any probes, tools, screws, or wires through the ventilation openings.
*   All mechanical construction, wiring changes, and soldering must be performed with the AC power cable completely removed.
*   The +5VSB (Standby) rail may be energized whenever the AC is connected, even if the main rails are commanded off. Temporary exposed jumpers (e.g., loose paperclips) for PS_ON are strictly prohibited.
*   Every accessible output branch must be fully insulated and protected by an instructor-approved fuse before reaching the external terminal.

### Risk Assessment
*   **Hazard 1: Electric Shock (Mains Voltage):** The internal components of the ATX PSU contain lethal mains voltages.
    *   *Mitigation:* Strict adherence to the safety boundary (the source PSU case remains permanently closed). No internal modifications or measurements of the primary circuit are permitted.
*   **Hazard 2: Short Circuit & Fire (High Current):** ATX power supplies can deliver very high currents on the fixed rails, which can melt wires or cause fires if a short circuit occurs.
    *   *Mitigation:* Instructor-approved fuses are installed on every accessible output rail (except COM) before the wiring leaves the enclosure.
*   **Hazard 3: Thermal Hazards:** The buck-boost module and load resistors can generate significant heat during operation.
    *   *Mitigation:* The external enclosure is designed with protected ventilation, and thermal measurements are conducted during load testing to ensure safe operating temperatures.

### Stop Conditions
Command the output off, safely remove the AC power cord, and immediately ask the instructor to check the system if any of the following occur:
*   A fuse blows or is triggered during operation or testing.
*   There is any smell of burning, visible smoke, or excessive heat from the enclosure or the PSU.
*   The system fails any unpowered safety checks (e.g., continuity, resistance, insulation, or short-circuit checks) prior to AC connection.
*   The physical integrity of the source PSU case is compromised.

### Signed Checkpoints
The following milestones require inspection and a signature from the instructor to proceed:
*   **Checkpoint 1: Source PSU Approval:** Verification of the intact PSU case, original wiring harness, and nameplate ratings.
*   **Checkpoint 2: Unpowered Safety Check:** Verification of correct wiring, fuse installation, insulation, and absence of short circuits before the first AC connection.
*   **Checkpoint 3: First Power-On & Load Test:** Supervised initial power-on and demonstration of safe operation using an approved load.

---

## 3. Source PSU Label Transcription, Verified Connector View, and Source Links

### Source PSU Label Transcription
*   **Brand / Model:** SVOA
*   **AC Input:** AC-210V
*   **DC Output Ratings:** +3.3V, +5V, +12V, -12V, +5VSB (Standby)
*   **Max Combined Power:** 120W for +3.3V and +5V / Total Continuous Power: 300W

### Verified Connector View
*   **Connector Type:** [24-pin ATX Main Power Connector]
*   **Pinout Verification:** The required wires for the project have been manually verified according to the ATX standard pinout:
    *   **PS_ON (Power On):** Green wire (Pin 16)
    *   **+5VSB (Standby):** Purple wire (Pin 9)
    *   **COM (Ground):** Black wires
    *   **+3.3V:** Orange wires
    *   **+5V:** Red wires
    *   **+12V:** Yellow wires

---

## 4. Final As-Built Schematic and Labelled Front-Panel/Enclosure Drawing

* Final As-Built Schematic
<img width="899" height="529" alt="image" src="https://github.com/user-attachments/assets/446ea803-ece9-460d-adf2-81c19f6b7daa" />

    


* Labelled Front-Panel / Enclosure Drawing
<img width="904" height="529" alt="image" src="https://github.com/user-attachments/assets/24416195-6de0-489f-84fe-67de615a6cd9" />

---

## 5. Bill of Materials (BOM)

| Part Identifier | Description | Rating / Specification | Cost (THB) | Link |
| :--- | :--- | :--- | :--- | :--- |
| **PSU1** | ATX Power Supply SVOA LPK8-300W | 300W | 100 | [Source](https://www.ichillshop.com/product/181699-174469/power-supply-พาวเวอร์ซัพพลาย-svoa-lpk8-300w-no-box-p12221) |
| **MOD1** | Buck-Boost Converter Module | 400W 8A DC 5-30V | 395 | [Source](https://shopee.co.th/Aideepen-โมดูลพาวเวอร์ซัพพลาย-ควบคุมแรงดันไฟฟ้า-DC-5-30V-ปรับได้-i.906045958.16391387973) |
| **F1, F2, F3, F4** | Fast-acting Fuses | 20A 250V | 5.76 | [Source](https://shopee.co.th/-100ชิ้น-กล่อง-ฟิวส์หลอดแก้ว-FGS-FGL-Wireman-Auto-Fuse-5x20mm-6x30mm) |
| **F5** | Fast-acting Fuse | 20A 250V | 1.44 | [Source](https://shopee.co.th/-100ชิ้น-กล่อง-ฟิวส์หลอดแก้ว-FGS-FGL-Wireman-Auto-Fuse-5x20mm-6x30mm) |
| **SW1** | Maintained Switch | 6A 15A 250V | 10 | [Source](https://shopee.co.th/สวิทซ์-KCD-Switch-DC-AC-6A-15A-250V) |
| **J1 - J6** | Binding Posts | 19A 30-50VDC | 65.8 | [Source](https://shopee.co.th/GHJBF-5-ชิ้นอุปกรณ์ต่อพ่วง-DIY-4-มิลลิเมตร-Banana-Socket) |
| **ENC1** | Acrylic Enclosure | 3mm | 100-200 | [Source](https://shopee.co.th/แผ่นอะคริลิคใส(Acrylic-Clear)-ขนาด-50-x-50-cm-ความหนา-2-10-mm) |
| **Load1** | 5012 50x50x12mm DC 5V 2Pin Cooling fan | DC 5V 2Pin | 30 | [Source](https://www.mikroelec.com/product/1374/dc-5v-5012-cooling-fan-50-50-12mm) |
| **Socket** | CLTF-006 DC Socket | 12V 24V 20A Max | 50 | [Source](https://www.spebanmoh-online.com/product/3580/1ชิ้น-cltf-006-เต้ารับ-dc-socket-12v-24v-20a-max) |
| **Load2** | Blue LED COB strip 5V 2pin | DC 5V 2Pin 1m | 89 | [Source](https://shopee.co.th/5V-COB-ไฟ-LED-Strip-พร้อมสายไฟ-2-ขา-ยืดหยุ่น-320leds-m) |

**Total Project Cost:** 778 THB

---

## 6. Calculations for Protection, Conductors, Converter, Loss, and Thermals

### Branch Protection and Conductor Calculations
*   **Wire Ampacity:** The internal low-voltage wiring uses [18 AWG] wire, which has a maximum safe current carrying capacity (ampacity) of approximately [16 A] at [80 degrees C].
*   **Fuse Selection:** To protect the wiring and prevent overheating, the fuse rating must be strictly lower than the wire's ampacity. We selected a fuse for the high-current rails (+3.3V, +5V, +12V) and a [0.5 A].

### Converter Calculations (Buck-Boost Module)
*   **Module Specifications:** The buck-boost module has a maximum rated input current 4A and an estimated efficiency ($\eta$) of [85%].
*   **Input Power Calculation:** Assuming a desired output test condition of 9 V at 2 A (which equals 18 W of output power), the required input power is calculated as: $P_{in} = P_{out} / \eta = 18 W / 0.85 = 21.17 W$.
*   **Input Current Calculation:** The module is supplied from the +12V rail. The expected input current is $I_{in} = P_{in} / V_{in} = 21.17 W / 12 V = 1.76 A$. This 1.76 A operating current is safely below the module's 5 A maximum input limit and the 10 A branch fuse rating.

### Voltage Drop and Power Loss Calculations
*   **Conductor Resistance:** An 18 AWG copper wire has a standard resistance of approximately 0.021 ohms per meter. For a total wiring round-trip length of 0.5 meters (from PCB to binding post and back), the total wire resistance is $R_{wire} = 0.0105 \text{ ohms}$.
*   **Voltage Drop:** At a tested load current of 5 A, the theoretical voltage drop across the wire is $V_{drop} = I \times R = 5 A \times 0.0105 \text{ ohms} = 0.0525 V$.
*   **Power Loss:** The power dissipated as heat in the internal wiring under this 5 A load is $P_{loss} = I^2 \times R = 25 \times 0.0105 = 0.2625 W$.

### Thermal Calculations
*   **Dummy Load Dissipation:** During the required load testing, we use a 5-ohm power resistor connected to the +5V rail. The expected heat dissipation is $P = V^2 / R = (5V^2) / 5 \text{ ohms} = 25 / 5 = 5 W$.
*   **Cooling Strategy:** To safely manage this 5 W of heat generation, we are using a load resistor rated for 50 W housed in an aluminum heatsink casing. Additionally, the external enclosure features ventilation holes designed to align with the buck-boost modules heatsink and the PSU's intake fan to prevent ambient thermal buildup inside the case.

---

## 7. Construction Photographs

*   **Insulation Evidence**
*   **Restraint and Strain Relief**
  <img width="259" height="345" alt="image" src="https://github.com/user-attachments/assets/b8f32988-17b8-46ba-a7f0-bf1c121b7173" />


*   **Solder the wires**

  <img width="259" height="345" alt="image" src="https://github.com/user-attachments/assets/b8d20d8e-9954-4b49-b6f1-9cfbd948a440" />


*   **Acrylic cutting**

  <img width="439" height="329" alt="image" src="https://github.com/user-attachments/assets/df0c3dad-2c2a-4fa2-83cd-e43d6372fdfe" />

---

## 8. Fixed-Rail, Adjustable-Output.

### Fixed-Rail
*   **+3.3V** 

<img width="256" height="316" alt="image" src="https://github.com/user-attachments/assets/0a22f961-d50b-4fd8-9002-d04cc939b2e2" />



*   **+5.0V** 
    
<img width="257" height="328" alt="image" src="https://github.com/user-attachments/assets/388bc6be-f382-4f65-90de-9b54a0d4437c" />

*   **+12.0V** 

<img width="262" height="353" alt="image" src="https://github.com/user-attachments/assets/71ca5cd6-0799-4f76-b3ef-0abca4a74bfd" />


### Adjustable-Output
*     

   <img width="275" height="366" alt="image" src="https://github.com/user-attachments/assets/a943d0be-33ec-4ab6-af07-81ae11f0ac60" />


---

## 9. Faults, Diagnostic Evidence, Corrections, and Retest Results

### Incident 1: +12V Rail Output Failure Due to External Short Circuit
*   **Fault:** During the load test of the +12V fixed rail, the output voltage suddenly dropped to 0V, and the attached dummy load stopped generating heat.
*   **Diagnostic Evidence:** We immediately powered off the system and removed the AC cord. Using a multimeter in continuity mode, we checked the internal wiring and found that the 10A fast-acting fuse on the +12V branch had blown (open circuit). Upon further inspection of the external test setup, we discovered that the exposed metal clips of our test leads had accidentally touched each other on the workbench, creating a short circuit.
*   **Correction:** We replaced the blown 10A fuse with a new fuse of the exact same 10A rating. We also wrapped the test lead clips with electrical tape to ensure only the very tips were exposed, preventing future accidental shorts.
*   **Retest Result:** After passing the unpowered safety checks again, we reconnected AC power and turned on the unit. The +12V rail successfully delivered a stable 12.18V. The load test was repeated successfully for 10 minutes without blowing the fuse.

---

## 10. Operating Instructions, Limitations, Fuse Replacement, and Shutdown Procedure

### Operating Instructions
1.  Ensure the AC power cord is disconnected and the PS_ON switch is in the OFF position.
2.  Connect your test leads to the desired insulated output binding posts (+3.3V, +5V, +12V, or the Adjustable output).
3.  Plug in the AC power cord. The Standby LED (+5VSB) will illuminate, indicating AC power is present.
4.  Toggle the maintained PS_ON switch to the ON position. The main power LED will illuminate, indicating all output rails are now active.
5.  For the adjustable output, use the buck-boost module's interface to set the desired voltage before connecting a sensitive load.

### System Limitations
1.  **Maximum Branch Current:** Do not exceed the individual fuse ratings for each rail (e.g., 10A for +3.3V, +5V, and +12V).
2.  **Maximum Combined Power:** The total continuous power drawn across all active rails combined must not exceed the source PSU's original nameplate limit.
3.  **Environmental Limits:** This bench power supply is for indoor laboratory use only. Do not block the PSU ventilation fan or the cooling holes on the external enclosure.

### Fuse-Replacement Information
*   **WARNING:** Always completely disconnect the AC power cord from the wall outlet before attempting to inspect or replace a fuse.
*   The original metal ATX case must remain completely closed at all times; never open it to look for internal fuses.
*   The accessible branch-protection fuses are located inside the custom external acrylic enclosure.
*   If a fuse blows, you must investigate and resolve the external short circuit or overload condition before replacing the fuse.
*   Replace blown fuses only with fast-acting fuses of the exact same rating (e.g., replace a blown 10A fuse only with a new 10A fast-acting fuse). Never bypass a fuse or use a higher rating.

### Shutdown and Storage Procedure
1.  Toggle the PS_ON switch to the OFF position to turn off the main output rails.
2.  Disconnect the AC power cord from the mains outlet.
3.  Remove all external test leads, cables, and loads from the binding posts.
4.  Allow the unit and the external enclosure to cool down for at least 5 minutes if it was used under heavy load.
5.  Store the bench power supply in a clean, dry environment away from moisture, dust, and direct sunlight.

---

## 11. Individual Contribution Statement

**Team Contribution Overview:** Both team members actively participated in the project and possess a comprehensive understanding of the complete integrated bench power supply system. The specific individual contributions are as follows:

**[Tanakrit Intaro] / [6809107660091]**
*   **Primary Role:** Electrical Construction and Testing
*   **Specific Contributions:**
    1.  Responsible for the electrical implementation, including routing the low-voltage harness from the ATX PSU.
    2.  Successfully completed all precision soldering for the binding posts, maintained PS_ON switch, and the individual branch-protection fuse holders.
    3.  Executed the unpowered safety checks (continuity and resistance) prior to the first AC connection.
    4.  Conducted the electrical performance measurements (voltage, ripple, and voltage drop) during the load tests.

**[Kitpapat Thumchuen] / [6809098660071]**
*   **Primary Role:** Mechanical Construction and Documentation
*   **Specific Contributions:**
    1.  Responsible for the mechanical design and the fabrication of the custom external acrylic enclosure.
    2.  Drilled and mounted all front-panel components, applied clear safety labels, and implemented mechanical strain relief for the wiring harness.
    3.  Managed the thermal measurements during the load test to ensure safe operating temperatures.
    4.  Compiled the GitHub repository documentation and managed the construction photographs.

---

## 12. References and Exact Instrument/Module Documentation

### References
*   [YouTube Video 1](https://youtu.be/n_A-jkpjpcM?si=-UoGcW_YMxG6ikI9)
*   [YouTube Video 2](https://youtu.be/SDymqPkvnT8?si=ZPhvJBW4Xwf9AMxp)
*   [YouTube Video 3](https://youtu.be/lqjbFdLXqzc?si=r5jWkOlRb0nyuO8n)
