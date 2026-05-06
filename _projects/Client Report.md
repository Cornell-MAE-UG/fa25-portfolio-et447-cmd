---
layout: project
title: Client Report: Buoyancy-Based Agitation System for SLF Removal
description: Centrifugal density separator for SLF post harvest
image: /assets/images/SLF.jpg
technologies: NA
---
Team Name: F4 Pest Control 
Team Members: Liz Tipton, Katelyn Fu, Arda Griffin, Sarah Bulkley, Junseok Kang 
Date: 5/5/26

## Context and Problem Statement
Invasive Spotted Lanternflies (SLF) pose a significant $8.8 million threat to the regional grape population (1). National food regulations mandate that SLF be removed before final production. Currently, entire batches of harvested grapes are often discarded if contamination is found. Our team focused on a post-harvest solution that leverages the physical density differences between the insects and the fruit to ensure crop viability and consumer safety. The primary constraint was to achieve a separation efficiency of at least 90% to meet industrial standards.

## Final Prototype and Application
We developed a water-based mechanical agitation system. The grapes contaminated with SLF are placed in the basin, and the mixture is agitated with the propeller (shown in purple), facilitating consistent and effective separation. SLF rises to the surface, and grapes sink due to their varying densities, achieving a 93% separation efficiency, exceeding our initial 90% goal.
This prototype is intended for use at the initial stage of grape processing, where harvested batches can be submerged and agitated to quickly remove invasive pests.

## Testing and Results 
Test 1: Identifying Optimal RPM
The primary objective of the product is to separate SLF from grapes. We wanted to test at what RPM separation is most effective. In previous testing, we identified that single-directional spinning was more effective than bi-directional agitation. In this test, we aim to refine our separation method.
Results
Observed that at low RPM (~3000 RPM), the majority of grape models sink, and SLF models get the most effectively separated at 3000 RPM. As the RPM increases above the 3000 ~ 4000 range,  grape models do not effectively sink and float with SLF models due to the excessively strong vortex created by the agitation. The highest separation efficiency of 93% is reached at approximately 3000 RPM.

Test 2: Leak Test
The design must be able to hold water without significant leakage since the separation mechanism relies on water to separate the grapes from the SLF. 
We tested the four most leak-prone areas in our design: areas 1,2 and 3 (highlighted orange) are where the side walls interface, and the blue highlighted area is near the agitator. 

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
The device is assembled by seating a bearing and an o-ring into the baseplate to house the agitator shaft. Three side walls are then joined and secured to the base using RTV sealant for its vibration resistance and water-blocking properties. The 3D-printed basin is mounted to a stand, where a motor spinning up to 7000 RPM is integrated. Finally, the agitator is attached to the motor shaft using a standard ASME press-fit reinforced with epoxy. 

**Testing methodology for separation efficiency.** 
To model the SLF and grapes, we used 3D printed models that were accurate to the density shown in the image on the right. SLF models (cylinders) with density 1g/cm3 and grape models (spheres) with density 1.1g/cm3 (3,4).
We placed 10 SLF models and 10 grape models into the container and ran the motor at varying RPMs ranging from 500 to 7000. For each of the three trials per RPM, we ran the motor for 30 seconds and then counted the number of SLF that floated to the surface (NSLF float )and the number of grapes that sunk (Ngrapes sunk ). 
Then we calculated separation efficiency using the following formula:
Separation efficiency=NSLF float + Ngrapes sunk Ngrapes + NSLF  =NSLF float + Ngrapes sunk 20 
Testing Methodology for Leak Test
Each leak-prone area was submerged each for 1 minute using an arbitrary controlled amount of water, and the number of drops was counted.

**Test for Structural Integrity and Fastening**
In addition to a leak test and a test for separation efficiency, we also tested the structural integrity of the connection between the motor shaft and the agitator. One key safety concern is that the agitator head must not come loose from the motor shaft during testing. 
Methodology
To test the connection, we performed a cycling test of 20 cycles, each lasting 30 seconds, and then inspected the attachment between the motor shaft and the agitator for signs of loosening.
  Results
After several tests, the shaft started spinning within the agitator without causing the agitator to spin. To combat this, we used a quick-setting epoxy adhesive, after which there were no more issues with adhesion between the agitator and the motor. 



