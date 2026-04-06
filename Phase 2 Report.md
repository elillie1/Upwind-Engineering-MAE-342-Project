Phase 2 Report

**Table of Contents**

[**1\. Overview of the Final Design	3**](#1.-overview-of-the-final-design)

[1.1 System Function	3](#1.1-system-function)

[1.1.1 Overall Function	3](#1.1.1-overall-function)

[1.1.2 Expected Operating Conditions	3](#1.1.2-expected-operating-conditions)

[1.1.2.1 Mechanical/actuation	3](#1.1.2.1-mechanical/actuation)

[1.1.2.2 Performance and Safety Expectations	3](#1.1.2.2-performance-and-safety-expectations)

[1.2 System Decomposition	3](#1.2-system-decomposition)

[1.2.1 Blade-Hub Interface Subsystem	4](#1.2.1-blade-hub-interface-subsystem)

[1.2.2 Pitch Actuation Subsystem	4](#1.2.2-pitch-actuation-subsystem)

[1.2.3 Power Generation	5](#1.2.3-power-generation)

[**2\. Description of the Major Design Decisions and Changes Post-Phase One	5**](#2.-description-of-the-major-design-decisions-and-changes-post-phase-one)

[2.1 Design Additions	5](#2.1-design-additions)

[2.1.1 Center Hub Addition	5](#2.1.1-center-hub-addition)

[2.1.2 Thrust Bearing Addition	5](#2.1.2-thrust-bearing-addition)

[2.1.3 Rotation Mechanics Addition	6](#2.1.3-rotation-mechanics-addition)

[2.1.4 Ball Bearings Addition	6](#2.1.4-ball-bearings-addition)

[2.2 Design Amendments	6](#2.2-design-amendments)

[**3\. Detailed Explanation of Required Analyses	6**](#3.-detailed-explanation-of-required-analyses)

[3.1 Engineering Analyses Test	6](#3.1-engineering-analyses-test)

[3.2 Engineering Analyses Results	7](#3.2-engineering-analyses-results)

[3.2.1 Analysis Results	7](#3.2.1-analysis-results)

[3.2.1.1 Blade	7](#3.2.1.1-blade)

[3.2.1.1.1 CASE 1: 90 Pa (low wind scenario)	7](#3.2.1.1.1-case-1:-90-pa-\(low-wind-scenario\))

[3.2.1.1.2 CASE 2: 200 Pa (medium-high wind)	9](#3.2.1.1.2-case-2:-200-pa-\(medium-high-wind\))

[3.2.1.1.3 CASE 3: 360.6 Pa (high wind conditions)	11](#3.2.1.1.3-case-3:-360.6-pa-\(high-wind-conditions\))

[3.2.2 Analysis Notes	13](#3.2.2-analysis-notes)

[**4\. Discussion of Design for Assembly & 3D Printing	13**](#4.-discussion-of-design-for-assembly-&-3d-printing)

[4.1 Engineering Drawings	13](#4.1-engineering-drawings)

[4.1.1 Linear Translation Mechanism	13](#4.1.1-linear-translation-mechanism)

[4.1.1.1 Linear Handle (Crank)	14](#4.1.1.1-linear-handle-\(crank\))

[4.1.1.2 Linear Linkage	14](#4.1.1.2-linear-linkage)

[4.1.1.3 Linear Shaft	15](#4.1.1.3-linear-shaft)

[4.1.1.4 Linear Disc	16](#4.1.1.4-linear-disc)

[4.1.1.5 Radial Ball Bearing	16](#4.1.1.5-radial-ball-bearing)

[4.1.2 Structural Support	17](#4.1.2-structural-support)

[4.1.2.1 35mm Shaft	17](#4.1.2.1-35mm-shaft)

[4.1.2.2 Support Beam (With Bearing)	17](#4.1.2.2-support-beam-\(with-bearing\))

[4.1.2.4 Blade Carrier	19](#4.1.2.4-blade-carrier)

[4.1.3 Hub Mechanism	19](#4.1.3-hub-mechanism)

[4.1.3.1 Blade Linkage	19](#4.1.3.1-blade-linkage)

[4.1.3.2 Hub Bottom	20](#4.1.3.2-hub-bottom)

[4.1.3.3 Hub Top	21](#4.1.3.3-hub-top)

[4.1.3.4 Thrust Bearing	21](#4.1.3.4-thrust-bearing)

[4.1.3.4.1 Thrust Bearing Outer Top Above	21](#4.1.3.4.1-thrust-bearing-outer-top-above)

[4.1.3.4.2 Thrust Bearing Outer Top Below	22](#4.1.3.4.2-thrust-bearing-outer-top-below)

[4.1.3.4.3 Thrust Bearing Inner Hollow	23](#4.1.3.4.3-thrust-bearing-inner-hollow)

[4.1.3.5 Wind Turbine Blade	23](#4.1.3.5-wind-turbine-blade)

[**4.3 3D Assembly	24**](#4.3-3d-assembly)

[4.3.1 System Assembly	24](#4.3.1-system-assembly)

[4.3.2 Exploded View	25](#4.3.2-exploded-view)

[4.4 Basic Motion Study (Operation)	26](#4.4-basic-motion-study-\(operation\))

[**5\. Anticipated Risks and Weaknesses	26**](#5.-anticipated-risks-and-weaknesses)

[5.1 Anticipated Failure Modes	26](#5.1-anticipated-failure-modes)

[5.1.1 Actuator Failure	27](#5.1.1-actuator-failure)

[5.1.2 Linkage Failure	27](#5.1.2-linkage-failure)

[5.3 Anticipated Risks and Weaknesses	27](#5.3-anticipated-risks-and-weaknesses)

[5.3.1 Linkage-to-Blade Root Connections	27](#5.3.1-linkage-to-blade-root-connections)

[5.3.2 Blade Root-Hub Interface	28](#5.3.2-blade-root-hub-interface)

[5.3.3 Linkage Buckling Under Compression	28](#5.3.3-linkage-buckling-under-compression)

[**6\. References**](#6.-References)

# 

# 

# 1\. Overview of the Final Design 

## 1.1 System Function 

### 1.1.1 Overall Function 

The active pitch mechanism rotates each turbine blade about its blade-pitch axis (the blade root) to dynamically adjust the blade’s angle of attack relative to the incoming wind velocity. By dynamically controlling the pitch angle, the system:

- Optimizes power capture below rated wind speed by maintaining an optimal aerodynamic operating point (usually near the optimal tip-speed ratio and lift-to-drag ratio).  
- Regulates power and rotor speed at and above rated wind speed by pitching toward the feather to reduce torque caused by turbulent wind flows.  
- Reduces structural loads during large gusts, turbulence, emergency shutdowns, and start-up and shutdown procedures.  
- Allows for safe shutdown and powering-down operations by quickly pitching the blades to a low-torque condition.

In normal operating conditions, the turbine blade pitch will be positioned based on measured/estimated wind speed, rotor speed, generator power, and sometimes blade root bending moments.

### 1.1.2 Expected Operating Conditions 

#### 1.1.2.1 Mechanical/actuation 

- Pitch range: typically 0-90 degrees (often operated within \-5 to 30 degrees for better control, larger angles will be used to feather and/or shutdown operation).  
- Loads through the pitch joint: large combined aerodynamic bending moments. axial/radial forces, and fatigue cycles (will be detailed later).  
- Duty Cycle: very high cycle count over lifespan; design is relatively fatigue-critical.

#### 1.1.2.2 Performance and Safety Expectations 

- Accurate pitch positioning (will require closed-loop control)  
- High reliability (pitch is the primary safety function)  
- Fail-safe ability to reach the feather position at any point.

## 1.2 System Decomposition 

Figure 1: Model Assembly  
<img width="756" height="833" alt="Turbine3" src="https://github.com/user-attachments/assets/f601dd0c-7df2-4b60-a129-e10cab2b3fa2" /> 


### 1.2.1 Blade-Hub Interface Subsystem 

The blade-hub interface consists of a fixed shaft with a center hub bearing at the front attached to three wind turbine blades through bearings. About midway down the fixed shaft are two plates; the back one has fixed rotation but allows translation up and down the shaft. The front one is free to rotate and translate about the shaft. The two plates experience sliding friction between them as the front one rotates. The front plate is pinned to three coupler links, one for each blade, and the other side of the couplers is pinned to one side of the collar of each turbine blade. The end of the fixed shaft is attached to a fixed support that has a hole offset from the middle to allow for another shaft. This other shaft is fixed to the back plate, only allowing for translational motion along the axis of the fixed shaft

### 1.2.2 Pitch Actuation Subsystem 

The pitch of the turbine blades is controlled by the translating shaft. As it moves back and forth with the fixed shaft, the two plates will also translate, pushing and pulling the couplers attached to the turbine blades. This causes the blades to rotate about their pitch axis along with the bearings between the blades and the center hub. A linear actuator will be used to control the motion of the blade pitch, driven by data such as optimal pitch vs wind speed.

- Slider motion 19.95mm   
- distance from joint to axis of blade 14.46  
- 79.05 degrees of rotation

### 1.2.3 Power Generation 

To generate power, a motor is placed in the back attached to the shaft. To harness and use the energy produced by the wind turbine model, a 12V DC motor (500-1000 rpm) is used as a generator. A diode must be placed in line with the positive output lead to ensure no power is going back to the motor, potentially causing harm. A capacitor such as 1000μF is placed across the output terminals of the motor, and if needed, a DC-DC boost converter is used to provide a steady output voltage. For much better efficiency, a gearbox between the shaft and the generator could be used to increase the output speed of the shaft.

# 2\. Description of the Major Design Decisions and Changes Post-Phase One 

The final design has had two major changes from the initial design, as well as many smaller modifications.   
<img width="250" height="320" alt="MEE342 3blade turbine design" src="https://github.com/user-attachments/assets/3c2041e0-59cf-4f3d-ba27-358d92f4cd4e" /> <img width="250" height="320" alt="Screenshot 2026-03-25 175901" src="https://github.com/user-attachments/assets/fe960e6b-4c31-42bb-8c3f-ad63aa1ffa79" /> <img width="250" height="320" alt="Turbine3" src="https://github.com/user-attachments/assets/b747c12b-c552-428d-93b9-1351f91b9537" />

   Figure 2: Phase 1 Design	                                         Figure 3: 1st Major Update                                                               Figure 4: Final Assembly

## 2.1 Design Additions 

### 2.1.1 Center Hub Addition 

A center hub was added to house the turbine blade carriers. This hub consists of a top and bottom piece that hold the blade carriers in place. The top hub is cone-shaped to prevent disrupting the airflow.

### 2.1.2 Thrust Bearing Addition 

A thrust bearing was designed to allow the pitch actuation system to rotate(along the axis of the shaft) while being controlled from a fixed position.

### 2.1.3 Rotation Mechanics Addition 

A disc, linkages, and a handle were added to convert rotation from a hand crank to linear motion (along the axis of the shaft). These linkages connect from the disc to the thrust bearing.

### 2.1.4 Ball Bearings Addition 

Two beams with ball bearings support the shaft and contain the pitch actuation input system.

## 2.2 Design Amendments 

- The blade carriers are now a stepped cylinder design to hold them in the blade hub while still allowing for rotation.  
- The linkages from the blade carriers to the thrust bearing are now curved, providing a smoother and larger range of pitch angle.  
- The middle shaft is no longer fixed, allowing it to rotate with the blade hub, and is much larger in diameter and length for strength and simplicity.  
- 

# 3\. Detailed Explanation of Required Analyses 

## 3.1 Engineering Analyses Test 

We performed engineering analysis tests on the critical components using Ansys. We ran a total deformation, Von-Mises stress, maximum principal stress, and safety factor test on the blades in a few different wind scenarios: 90 Pa (approx.12.1 m/s) , 200 Pa (approx.18 m/s), 360.6 Pa (approx.24.6 m/s), from [Wind Power Facts](https://cleanpower.org/facts/wind-power/). These values were determined from the wind pressure formula:  
q = 0.5*ρV^2 
Where:  
q = pressure (Pa)  
ρ = 1.225 kg/m^3 (air density)  
V = wind speed (m/s)

Modern wind turbines begin generating electricity at wind speeds of 3 to 4m/s, known as the cut-in speed, and are designed to shut down near 25 m/s to prevent structural damage. In this study, pressure cases were selected on the basis of [realistic operating range of wind turbines.


## 3.2 Engineering Analyses Results 

The blade was modeled using a fiberglass composite (GFRP) with an isotropic approximation to simplify analysis, using representative material properties from literature. Three loading cases (90 Pa, 200 Pa, and 360.6 Pa) were evaluated to simulate low to high wind conditions and assess structural performance. Results showed that maximum deformation occurs at the blade tip, with values around 1.19 mm, which is acceptable given the flexibility of composite materials. Peak stresses were concentrated in the root of the blade, but remained well below the material’s tensile strength. Under the highest loading condition, the maximum stress (8.48 MPa) was within safe limits when measured against the 59 MPa tensile strength of GFRP. 

### 3.2.1 Analysis Results 

#### 3.2.1.1 Blade 

Wind turbine blades are typically made from glass-fiber reinforced polymer (GFRP) due to its high strength-to-weight ratio. Thus, a fiberglass composite was assumed for this analysis. An isotropic approximation was used to simplify the model, with Young's Modulus derived from the Longitudal Modulus and Poisson's ratio, and the material properties were selected based on literature values for GFRP (1962 kg/m^3, Young’s Modulus 33.61 GPa, Poisson’s ratio 0.27, and tensile yield/ultimate strength 59 MPa) from [Static and Fatigue Performance of GFRP](https://www.sciencedirect.com/science/article/pii/S0141029625015081#fig7). For the stress analysis on the blade, three different loading cases were used in order to study the structural response under varying wind conditions. The root end of the blade is modeled with a fixed support to simulate cantilever behavior. The maximum stress is expected at the root due to the smaller cross section and changes in geometry, as confirmed by ANSYS simulation results.

The S-N curve used in the fatigue analysis was adapted from [published experimental fatigue-life data for GFRP composite panels](https://www.sciencedirect.com/science/article/pii/S0141029625015081#fig7) by Olena Karpenko (2025). Since the available data do not correspond exactly to the present blade geometry, the curve was used as a conservative literature-based approximation rather than a blade-specific material characterization.

It’s important to notice that for the thickness of the model, a value of 0.5mm was used. According to an [investigation](https://www.researchgate.net/publication/271635635_Research_on_Structural_Lay-up_Optimum_Design_of_Composite_Wind_Turbine_Blade) by Zhang Lanting (2012), a 30 m composite wind turbine blade was designed with a laminate thickness varying 80 mm at the root to 20 mm at the tip. Scaling thse dimensions to the present approx. 250 mm blade gives approximately equivalent thicknesses on the order of 0.65 mm at the root and 0.20 mm at the tip. Therefore, a uniform thickness of 0.6 mm was selected for the simplified representative value.

For the boundary condition, a fixed support was applied at the blade root around the hole region to represent the connection to the hub. 


##### 3.2.1.1.1 CASE 1: 90 Pa (low wind scenario) 

Figure 5: Total Deformation \- Case 1  
<img width="1342" height="571" alt="90_deformation" src="https://github.com/user-attachments/assets/0d181fec-e2b4-47f6-81be-4e53b111f678" />



Figure 6: Equivalent Stress (Von Mises) \- Case 1  
<img width="1346" height="566" alt="90_von mises" src="https://github.com/user-attachments/assets/7bff0828-7d61-4cb0-828c-c6bf63b7b42f" />



Figure 7: Maximum Principal Stress \- Case 1  
<img width="1345" height="562" alt="90_maxprincipal" src="https://github.com/user-attachments/assets/cf2ba9bf-653c-45d3-88b8-5857304d4860" />



Figure 8: Safety Factor \- Case 1  
<img width="1347" height="561" alt="90_safety" src="https://github.com/user-attachments/assets/dbd65ba0-51b4-4518-a7e2-3151f323723a" />

Figure 9: Life-Fatigue \- Case 1 
<img width="1347" height="565" alt="90_life" src="https://github.com/user-attachments/assets/83c8867b-7639-47b3-866d-6887b3a7e79b" />


##### 3.2.1.1.2 CASE 2: 200 Pa (medium-high wind) 

Figure 10: Total Deformation \- Case 2  
<img width="1398" height="560" alt="200_deformation" src="https://github.com/user-attachments/assets/159a1165-d3ee-4cca-89d2-c0a859bf7a53" />



Figure 11: Equivalent Stress (Von Mises) \- Case 2  
<img width="1397" height="561" alt="200_von mises" src="https://github.com/user-attachments/assets/5a0c77b4-684a-41d6-822c-fa2ea87faad9" />



Figure 12: Maximum Principal Stress \- Case 2  
<img width="1396" height="553" alt="200_maxPrincipal" src="https://github.com/user-attachments/assets/26335ff1-14a2-453d-966c-917530e5d200" />



Figure 13: Safety Factor \- Case 2  
<img width="1402" height="570" alt="200_safety" src="https://github.com/user-attachments/assets/863def34-d592-4d0f-a7fe-5959e6509af3" />

Figure 14: Life - Fatigue \- Case 2  
<img width="1401" height="567" alt="200_life" src="https://github.com/user-attachments/assets/f5a9af72-7c0c-41d9-95b3-eb4b91e309aa" />


##### 3.2.1.1.3 CASE 3: 360.6 Pa (high wind conditions) 

Figure 15: Total Deformation \- Case 3
<img width="1323" height="556" alt="360_deformation" src="https://github.com/user-attachments/assets/6a094b25-4245-41ea-875c-57602234b133" />



Figure 16: Equivalent Stress (Von Mises) \- Case 3  
<img width="1323" height="558" alt="360_von mises" src="https://github.com/user-attachments/assets/471979c6-f102-468b-9f9c-728a0ee4d833" />



Figure 17: Maximum Principal Stress \- Case 3  
<img width="1325" height="567" alt="360_maxprincipale" src="https://github.com/user-attachments/assets/7762ad73-2410-4148-adfc-045f98764ade" />



Figure 18: Safety Factor \- Case 3  
<img width="1321" height="561" alt="360_safety" src="https://github.com/user-attachments/assets/fe02167d-a61c-436a-8940-9a4db8efa4b1" />

Figure 19: Life - Fatigue \- Case 3 
<img width="1326" height="563" alt="360_life" src="https://github.com/user-attachments/assets/71b57f65-e71d-4e46-a3c9-9253ac73c9f1" />



### 3.2.2 Analysis Notes 

The tip of the blade experiences the most deformation. In the 3 cases, the maximum deformation is around 1.19 mm, which is acceptable for fiberglass as it is a composite material that allows for flexing without breaking due to bending. The maximum stress occurs at the root of the blade where the geometry changes. Since the material is a composite, the strength is determined by its layer thickness and internal density. According to a study included in the [Static and Fatigue Performance of GFRP](https://www.sciencedirect.com/science/article/pii/S0141029625015081#fig7), the tensile strength of GFRP for small samples was 59MPa, higher than the maximum of 8.48MPa we encountered in the high wind scenario. From the difference in tensile strength with 59MPa as a baseline for failure, the safety factor was well above standards. In the maximum wind scenario of 360.6Pa, the minimum safety factor was 6.96. 

# 4\. Discussion of Design for Assembly & 3D Printing 

## 4.1 Engineering Drawings 

### 4.1.1 Linear Translation Mechanism 

The linear translation mechanism is designed to convert rotational input from a manually operated crank into controlled axial motion of the hub along the shaft. This motion enables synchronized adjustment of blade pitch through a system of linkages connected to each blade. The engineering drawings detail the geometry, assembly, and functionality of these components to ensure accurate motion transfer.

#### 4.1.1.1 Linear Handle (Crank) 

Figure 17: Linear Handle  
 <img width="800" height="600" alt="Screenshot 2026-03-24 155144" src="https://github.com/user-attachments/assets/a4678690-67e8-48a0-8b4b-a554bc941ecd" />

The CAD drawing illustrates the pitch control handle, designed to allow manual operator adjustment of the turbine blade angles. This mechanism is engineered to accommodate an integrated motor, enabling automated blade pitch adjustment based on real-time RPM and wind speed data.

#### 4.1.1.2 Linear Linkage 

Figure 18: Linear Linkage  
 <img width="800" height="600" alt="Screenshot 2026-03-24 155202" src="https://github.com/user-attachments/assets/524da947-1117-430c-a4d1-b4615efdbd96" />

The model contains two linkages for the linear actuation input system. These connect from the input disc to the inner thrust bearing to provide axial motion along the shaft. The slight curve allows the linkage to rotate farther back on the input disc.

#### 4.1.1.3 Linear Shaft 

Figure 19: Linear Shaft  
 <img width="800" height="600" alt="Screenshot 2026-03-24 155213" src="https://github.com/user-attachments/assets/ea05de40-fbab-49e3-a00b-b3f5dd14f8db" />

The shaft for the linear actuation system input is housed in the first support beam, connected to the linear disc and the handle to ensure synchronized rotation for all components..

#### 4.1.1.4 Linear Disc 

Figure 20: Linear Disc  
<img width="800" height="600" alt="Screenshot 2026-03-24 155134" src="https://github.com/user-attachments/assets/02e20880-9dc1-4086-af9b-09bdd637761a" />

This disc connects the linear shaft to the linkages, transforming rotational motion into translational motion.

#### 4.1.1.5 Radial Ball Bearing 

Figure 21: Radial Ball Bearing  
 <img width="800" height="600" alt="Screenshot 2026-03-24 155222" src="https://github.com/user-attachments/assets/24298bbe-1aa8-4af8-b753-251fae270f2e" />

This radial ball bearing was outsourced, but may require a custom design if not locally available. The middle diameter should be 35mm; the outer diameter can vary.

### 4.1.2 Structural Support 

The structural supports and mounting system are designed to provide a stable framework for the blade pitch adjustment mechanism while maintaining proper alignment of the shaft and hub during operation. These components are responsible for transferring loads to the base structure and minimizing deflection that could affect performance. The engineering drawings define the geometry, constraints, and attachment methods required to ensure rigidity, strength, and overall stability.

#### 4.1.2.1 35mm Shaft 

Figure 22: 35mm Shaft  
  <img width="800" height="600" alt="Screenshot 2026-03-24 155229" src="https://github.com/user-attachments/assets/0fad2c6b-649f-4ce6-841a-6eb6ef0b43ad" />

The shaft design specifies high-strength forged steel to meet operational load requirements. For prototyping purposes, a 1 ⅜ ‘’ poplar dowel (34.925mm) was utilized to approximate the nominal 35mm diameter, providing sufficient tolerance for initial assembly validation.

#### 4.1.2.2 Support Beam (With Bearing) 

Figure 23: Support Beam (With Bearing)  
<img width="800" height="600" alt="Screenshot 2026-03-24 155237" src="https://github.com/user-attachments/assets/15d0f428-cfb6-443e-acd7-d30e06857052" />

The first support beam provides structural support for the shaft, integrating the pitch actuation system input. It features integrated hard stops for linear handle limitation. Ball bearings are utilized to minimize friction at the interface.

4.1.2.3 Support Beam  
Figure 24: Support Beam  
<img width="800" height="600" alt="Screenshot 2026-03-24 155245" src="https://github.com/user-attachments/assets/e9bb878d-f961-4d58-a5f8-80db00a52841" />

The support beam in the back is designed to handle primary tensile loads, balancing the turbine's weight to ensure structural stability. A ball bearing is integrated to minimize rotational friction and maintain efficiency at the tension point.

#### 4.1.2.4 Blade Carrier 

Figure 25: Blade Carrier  
<img width="800" height="600" alt="Screenshot 2026-03-24 155051" src="https://github.com/user-attachments/assets/e19a1536-b957-4eb4-b8d8-c9490465d405" />

The blade carrier is constrained within the hub utilizing specialized geometry, with the turbine blade secured to the carrier via a pin connection. The design integrates a dedicated linkage mounting point to facilitate active pitch adjustment.

### 4.1.3 Hub Mechanism  

The hub mechanism is designed to translate axial motion from the actuation system into coordinated rotational motion of the blades for pitch adjustment. It serves as the central load-bearing component, transferring forces between the shaft, linkages, and blade roots while maintaining alignment and smooth operation. The engineering drawings detail the geometry, internal features, and connection interfaces necessary to ensure reliable motion transfer and structural integrity.

#### 4.1.3.1 Blade Linkage 

Figure 26: Blade Linkage  
 <img width="800" height="600" alt="Screenshot 2026-03-24 155102" src="https://github.com/user-attachments/assets/39774bef-6e89-4480-9837-c1ffac5db7c5" />

The blade linkage utilizes a pinned connection to couple the blade carriers to the forward face of the thrust bearing. Featuring a curved geometry, the linkage maintains structural clearance around the carrier while enabling consistent torque transmission throughout the operational pitch angle range.

#### 4.1.3.2 Hub Bottom 

Figure 27: Hub Bottom  
<img width="800" height="600" alt="Screenshot 2026-03-24 155114" src="https://github.com/user-attachments/assets/44643561-eee2-4802-bcf6-4beb4c410aa7" />

The center hub assembly comprises a two-piece, top-and-bottom design, with the lower component featuring a hexagonal recess for positive shaft retention via a bolt. The design incorporates three pinned interfaces for alignment with the top component and specialized, geometry-driven slots to secure the blade carriers.

#### 4.1.3.3 Hub Top 

Figure 28: Hub Top  
<img width="800" height="600" alt="Screenshot 2026-03-24 155124" src="https://github.com/user-attachments/assets/e845576a-01ab-4658-bfe0-a1b4bcd3d7d9" />

The top hub piece features a shallow conical face on one side and incorporates three matching holes, along with specialized geometric slots for assembly alignment. This part mirrors the bottom piece's geometry for securely clamping the blade carriers.

#### 4.1.3.4 Thrust Bearing 

##### 4.1.3.4.1 Thrust Bearing Outer Top Above 

Figure 29: Thrust Bearing Outer Top Above  
<img width="800" height="600" alt="Screenshot 2026-03-24 155456" src="https://github.com/user-attachments/assets/205c8700-a936-4f70-8042-d8c9c51f750e" />

The rear thrust bearing component features a planar rear surface and an opposing face with a groove for ball bearing retention. It incorporates a central stepped-radius design with increased thickness for structural rigidity, along with six holes to facilitate assembly with the front piece and secure the middle component.

##### 4.1.3.4.2 Thrust Bearing Outer Top Below 

Figure 30: Thrust Bearing Outer Top Below  
<img width="800" height="600" alt="Screenshot 2026-03-24 155502" src="https://github.com/user-attachments/assets/429d350d-a473-4882-a64e-186ee4b12e42" />

The top piece design is functionally similar to the rear bearing, featuring a circular groove for the bearing balls on one face and a stepped radius for structural integrity. The flat opposing face features three mounting spots designed to attach the blade linkages via a pin.

##### 4.1.3.4.3 Thrust Bearing Inner Hollow 

Figure 31: Thrust Bearing Inner Hollow  
<img width="800" height="600" alt="Screenshot 2026-03-24 155446" src="https://github.com/user-attachments/assets/3bfda555-017f-48ad-9247-d904a4bafa72" />

The central thrust bearing piece features dual-sided grooves designed for ball bearing containment. The outer diameter includes a mounting bracket, allowing the linear linkages to attach.

#### 4.1.3.5 Wind Turbine Blade 

Figure 32: Wind Turbine Blade  
<img width="800" height="600" alt="Screenshot 2026-03-24 155508" src="https://github.com/user-attachments/assets/c877df70-e773-4cc9-96d7-754e5226ea6a" />

The CAD model was derived from a full-scale industrial turbine blade, incorporating optimized airfoil profiles and a tailored twist-taper distribution to maximize aerodynamic efficiency. The design was scaled to a 250mm length for 3D printing, maintaining proportional geometric features such as the chord length and leading-edge profile.

# 4.3 3D Assembly 

### 4.3.1 System Assembly 

Figure 4: Final Assembly  
<img width="700" height="800" alt="Turbine3" src="https://github.com/user-attachments/assets/a0c1bcc7-3a64-4131-b222-f4bec6f8d7d8" />

[View 3D Model](https://github.com/elillie1/Upwind-Engineering-MAE-342-Project/blob/1f9b453a7d7cd4b98a47d015ca5a2ef3f42e7306/Turbine%20STL.STL)

### 4.3.2 Exploded View 

Figure 21: Exploded View of Final Assembly  
<img width="878" height="741" alt="Screenshot 2026-03-24 160523" src="https://github.com/user-attachments/assets/c9e08142-6f98-46c9-aa7b-9e4acfad2ed8" />


https://github.com/user-attachments/assets/be5e3758-bcd8-45b3-98b0-f90c94066fdc 



## 4.4 Basic Motion Study (Operation) 



https://github.com/user-attachments/assets/12fe3cff-83d5-4e09-9deb-0a8b23c74059





# 5\. Anticipated Risks and Weaknesses 

## 5.1 Anticipated Failure Modes 

The pitch mechanism operates in a high-cycle, outdoor, and vibration-filled environment, which will cause it to be subjected to aerodynamic load reversals, centrifugal effects, and gust-driven transients. Failure modes due to these conditions are dominated by fatigue, wear, misalignment, and loss of control.

### 5.1.1 Actuator Failure 

1. Linear actuator stall or insufficient force  
- Underestimated aerodynamic pitch torque, cold temperature effects, high friction, and binding in the linkages.   
- Possible effects: the blade cannot reach the suggested pitch.  
2. Actuator mechanical failure due to wear  
- Possible mechanical failures include: high duty cycle, Contamination, poor lubrication, and side loads.   
- Possible effects: degraded control and eventual seizure can happen.  
3. Actuator electrical failure  
- Possible electrical failures include: Motor/driving overheating, water ingress, cable fatigue, and erosion between connectors.   
- Possible effects: Loss of pitch motion.

### 5.1.2 Linkage Failure 

1. Linkage fatigue cracking  
- Possible linkage fatigue cracking includes: cyclic loading from pitch commands and aerodynamic oscillations; stress concentrations at holes and threads.  
- Possible effects: partial or total loss of pitch authority for one blade; imbalance and high vibration.  
2. Linkage pin wear and deformation  
- Possible pin wear and deformation stems from: fretting, poor lubrication, and contamination.  
- Likely effects: backlash leads to pitch angle error, control oscillations, and shock loads that accelerate fatigue.  
3. Buckling of members under compression  
- Buckling possibilities under compression causes: actuator pushing toward hub loads linkage in compression; slender rods can buckle under gust loads.  
- Likely effects: sudden loss of pitch command transmission.

## 5.3 Anticipated Risks and Weaknesses 

The blade pitch adjustment mechanism presents several critical regions where elevated stresses, wear, or instability may occur due to the nature of the loading and geometry. These areas are discussed below.

### 5.3.1 Linkage-to-Blade Root Connections 

The connections between the actuation linkages and the blade roots are one of the most critical regions in the design. These joints are responsible for transferring axial motion of the hub into rotational motion of the blades, resulting in combined loading conditions including shear, bending, and axial forces.

Due to the presence of pins or joints, stress concentrations are expected at these locations. Additionally, these components are likely subjected to cyclic loading during operation, making them particularly susceptible to fatigue failure. As a result, these joints are anticipated to experience the highest localized stresses and are a primary concern for structural integrity.

### 5.3.2 Blade Root-Hub Interface 

The interface between each blade and the central hub is another high-risk region. This area must withstand the combined effects of pitch actuation forces, as well as any external loading applied to the blades. The geometric transition between the blade and hub can introduce stress concentrations, increasing the likelihood of crack initiation.

Because this interface transfers all loads from the blade into the hub, it is expected to be a governing location for failure, particularly under repeated loading conditions where fatigue may dominate.

### 5.3.3 Linkage Buckling Under Compression 

During operation, the linkages may experience compressive forces when the hub pushes the blades to adjust pitch. If the linkages are slender, they may be susceptible to buckling before reaching their material yield strength.

This represents a potential instability failure mode that may not be immediately evident from stress analysis alone. As such, buckling should be considered when evaluating the safety and performance of these components.

# 6\. References
[Static and Fatigue Performance of GFRP](https://www.sciencedirect.com/science/article/pii/S0141029625015081#fig7)
[Wind Power Facts](https://cleanpower.org/facts/wind-power/)
