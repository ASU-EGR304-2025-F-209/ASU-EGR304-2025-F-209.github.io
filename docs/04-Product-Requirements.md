---
title: Product Requirements
tags:
- tag1
- tag2
---

## Project Objective

This project aims to investigate and develop smart adaptive technologies, an improved user experience, better fit, improved product design, and product customization options for the next-generation of home door sensors. The target is to create a working prototype by the end of 2025. We aim to create a product that is better than existing products by focusing on implementing user feedback.

## Stakeholders

**Primary users**
The system provides door activity awareness to residential home and apartment residents who need this information for safety purposes and security needs and caregiving requirements and personal convenience. The system serves people who have mobility issues and parents with children and senior citizens who need assurance and travelers who need door status updates.

**Secondary users**
The accurate status information helps family members and caregivers who need it to support their dependent older adults and children.

**Installers**
The device requires users to perform basic setup and maintenance tasks using simple tools without needing extensive technical knowledge.

**Manufacturing and reliability teams**
The teams need to verify that the device remains functional through storage and environmental tests which occur during distribution and extended usage.

**Service and support teams**
The teams need to understand device diagnostics and repair standards and performance stability to deliver excellent customer service over time.


## Use Cases

* **Persona 1: Jordan**
The 34-year-old single parent Jordan cares for his two children who are younger than eight years old. The door status notification system must function during peak times when people enter and leave their homes. The person needs to check the door status through a device because their hands remain occupied at all times. The system must provide door status updates in real time through a simple interface that requires minimal user input. The system requires operation under both noisy and fast-paced conditions.

* **Persona 2: Kai**
The 72-year-old retired teacher Kai suffers from arthritis which limits his mobility. The door requires multiple attempts to open which leads to discomfort for him. The door needs to provide absolute confirmation of its closed position before Kai goes to sleep. The system must provide information that can be understood easily without needing quick responses or precise hand movements. The system needs to be reliable while providing easy access to information.

* **Persona 3: Sam**
Sam travels extensively because he spends extended periods outside his home. The system needs to track door activity precisely while sending alerts about unusual door behavior or extended door openings. The system needs to operate consistently for extended periods while resisting environmental stress to prevent breakdowns when no one is present.
## Requirements

1. Functional Requirements

1.1 The device shall detect door position states with at least 99 percent accuracy under normal residential use conditions.
1.2 The device shall report a change in door position within one second of that change.
1.3 The device shall store a minimum of five hundred recorded door events accessible for review.
1.4 The device shall operate without user recalibration for at least twelve months under typical usage.
1.5 The device shall function in indoor temperatures between zero and forty degrees Celsius with no performance loss measurable greater than five percent.
1.6 The device shall support operation during temporary loss of external connectivity and shall restore full reporting when connectivity returns with no user intervention.
2. Usability and Accessibility Requirements

2.1 The device shall communicate door status in a format understandable by users who have reduced hearing, reduced vision, or limited mobility.
2.2 The setup process shall be completable by a first time user in less than fifteen minutes using only basic tools commonly found in residential settings.
2.3 All user facing feedback indicators shall be perceivable at a distance of at least three meters under normal indoor lighting.
2.4 The device shall require no fine motor action smaller than ten millimeters for setup or operation.
2.5 Instructions shall be understandable at a reading level equivalent to grade eight.

3. Safety Requirements

3.1 The device shall not create pinch hazards and shall maintain a minimum physical clearance of four millimeters between moving parts.
3.2 The device shall remain safe to touch in operating conditions and shall not exceed a surface temperature of fifty degrees Celsius.
3.3 The device shall enter a fail safe state that prevents entrapment hazards if internal power is lost.
3.4 The device shall generate a user alert when its remaining power is estimated to last fewer than two weeks of normal operation.

4. Reliability and Durability Requirements

4.1 The device shall complete at least fifty thousand door state cycles without measurable degradation of accuracy greater than one percent.
4.2 The device shall withstand direct mechanical force of at least four thousand five hundred newtons without structural failure.
4.3 All components shall function after storage at humidity levels up to eighty percent for at least one month.
4.4 The device shall operate for at least twelve months on a single set of consumer replaceable batteries under standard usage assumptions.
4.5 The device shall resume normal function within five seconds following a power restoration event.

5. Environmental and Manufacturing Requirements

5.1 The device shall contain at least ninety percent recyclable material by weight.
5.2 The device packaging shall contain at least ninety percent recyclable or biodegradable material by weight.
5.3 The device design shall allow disassembly of major subassemblies in under three minutes for repair by trained service personnel.
5.4 All materials used shall comply with RoHS restrictions on hazardous substances.


## Open Questions

* What concerns do you have about forgetting to close your door?
* Can we add intrusion-detection sensors that also meet privacy expectations?
* Can we allow software customization at different levels (basic vs. advanced user modes)?
* Can the setup process be simplified to under 15 minutes for a non-technical homeowner?
* Can the app support offline operation (e.g., Bluetooth-only) for users without Wi-Fi?
