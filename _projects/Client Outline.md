---
layout: project
title: MAE2250 Open Design Project
description: Centrifugal density separator for SLF post harvest
image: /assets/images/SLF.jpg
technologies: NA
---
## Milestones
- [Client Outline](#client-outline)
- [Functional Prototype](#functional-prototype)
- [Client Report](#client-report)

# Client Outline
**Client(s):** Cornell CALS Extension / E\&J Gallo Winery / National Grape  

## Problem statement 

 Viticulturalists in New York State are affected by the spotted lantern fly infestation, an invasive species that contaminates the harvest. Batches are rejected from juiceries and wineries, resulting in economic loss. Traditional pest-control methods are insufficient. Pesticides come with high economic and environmental costs. Egg removal proves too difficult because of the massive scale of laying locations, costing too much in labor.  

## Impact
Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting the growing consumer demand. 

## Proposed direction: Centrifugal Density Separator

**What it is:** A high-speed rotation device that separates harvested grapes from SLF by density, removing them from the desired product. 
  
**How it would be used:** Harvest is loaded into the device, and an internal drum spins at a calculated RPM. Heavier grapes are pushed out furthest, sliding down the angled outer walls into a collection bin. Lighter insects get pulled into a secondary bag. This way, grape pulp is conserved without contamination. 
 
**Why it’s better than the status quo:** Pesticides leave a taint on the wine’s taste profile and contaminate the organic integrity of the grapes. Manual sorting is slow, costly, and prone to human error/inconsistencies. Our solution is non-chemical and efficient on a large scale.

**End-of-semester proof-of-concept:**  A benchtop rotating drum prototype using grapes and 3D printed SLF accurate to weight and size, allowing us to optimize RPM. Success is determined by comparing the percentage of pests (SLF models) successfully sorted with the percentage of harvest lost.

## Key risks and unknowns

**Damage to grapes:** A high RPM exerts a force on the grape skin, possibly causing the grapes to break apart. Assessing the damage to grapes requires a physical "Burst Test," spinning grapes at incremental RPMs to identify when skins rupture, then comparing our results to the RPM needed to separate SLF.

**Mass variation and obstructions:** While a dry lanternfly is less dense than a grape, a lanternfly soaked in grape juice is much denser. Similarly, an SLF wedged inside a tight cluster might not separate easily, resulting in less effective separation. We can test this by using "weighted" objects (3D-printed bugs with adhesive, SLF tucked inside dense clusters or higher-density SLF), measuring SLF removed per cycle at various degrees of obstruction.

**Processing time:** A centrifuge is often a batch process, and if the device takes too long to load, spin, and unload, farmers will reject it in favor of faster methods. To address this, we will test the time the cycle duration of our prototype, and calculate the throughput to compare it to standard manual sorting speeds.


## Questions for the client
1. **How much material other than grapes, like stems and leaves, typically remains in the bin after your primary harvest?**  
   *Decision affected:* This changes our separation threshold and testing parameters based on what we want to separate/how much grapes weigh.

2. **What is the maximum holding time allowed between the grape being picked and it reaching the crusher before you worry about quality loss?**  
   *Decision affected:* This determines the constraints of our time trials and whether or not our product is viable in the time scale of grape processing.

3. **Do the SLF tend to stay on the surface of the grape clusters when disturbed, or do they retreat deep into the center of the bunch?**  
   *Decision affected:* This affects the “ramping profile” (i.e. how fast we accelerate) based on how hard SLF tends to stay on grapes, and also how we simulate SLF in our separation experiments


## References
- Penn State Agricultural Division. “Spotted Lanternfly.” Penn State Extension, extension.psu.edu/spotted-lanternfly.
- Penn State Agricultural Division, “Spotted Lanternfly Management in Vineyards.” Penn State Extension, extension.psu.edu/spotted-lanternfly-management-in-vineyards.
- Department of Environmental Conservation, NYS. “Spotted Lanternfly - NYDEC.” Dec.ny.gov, 16 Mar. 2017, dec.ny.gov/nature/animals-fish-plants/spotted-lanternfly.

---
# Client Report
Team Name: F4 Pest Control 
Team Members: Liz Tipton, Katelyn Fu, Arda Griffin, Sarah Bulkley, Junseok Kang 
Date: 5/5/26

## Context and Problem Statement
<img src="../../assets/images/rendered_view.png" alt="Rendered View of Final Prototype" width="500">

Invasive Spotted Lanternflies (SLF) pose a significant $8.8 million threat to the regional grape population (1). National food regulations mandate that SLF be removed before final production. Currently, entire batches of harvested grapes are often discarded if contamination is found. Our team focused on a post-harvest solution that leverages the physical density differences between the insects and the fruit to ensure crop viability and consumer safety. The primary constraint was to achieve a separation efficiency of at least 90% to meet industrial standards.

## Final Prototype and Application
We developed a water-based mechanical agitation system. The grapes contaminated with SLF are placed in the basin, and the mixture is agitated with the propeller (shown in purple), facilitating consistent and effective separation. SLF rises to the surface, and grapes sink due to their varying densities, achieving a 93% separation efficiency, exceeding our initial 90% goal.
This prototype is intended for use at the initial stage of grape processing, where harvested batches can be submerged and agitated to quickly remove invasive pests.

## Testing and Results 
**Test 1: Identifying Optimal RPM**
The primary objective of the product is to separate SLF from grapes. We wanted to test at what RPM separation is most effective. In previous testing, we identified that single-directional spinning was more effective than bi-directional agitation. In this test, we aim to refine our separation method.
*Results*
Observed that at low RPM (~3000 RPM), the majority of grape models sink, and SLF models get the most effectively separated at 3000 RPM. As the RPM increases above the 3000 ~ 4000 range,  grape models do not effectively sink and float with SLF models due to the excessively strong vortex created by the agitation. The highest separation efficiency of 93% is reached at approximately 3000 RPM.
<img src="../../assets/images/separationefficiency_rpm.png" alt="Graph comparing RPM with separation efficiency" width="500">

**Test 2: Leak Test**
<img src="../../assets/images/leak_prone.png" alt="Highlighting Leak-prone Areas" width="500">
The design must be able to hold water without significant leakage since the separation mechanism relies on water to separate the grapes from the SLF. 
We tested the four most leak-prone areas in our design: areas 1,2 and 3 (highlighted orange) are where the side walls interface, and the blue highlighted area is near the agitator. 
*Results*
<img src="../../assets/images/leak_test_data.png" alt="Leak Test Data" width="500">
No leak through the gap between the three side wall parts (Area 1, 2, 3), suggesting that using sealant and glue to connect the sides was sufficient. However, there was a noticeable leak through the center of the product (Area 4), where the shaft and bearing are. After the results, we added more sealant below the base, which reduced leakage. The results suggest that the interface between the agitator and the base requires a redesign. 

## Conclusion and Recommendation
Our prototype was evaluated against 3 primary success criteria defined in Milestone 05:
Separation Efficiency: Achieve >= 90% removal of SLF from grapes. Result: Passed (93.3%)
Containment/Leakage: Zero leaks from wall interfaces over 1 minute of submersion. Result: Passed (Areas 1-3); however, the shaft interface (Area 4) leaked 15 drops/min, failing our "zero-leak" goal for that specific component.
Structural Integrity: Maintain attachment between motor shaft and agitator through 20 cycles of 30-second operation. Result: Passed after applying epoxy adhesive to reinforce the initial press-fit.
Based on these outcomes, we recommend moving forward with a redesigned monolithic basin to address SC2 failures while maintaining the 3000 RPM agitation speed that secured our SC1 success.

For industrial scaling, the side walls should be manufactured as a singular unit to eliminate seam-related leak risks. Future iterations must utilize a motor capable of maintaining a constant 3,000 RPM under load. Materials should be transitioned to plastics or metals that will not corrode after long-term exposure to water and acidic grape juice. Other considerations include food safety. Although RTV sealant is food-safe, as is PETG, the lubricant we used around the shaft, as well as the glue used to hold the side walls together, is not suitable for use in food production. 

Since the design uses very few commercially available components, most manufacturing would have to be custom, increasing the per-unit cost. If scaled up, a mechanism would have to be put in place to extract the SLF once they rise to the top and extract the grapes when they sink. The current prototype was only designed with the testing efficiency of separation in mind. Another shortcoming of the design is the potential loss of harvest. Without draining, grape juice is lost when it is diluted with water, so systems would have to be put in place to preserve as much of the harvest as possible. So, despite high separation efficiency, a redesign is required if the design is to be used on an industrial scale. 

## Prototype and Testing Details
<img src="../../assets/images/exploded_view.png" alt="Exploded View of Prototype" width="500">
The device is assembled by seating a bearing and an o-ring into the baseplate to house the agitator shaft. Three side walls are then joined and secured to the base using RTV sealant for its vibration resistance and water-blocking properties. The 3D-printed basin is mounted to a stand, where a motor spinning up to 7000 RPM is integrated. Finally, the agitator is attached to the motor shaft using a standard ASME press-fit reinforced with epoxy. 

**Testing methodology for separation efficiency.** 
<img src="../../assets/images/slicer_settings.png" alt="Slicer View of SLF and Grape Models Showing Density Difference" width="500">
To model the SLF and grapes, we used 3D printed models that were accurate to the density shown in the image on the right. SLF models (cylinders) with density 1g/cm3 and grape models (spheres) with density 1.1g/cm3 (3,4).
We placed 10 SLF models and 10 grape models into the container and ran the motor at varying RPMs ranging from 500 to 7000. For each of the three trials per RPM, we ran the motor for 30 seconds and then counted the number of SLF that floated to the surface (NSLF float )and the number of grapes that sunk (Ngrapes sunk ). 
Then we calculated separation efficiency using the following formula:
<img src="../../assets/images/separation_efficiency_formula.png" width="500">
Each leak-prone area was submerged each for 1 minute using an arbitrary controlled amount of water, and the number of drops was counted.

**Test for Structural Integrity and Fastening**
In addition to a leak test and a test for separation efficiency, we also tested the structural integrity of the connection between the motor shaft and the agitator. One key safety concern is that the agitator head must not come loose from the motor shaft during testing. 
Methodology
To test the connection, we performed a cycling test of 20 cycles, each lasting 30 seconds, and then inspected the attachment between the motor shaft and the agitator for signs of loosening.
Results
After several tests, the shaft started spinning within the agitator without causing the agitator to spin. To combat this, we used a quick-setting epoxy adhesive, after which there were no more issues with adhesion between the agitator and the motor. 

---
# Functional Prototype
## Test 1: Comparing the effectiveness of agitation with single-direction spinning
**What is being tested:** 
The effectiveness of the propeller’s constant change of direction vs single-direction spinning in separating grapes and SLF models
**How it was tested:**
Place a known mixture (10 grape models and 10 SLF models) into the container of water.
Run the drill for 30 seconds using a single-direction spin.
Repeat the rest with a new mixture, but manually toggle the drill direction every 2 seconds to simulate an agitator.
Visually assess the separation of SLF and grapes, taking images. Count how many SLF models have successfully floated/separated from the grape cluster in each scenario
**What happened:**
Both directions of agitation showed similar amounts of separation; however, the oscillating mechanism led to a greater success rate among 10 trials. There are 10 of each, grape and SLF, represented by their densities and general surfaces in 3D printed form, in each of 10 trials, (see the table below) the oscillating mechanism performed marginally better and with less variance.
<img src="../../assets/images/first_separationtest.png" alt="Comparing Single Directional with Bi-directional Oscillation" width="500">
**Quantitative metrics:** 
Avg Separation % for Single Direction Spinning (#Flown/Sunk over total): 79.5% 
Avg Separation % for Bi-Directional (#Flown/Sunk over total): 84.5% 
Time to first separation: 3.78 sec ± 0.15 seconds (from each of the 20 trials)
**Design Changes Needed:** 
Since bi-directional agitation is significantly more effective, we need to design a mechanical linkage or use a programmable motor controller to automate the direction switching rather than relying on a manual drill trigger.

## Test 2: Propeller Cavitation & Turbulence Range
**What is being tested:** 
Determining whether the propeller creates enough "lift" to move the SLF models without hitting the bucket walls or the grapes themselves
**How it was tested:** 
Fill the bucket to a marked "fill line" and operate the propeller at 25%, 50%, and 75% power.
Observe the "vortex depth" (the distance from the water surface to the lowest point of the whirlpool).
Measure the distance (in mm) between the spinning propeller tip and the inner wall of the 3D-printed bucket to check for dynamic clearance.
**What happened:** 
The drill was run at 75,50,25 percent power by marking how far the trigger traveled and (assuming it was proportional to the drill's power/speed) running the experiment while the trigger is pulled to its respective mark. Using a custom 3d printed measuring tool (that was tiny enough not to disturb the vortex, 2 trials on each of the three speeds were conducted (see data below). Because of the nature of our oscillations being inconsistent and often breaking the vortex, only single-directional vortices were measured
**Quantitative metrics:** 
<img src="../../assets/images/vortex_depth.png" alt="Vortex Depth in cm at different % of power" width="500">
Clearance from walls: 4.86 inches
Spillage. Low, with only a few drops being spilled onto the paper tower
**Design Changes Needed:** 
We must increase the diameter and size of our propeller since the vortex is both low in depth and also has an incredibly small width. By scaling the vortex up almost around 2.2X its original size, we were able to conduct the nice separation test from above. In addition, we need to make the propellers' workholding a larger diameter, as in the courses on these tests, around 3 propellers broke and needed replacement.

## Test 3: Structural Integrity & Fastening (The "Drill-to-Propeller" Joint)
**What is being tested:** 
Assembly and fastening to ensure the connection between the drill bit and the 3D-printed propeller doesn't slip or strip under the resistance of the water.
**How it was tested:** 
Perform a cycling test of 20 cycles, each lasting 30 seconds.
Between each cycle, attempt to manually wiggle the propeller on the shaft to check for loosening.
Inspect the 3D-printed "socket" for signs of permanent deformation or cracking
**What happened:** 
After 20 cycles (30 seconds of spinning), the propeller developed slight rotational play and minor wear inside the 3D-printed socket, but no cracking occurred.
Visual Inspection: Shining a light perpendicular to the surface of the socket, you can visually inspect the gap from how much light goes through, and hits our shaft seal and reflects the TPU coating. Comparing the before and after, we could visually see more of the TPU shaft seal than before.
**Quantitative Metrics:** 
Cycles completed: 20 Cycles of 30 seconds, no breakage, but increased vibration/chatter in the final 5 cycles.
Connection Play in mm developed after 20 cycles. 2.7 mm (measured via bore caliper, comparing the original socket diameter to the new one)
**Design Changes Needed:** 
If the propeller begins to slip on the drill shaft, we will iterate the design to ensure a more secure mechanical lock between the motor and the agitator.

## Test 4: Leak test
**What is being tested:** 
How much water is lost through the basket.
**How it was tested:** 
Fill the basket with water to the highest level.
For 1 minute, count the number of droplets that leave the basin
Repeat the test 3 times
What happened: Water was filled to the fill line, paper towels were placed underneath the base for better accuracy, and a minute was timed on the stopwatch.
**Quantitative Metrics:** 
Number of drops lost in each cycle (list): 11,7,14
Average rate of water loss (ml/minute) = #drops*0.05ml/1min = 0.55 ml, 0.35 ml, 0.7 ml
Design Changes Needed: While the TPU shaft seal holds water incredibly well, better tolerancing on our 3D prints and machine shaft and perhaps an actual shaft seal from McMaster Carr will truly make this a watertight machine.

## Success Criteria
Context: Our device helps grapevine farmers mechanically separate invasive Spotted Lanternflies (SLF) from harvested grapes using water-based agitation and density-driven buoyancy.
Criterion 1 – Separation Efficiency (High Priority): Assesses whether the device reliably floats SLF models away from grape clusters. 
Measurement: Count SLF models remaining entangled with grapes before and after a 60-second agitation cycle. 
Target: ≥90% of SLF models successfully separated.
Criterion 2 – Processing Throughput (Medium Priority): Assesses whether the device is fast enough for practical farm use. 
Measurement: Stopwatch timing from when the user touches the lid to when the grapes are ready for the next stage. 
Target: ≤4 minutes per 1kg batch.
Criterion 3 – Operating Stability (Medium Priority): Assesses whether the device stays safe and controlled during operation. 
Measurement: Pre- and post-spin position markings on the table (target: ≤2cm of movement) and a graduated cylinder to capture spilled water (target: ≤50ml lost at maximum RPM).
Exhibit Day Demo: We will present a 3D-printed bucket pre-filled with water and a contaminated batch of grape and SLF models. After a 30-second agitation cycle, we will pour the cleaned grapes into a transparent bowl to visually show separation, then weigh the recovered SLF models on a small scale to demonstrate Criterion 1 is met in real time.

## Components List
<img src="../../assets/images/first_componentslist.png" alt="Components List" width="500">

## Design intent
The prototype is a water-based agitation system driven by a handheld drill. The core functional components are:
Agitator Bucket – A sealed 3D-printed PLA container that holds water, grape models, and SLF models. It acts as the stationary outer vessel during operation.
Shaft – A machined aluminum (Al 6061) rod that transfers rotational motion from the drill down into the bucket. A flange at the top constrains vertical movement, and the shaft rotates freely relative to the bucket. Connected to the agitator head via press fit.
Agitator Head – A 3D-printed PLA propeller/paddle assembly press-fit onto the bottom of the shaft. When spun by the drill, it agitates the water, creating turbulence that causes low-density SLF models to float while denser grape models sink.
Legs – 3D-printed PLA columns that provide enough clearance between the floor and the bottom of the bucket for the drill to fit in.
Additionally, grape and SLF models were made to test separation.
Grape Models – 3D-printed PLA parts sized, shaped, and weighted to replicate the density and surface geometry of real grapes. Spheres with a diameter of 20mm and a weight of 4.61g.
SLF Models – 3D-printed PLA parts sized, shaped, and weighted to simulate the density and surface geometry of real Spotted Lanternflies. Cylinders with diameter 10mm, height 5mm, and weight of 1.42g.

<img src="../../assets/images/first_functionsketch.png" alt="Sketch of System" width="500">

## Assembly instructions
Step 1 – Prepare the Shaft Insert the machined aluminum shaft through the center hole of the Agitator Bucket. The flange at the top of the shaft should seat flush against the rim of the bucket, constraining the shaft from dropping through.
Step 2 – Attach the Agitator Head Press-fit the Agitator Head onto the top of the shaft inside the bucket. Ensure the fit is firm with no rotational play. The agitator head should sit near the bottom of the bucket without contacting the bucket floor.
Step 3 – Verify Clearance Rotate the shaft by hand to confirm the agitator head spins freely without scraping the inner walls of the bucket. Minimum clearance should be maintained on all sides (reference Test 2 data: 4.86 inches measured).
Step 4 – Connect the Legs. Insert three legs into the three bottom holes near the circumference of the bucket. The fit should be tight.
Step 5 – Connect the Drill. Insert the end tip of the shaft into the drill chuck. Tighten securely. The drill should be able to drive the shaft in both clockwise and counterclockwise directions for oscillating agitation.
Step 6 – Load the Bucket. Fill the Agitator Bucket with water to the marked fill line. Add the grape models and SLF models to the water.
Step 7 – Operate. Power the drill, toggling direction every ~2 seconds to simulate oscillating agitation. Run for 30–60 seconds. SLF models should migrate to the water surface while grape models remain submerged.

