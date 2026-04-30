# Report

# Phase 3 Report

**Table of Contents**

[**1. Overview of Phase 3**](#1.-overview-of-phase-3)

[1.1 Phase 3 Objectives	3](#1.1-phase-3-objectives)

[1.2 Scope of Phase 3	3](#1.2-scope-of-phase-3)

[**2. Prototype Fabrication	3**](#2.-prototype-fabrication)

[2.1 Fabrication Overview	3](#2.1-fabrication-overview)

[2.2 Additive Manufacturing Details	3](#2.2-additive-manufacturing-details)

[2.2.1 Printer Details	4](#2.2.1-printer-details)

[2.2.1.1 Printer Model	4](#2.2.1.1-printer-model)

[2.2.1.2 Filament Type	4](#2.2.1.2-filament-type)

[2.2.1.3 Nozzle Size	4](#2.2.1.3-nozzle-size)

[2.2.1.4 Layer Height	4](#2.2.1.4-layer-height)

[2.2.1.5 Infill Percentage	4](#2.2.1.5-infill-percentage)

[2.2.1.6 Print Speed	4](#2.2.1.6-print-speed)

[2.2.1.7 Printer Support Settings	4](#2.2.1.7-printer-support-settings)

[2.2.1.8 Print Orientation Notes	4](#2.2.1.8-print-orientation-notes)

[2.2.2 Printed Components	5](#2.2.2-printed-components)

[2.2.2.1 Hub Top and Bottom	5](#2.2.2.1-hub-top-and-bottom)

[2.2.2.2 Blade Carriers	5](#2.2.2.2-blade-carriers)

[2.2.2.3 Blade Linkages	6](#2.2.2.3-blade-linkages)

[2.2.2.5 Linear Disc	7](#2.2.2.5-linear-disc)

[2.2.2.9 Thrust Bearing Components	8](#2.2.2.9-thrust-bearing-components)

[2.2.2.10 Wind Turbine Blades	11](#2.2.2.10-wind-turbine-blades)

[2.2..11 Final Prototype Assembly	12](#2.2..11-final-prototype-assembly)

[2.3 Print Iterations and Reprints	13](#2.3-print-iterations-and-reprints)

[2.4 Other Manufacturing Materials Used	13](#2.4-other-manufacturing-materials-used)

[**3. Assembly Procedure and Challenges	13**](#3.-assembly-procedure-and-challenges)

[3.1 Assembly Procedure	13](#3.1-assembly-procedure)

[3.1.1 Thrust Bearing Assembly	13](#3.1.1-thrust-bearing-assembly)

[3.1.2 Hub Assembly	14](#3.1.2-hub-assembly)

[3.1.3 Final Integration	14](#3.1.3-final-integration)

[3.1.4 Summarized List for Full Assembly	14](#3.1.4-summarized-list-for-full-assembly)

[3.2 Assembly Challenges	15](#3.2-assembly-challenges)

[**4. Prototype Testing and Results	16**](#4.-prototype-testing-and-results)

[4.1 Test Objectives	16](#4.1-test-objectives)

[4.2 Test Procedure	16](#4.2-test-procedure)

[4.3 Test Results	16](#4.3-test-results)

[4.4 Interpretation of Results	16](#4.4-interpretation-of-results)

[**5. Comparison to Phase 2 Projections and Predictions	17**](#5.-comparison-to-phase-2-projections-and-predictions)

[**6. Failures, Mistakes, and Lessons Learned	17**](#6.-failures,-mistakes,-and-lessons-learned)

[6.1 Major Failures Observed	17](#6.1-major-failures-observed)

[6.2 Mistakes in Fabrication and Assembly	18](#6.2-mistakes-in-fabrication-and-assembly)

[6.3 Unexpected Outcomes	18](#6.3-unexpected-outcomes)

[6.4 Lessons Learned	18](#6.4-lessons-learned)

[**7. Recommended Design Changes For Final Product	18**](#7.-recommended-design-changes-for-final-product)

[**8. Final Poster	18**](#8.-final-poster)

[**9. Conclusion	20**](#9.-conclusion)

**List of Tables**

Table 1: Phase 2 Predictions and Phase 3 Outcomes

**List of Figures**  
Figure 1: Printer Part Assignment  
Figure 2: Physical Model for Hub Top  
Figure 3: Physical Model for Hub Bottom  
Figure 4: Physical Model for Blade Carriers (x3)  
Figure 5: Physical Model for the Blade Linkages (x3) (Side-View)  
Figure 6: Physical Model for the Blade Linkages (x3) (Top-View)  
Figure 7: Physical Model for the Linear Disc  
Figure 8: Physical Model for the 10-tooth Linear Gears  
Figure 9: Physical Model for the 16-tooth Linear Gears  
Figure 10: Physical Model for the Thrust Bearing Top Back (1)  
Figure 11: Physical Model for the Thrust Bearing Top Back (2)  
Figure 12: Physical Model for the Thrust Bearing Top Front  
Figure 13: Physical Model for the Thrust Bearing Bottom Front  
Figure 14: Physical Model for the Thrust Bearing Bottom Back (1)  
Figure 15: Physical Model for the Thrust Bearing Bottom Back (2)  
Figure 16: Physical Model for the Turbine Blades  
Figure 17: Physical Model for the Final Prototype Assembly  
Figure 18: Final Project Poster

# 1\. Overview of Phase 3 

## 1.1 Phase 3 Objectives 

Phase 3 focused on the fabrication, assembly, and physical validation of the wind turbine pitch adjustment system developed in Phases 1 and 2. The objective of this phase was to manufacture a 1:1 functional prototype, assemble the complete mechanical system, evaluate its ability to demonstrate active blade pitch adjustment, and compare observed physical behavior against the Phase 2 design predictions. This phase also emphasized identifying fabrication limitations, assembly challenges, mechanical discrepancies, and opportunities for future design refinement.

## 1.2 Scope of Phase 3 

This report documents the physical design and prototyping process of the wind turbine blade pitch adjustment mechanism, including the manufacturing decisions, assembly procedure, prototype testing, comparison to predicted behavior from Phase 2, post-test reflections, and what we would do differently if developing a second iteration. Particular emphasis is placed on evaluating whether the physical prototype successfully demonstrated the intended core mechanical function: synchronized blade pitch adjustment through axial-to-rotational motion transfer. This phase serves as the validation step of the design process established in Phase 2.

# 2\. Prototype Fabrication 

## 2.1 Fabrication Overview 

The Phase 3 prototype was fabricated as a physical model of the wind turbine blade pitch adjustment system developed in Phase 2. The design was manufactured primarily via additive manufacturing (3D printing) to quickly produce complex geometry, minimize fabrication costs, and validate the design's mechanical function under safe operating loads. Printed components included the hub assembly, blade carriers, blade linkages, support beams, linear actuation components, and wind turbine blades. The components not 3D-printed were the main shaft and dowel supports, and this design choice will be described further in section 2.4, Other Manufacturing Materials Used. The prototype was intended to validate the functionality of the blade-hub interface subsystem, pitch actuation subsystem, and structural support subsystem originally defined in Phase 2. There was an emphasis on the interaction among the subsystems, as the system's importance lay in its function in unison rather than in the independent subsystems' operations.

## 2.2 Additive Manufacturing Details 

All custom components were exported from SolidWorks as individual STL files in accordance with MEE 342 fabrication requirements. In order to print our parts in batches and on our time, we opted to use Wyatt Perez’s personal 3D printer, the Creality K2 Combo. Following the prints, each part was monitored for dimensional accuracy and modular replacement if needed.

### 2.2.1 Printer Details 

#### 2.2.1.1 Printer Model 

* Creality K2 Combo

#### 2.2.1.2 Filament Type 

* Creality Ender PLA

#### 2.2.1.3 Nozzle Size 

* 0.4 mm

#### 2.2.1.4 Layer Height 

* 0.2 mm

#### 2.2.1.5 Infill Percentage 

* 15%

#### 2.2.1.6 Print Speed 

* 250 mm/s

#### 2.2.1.7 Printer Support Settings 

* Tree Supports with top Z distance 0.2mm

#### 2.2.1.8 Print Orientation Notes 

* Prints were oriented to reduce the need for supports and increase strength.

**Figure 1: Printer Part Assignment**  
<img width="533" height="573" alt="Screenshot 2026-04-30 112224" src="https://github.com/user-attachments/assets/6d9a79fa-cfa2-4ee3-806f-c88b3ce54a97" />

2.2.2 Printed Components 

#### 2.2.2.1 Hub Top and Bottom 
**Figure 2: Physical Model for Hub Top**  
<img width="2157" height="1618" alt="Wing_Pitch_Cone_2" src="https://github.com/user-attachments/assets/3fbcea2e-76aa-4687-98b9-7efe4eb05bcf" />

**Figure 3: Physical Model for Hub Bottom**  
<img width="3093" height="2320" alt="Wing_Pitch_Cone" src="https://github.com/user-attachments/assets/adb3bf0f-833d-48a8-a714-2fbb76cc5b64" />

2.2.2.2 Blade Carriers 

**Figure 4: Physical Model for Blade Carriers (x3)**  

2.2.2.3 Blade Linkages 

**Figure 5: Physical Model for the Blade Linkages (x3) (Side-View)**  

**Figure 6: Physical Model for the Blade Linkages (x3) (Top-View)**  

2.2.2.5 Linear Disc 

**Figure 7: Physical Model for the Linear Disc**  

2.2.2.8 Linear Gears

**Figure 8: Physical Model for the 10-tooth Linear Gears**  

**Figure 9: Physical Model for the 16-tooth Linear Gears**  

2.2.2.9 Thrust Bearing Components 

**Figure 10: Physical Model for the Thrust Bearing Top Back (1)**  

**Figure 11: Physical Model for the Thrust Bearing Top Back (2)**  

**Figure 12: Physical Model for the Thrust Bearing Top Front**  

**Figure 13: Physical Model for the Thrust Bearing Bottom Front**  

**Figure 14: Physical Model for the Thrust Bearing Bottom Back (1)**  

**Figure 15: Physical Model for the Thrust Bearing Bottom Back (2)**  

2.2.2.10 Wind Turbine Blades 

**Figure 16: Physical Model for the Turbine Blades**  

2.2..11 Final Prototype Assembly 

**Figure 17: Physical Model for the Final Prototype Assembly**<img width="3093" height="2320" alt="Wing_Pitch_Cone" src="https://github.com/user-attachments/assets/7f0db1db-fb70-4cfb-b722-51b440b07bdf" />
<img width="2157" height="1618" alt="Wing_Pitch_Cone_2" src="https://github.com/user-attachments/assets/7d732272-1c71-4bca-8702-8e076fdf7c03" />


**GLB file**

Print orientations were selected to reduce support use in curved and bearing-contact areas while preserving dimensional accuracy in mating and rotational interfaces. Care was taken in orienting the blade linkages, thrust bearing components, and blade carriers due to their sensitivity to tolerance, fitment, and alignment.

## 2.3 Print Iterations and Reprints 

Due to how complex the assembly is and the small tolerances needed for rotational and sliding surfaces and interfaces, multiple printed parts required small adjustments and re-printing. Reprints were primarily caused by:

* Dimensional interference in mating surfaces.
* High friction in rotating surfaces and interfaces.
* Insufficient clearance in linkage holes.
* Weakness in printed sections that were thin or had minimal mass.
* Tolerance mismatch between printed and purchased components.

There was a maximum of 3 reprints for a few parts due to tolerance mismatch issues and breaking due to stress concentrations on sharp corners. Each reprint we added mass to the material and shrunk the footprint to alleviate both the stress concentration and tolerance mismatches that existed.

The most iteration-sensitive components were expected to be the blade carriers, thrust bearing interfaces, and blade linkages due to their critical role in transmitting pitch motion and maintaining alignment. This seemed to be consistent with the anticipated high-risk regions identified in Phase 2.

## 2.4 Other Manufacturing Materials Used 

The shaft and support structure were made from wood. This was chosen for the inherent strength of the material, price point, and time savings. We also used fasteners (3mm and 5mm bolts and a large Hex bolt) to put the parts together and steel BBs for the thrust bearing.

# 3\. Assembly Procedure and Challenges 

## 3.1 Assembly Procedure 

### 3.1.1 Thrust Bearing Assembly 

The thrust bearing assembly was the first one to be put together, as it serves as the main interface responsible for axial actuation input while allowing rotational motion of the hub. We began by placing the upper thrust bearing housing in an upside-down orientation, effectively showing the bearing race geometry. Ball bearings were then put evenly along the race channel to set the first rolling contact interface. The lower thrust bearing housing was then prepared the same way by placing another set of ball bearings along its race channel.

Once we had both outer bearing races filled, the central thrust bearing was placed into the lower housing to secure the set of ball bearings and establish the internal translating interface. This partly assembled unit was then aligned with the upper housing and put together to form the complete thrust bearing assembly. Next, the assembly was secured using six M3 screws, installed in two stages to maintain alignment and ensure even clamp force of the bearing components. Care needed to be taken during tightening to avoid excessive loading, as overconstraint of the bearing races especially increased resistance and dragging.

### 3.1.2 Hub Assembly 

The hub assembly was next to be built to form the blade support and pitch transfer structure. We started assembly by securing the central hex bolt into the lower hub piece, allowing the primary shaft connection and rotational anchor for the hub assembly. The three blade carriers were then put into the dedicated hub cutouts, where each carrier was set to allow constrained rotation while allowing axial retention within the hub body.

After that, the upper hub component was placed over the lower hub to grab the carriers and complete the hub enclosure. The two halves of the hub were then secured using three M5 screws to provide rigidity while maintaining blade carrier mobility. After the hub body was assembled, the linkages were attached to the blade carriers using M3 screws. Each linkage was oriented in a way that the curved geometry provided clearance for the expected range of pitch motion and lowered interference with neighboring components during actuation and translation.

### 3.1.3 Final Integration 

Final assembly consisted of integrating the thrust bearing and hub subsystems into the full pitch adjustment mechanism. The blade linkages stretching from the hub assembly were the first pieces attached to the outer portion of the thrust bearing using M3 screws once again, allowing the mechanical connection between axial thrust bearing motion and rotational blade pitch actuation.

Once the linkages were connected all the way, the thrust bearing and hub assembly was mounted onto the wooden shaft and secured using the central hex bolt. This established the main rotational axis of the system and allowed the pitch mechanism to translate and rotate as we intended. Then lastly, the wind turbine blades were installed onto the blade carriers to complete the assembly and enable full-system pitch actuation.

### 3.1.4 Summarized List for Full Assembly 

Assemble the thrust bearing

1. Place the top thrust housing upside down on the table
2. Place BBs along the channel
3. Get the bottom thrust housing and place BBs along its channel
4. Get the center thrust component and place it on the bottom thrust housing to secure the BBs in place
5. Get that whole unit and place it on top of the top thrust housing and secure it with 3 M3 bolts
6. Flip over and add the last 3 M3 bolts

Assemble the Hub

1. Get the large Hex bolt and secure it to the bottom hub
2. Add the blade carriers to the bottom hub, one per cutout
3. Add the top hub over everything and secure with 3 M5 bolts
4. Get the 3-blade linkages and secure the more curved part to the blade linkages with 1 M3 bolt, do this for each one

Full assembly

1. Get the thrust bearing assembly and hub assembly
2. Secure the blade linkages to the top of the thrust bearing with M3 bolts
3. Secure the full assembly to the wooden shaft with the large hex bolt
4. Add the blades to the blade carrier

## 3.2 Assembly Challenges 

There were a few challenges during assembly that we encountered, namely the dimensional tolerance variation, assembly complexity, and the time-intensive nature of repeated manual fitting. Due to the number of printed components interacting and the tight tolerances required for rotational and pinned interfaces, some dimensional inaccuracies in several printed parts led to fitment issues. These discrepancies required a lot of adjustment, manual rework, and occasional disassembly to fix the alignment or decrease the interference experienced by the assembly.

The most significant tolerance-related issues emerged from the thrust bearing races, pinned linkage interfaces, and mating surfaces between the hub and blade carriers. In multiple cases, printed dimensions produced either too much friction or not enough clearance, requiring additional sanding and trimming to achieve good motion. These issues were made worse by incremental tolerance building across multiple interfacing components, which obviously increased resistance and reduced efficiency during assembly and testing.

Another challenge was the labor-intensive nature of the assembly process. Because the prototype relied on a bunch of small fasteners, pinned joints, and repeated aligning of subassemblies, assembly and disassembly became time-consuming and tedious. This was very evident during troubleshooting, where multiple disassembly cycles were required to isolate sources of binding, adjust component fitment, and validate design mods. While these issues did not prevent success, they definitely increased build time and showed the need for improved manufacturability and simplification in future iterations.

# 4\. Prototype Testing and Results 

## 4.1 Test Objectives 

The main objective of prototype testing was to evaluate the functionality and performance of the pitch actuation mechanism and validate the kinematic behavior predicted in Phase 2. Testing focused on verifying smooth rotational motion of the thrust bearing and assembly, transmission of axial input through the linkage system, and coordinated blade pitch adjustment across the three blades. We also utilized this testing period to identify things like mechanical resistance, misalignment, and friction that could degrade motion quality or reduce actuation efficiency.

## 4.2 Test Procedure 

The fully assembled prototype was tested through manual actuation of the pitch control mechanism to evaluate the interaction between the thrust bearing, linear linkages, and blade pitch system. The thrust bearing was manually rotated and translated along the shaft axis to simulate the intended actuation path so we could assess its rotational smoothness under load. Simultaneously, axial push-pull input was applied through the actuation linkage system to induce blade rotation and evaluate the consistency of pitch response, linkage motion transfer, and overall kinematic functionality.

## 4.3 Test Results 

Initial testing showed that the thrust bearing assembly showed high rotational resistance, limiting smooth actuation and increasing input effort. When looking at the system, we noticed that it indicated the stiffness was primarily caused by high internal preload and friction within the printed thrust bearing. After some minor modifications, specifically the removal of one bearing ball to reduce internal constraint and contact pressure, we saw that rotational smoothness improved significantly, and the bearing was able to rotate with much lower resistance.

The blade pitch linkages successfully transmitted axial motion into rotational blade actuation, verifying the intended kinematic behavior of the mechanism. All three blades responded to actuation input and verified coordinated pitch adjustment. However, motion through the linkage system remained moderately stiff and showed localized resistance throughout parts of the actuation range. We believed this behavior results primarily from shaft misalignment, differing tolerances, and friction at the contact surfaces between the wooden shaft and printed components. While the mechanism remained functional, these effects did in fact reduce motion smoothness and caused minor inconsistencies in blade response.

## 4.4 Interpretation of Results 

Prototype testing confirmed that the pitch adjustment mechanism is capable of performing its mechanical task, which was converting axial actuation into blade pitch rotation. The operation of both the thrust bearing and blade linkage systems was successful and validates the core design idea developed in Phase 2, and demonstrates that the kinematic architecture is viable.

Although the prototype needed small modifications to achieve the performance we ultimately wanted, the observed issues were mostly due to fabrication tolerances, alignment sensitivity, and friction rather than basic design failure. These results prove that the concept is mechanically sound, but performance is strongly dependent on improved dimensional control, precise alignment, and reduced friction.

# 5\. Comparison to Phase 2 Projections and Predictions 

**Table 1: Phase 2 Predictions and Phase 3 Outcomes**

|Metric|Phase 2 Prediction|Phase 3 Prediction|Discussion|
|-|-|-|-|
|Pitch actuation|Functional|Functional|The prediction was validated|
|Blade synchronization|Smooth|Moderate Lag|Tolerance/friction reduced smoothness|
|Pitch range|\~79 degrees|\~30 degrees|Reduced by physical interference and limited range of motion|
|Structural rigidity|Stable|Stable|The prediction was validated|
|Linkage buckling|Possible|Not observed|Could occur under greater load|
|Hub/blade interface stress|Critical region|Minor play observed|Matches predicted weakness|

Phase 2 predicted that the linkage interfaces, blade root-hub interface, and compressive linkage loading would be the most critical regions for mechanical error and failure. These predictions were validated during prototype testing, where most of the performance loss originated from those same interfaces.

# 6\. Failures, Mistakes, and Lessons Learned 

## 6.1 Major Failures Observed 

The most significant performance limitations were friction, tolerance mismatches, and alignment sensitivity, rather than catastrophic structural failure.

## 6.2 Mistakes in Fabrication and Assembly 

One primary design mistake was underestimating the sensitivity of multi-part tolerances in rotating and pinned assemblies. CAD-defined clearances were sufficient digitally, but less forgiving in printed parts.

## 6.3 Unexpected Outcomes 

The prototype was more functionally successful than expected in demonstrating pitch motion, but less smooth and more friction-sensitive than predicted.

## 6.4 Lessons Learned 

The largest takeaway from Phase 3 was that mechanical functionality was successfully demonstrated, but manufacturability and tolerance control dominated real-world performance.

# 7\. Recommended Design Changes For Final Product 

* Increase the linkage thickness to reduce compliance.
* Add bushings or bearings to pinned interfaces.
* Redesign thrust bearing with lower-friction contact surfaces.
* Increase tolerances in mating rotational interfaces.
* Reinforce blade-root interface.
* Improve shaft alignment and support rigidity.
* Replace the manual crank with guided linear actuation.

# 8\. Final Poster 

**Figure 18: Final Project Poster**

# 9\. Conclusion 

Phase 3 successfully demonstrated the core mechanical functionality of the wind turbine blade pitch adjustment system through a 1:1 physical prototype. The prototype validated the primary design concept developed in Phase 2 by converting axial motion into synchronized blade pitch rotation across all three blades. While friction, tolerance mismatch, and assembly sensitivity reduced motion quality, the system successfully achieved its intended mechanical function and provided valuable insight into real-world manufacturability and design refinement.

