# ⚡ Power Converter PCB

Designed and validated a 5V-to-3.3V Low Dropout (LDO) regulator in Altium Designer, executing the complete PCB design flow from schematic capture and ERC validation to PCB layout, routing, and Gerber X2 file generation.


## 
The design was based on the MIC5317 LDO, selected through datasheet analysis for the required output voltage and performance. The schematic implements the recommended application circuit, including proper input/output decoupling and layout considerations for stable operation.

<img width="953" height="441" alt="image" src="https://github.com/user-attachments/assets/6bb8effb-48cd-448c-97f2-864c1a9c7266" />


`LDO_Schematic.SchDoc`:
<img width="1232" height="408" alt="image" src="https://github.com/user-attachments/assets/55453714-05b0-4b89-9761-8315b1166069" />
Two SM02b-GHS-TB(lf)(sn) connectors were added for input and output. The schematic successfully passed Electrical Rules Check (ERC).
After setting up the PCB, the components imported from the schematic were placed on the top layer in a compact layout. The board size was minimized, as this is a relatively small design. Routing was performed by connecting the 5V and 3.3V power nets on the top layer, while the GND net was implemented as a copper pour on the bottom layer, connected through vias..
`LDO_PCB.PcbDoc`:
<img width="1441" height="599" alt="image" src="https://github.com/user-attachments/assets/071f2a47-c5e8-47ba-bd7c-57f9b0b7711d" />
<img width="1516" height="645" alt="image" src="https://github.com/user-attachments/assets/8db76426-35cb-44fe-b30d-d33397ac5b17" />
Before finalizing the PCB and exporting the Gerber X2 files, a Design Rules Check (DRC) was performed. All warnings and errors were reviewed and corrected to ensure manufacturability and compliance with design constraints.



This PCB was developed by following a <a href="https://youtu.be/YTGzncKU5RY?si=9Ydo8GLXhMg-J4NR"> tutorial </a> and consulting Altium educational resources.
