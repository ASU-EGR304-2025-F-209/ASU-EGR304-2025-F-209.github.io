---
title: Product Requirements
tags:
- tag1
- tag2
---

## Project Objective

This project aims to investigate and develop smart adaptive technologies, an improved user experience, better fit, improved product design, and product customization options for the next-generation of home door sensors. The target is to create a working prototype by the end of 2025. We aim to create a product that is better than existing products by focusing on implementing user feedback.

## Stakeholders

- **Target group** Home owners or apartment renters. They fit the use-case of the product. The main benefits are security and energy savings.
- **Target purchaser** Target group profile with special attention to Full Nest I and Full Nest II mothers.
- **Customer service** Prefers easy-to-repair, easy-to-fix complaints, and clear instructions.
- **Marketing & Sales division** Looks for unique selling points around retail stores and online marketplaces.
- **Retailers** Prefer products that can withstand a wide range of storage conditions including variations in temperature, vibration, humidity, and atmospheric pressure, and have a strong and compact, theft, and vandalism-proof packaging.


## Use Cases

* **User Story #1: Matthew**
Matthew is a 33-year-old new homeowner. He is looking for something to provide some extra security to his home. His new smart door sensor allows him to sleep easy knowing it will alert him to any theives breaking in at night.<br>
Matthew also likes to travel. His new smart door sensors allow him to know whenever a door is open by alerting him on his phone. 

* **User Story #2: Alice**
Alice is a 27-year-old mother of three boys. She is looking for a device to monitor when her children open the door and leave the house while with the door open. This smart door sensor assists her by alerting when the door has been left open for a while, and when the door is used by her children.<br>
This device provides ease for the mother from having to check up on the door whenever it is used.

## Aspects

The product design will be based on highlights of the benchmarked products while adhering the following requirements. The **P1 - P10** is the "code" to indicate the priority of the requirement, from low to high.

1. **Producr Design**
      * 1.1 The product shall operate with a motor noise level not exceeding 40 dB. (P2)
      * 1.2 The product shall provide a tamper-resistant locking mechanism compatible with standard residential doors. (P3)
      * The product shall maintain a compact form suitable for standard US, EU, and Asian door frames. (P3)
  
2. **Functionality**
      * 2.1 The product shall provide mobile app control on both iOS and Android with secure authentication. (P10)
      * 2.2 The product shall send real-time alerts for door left open, forced entry attempts, and lock tampering. (P9)
      * 2.3 The product shall integrate with smart home ecosystems such as Google Home, Alexa, and Apple HomeKit. (P5)
      * 2.4 The product shall log and store access history including user identity and timestamp. (P2)

3. **Interactivity & User Experience**
      * 3.1 The product shall provide haptic or audio feedback when locking and unlocking. (P8)
      * 3.2 The product shall support DIY-friendly installation with clear instructions. (P5)
      * 3.3 The product shall provide an intuitive mobile app interface with a simple lock/unlock dashboard. (P9)
      * 3.4 The product shall support multi-language options in the mobile app. (P6)

4. **Customization**
      * 4.1 The product shall allow replaceable external covers and finishes for aesthetic preferences. (P2)
      * 4.2 The product shall allow customization of lock/unlock sounds and app themes. (P7)
      * 4.3 The product shall support optional add-on modules such as a camera or keypad. (P5)

5. **Manufacturing**
      * 5.1 The product shall be designed to meet a durability standard of at least 100,000 lock/unlock cycles. (P10)
      * 5.2 The product shall use energy-efficient components that allow a minimum battery life of one year using 4 AA batteries. (P8)
      * 5.3 The product shall be designed with modular components to allow easy replacement of faulty parts. (P6)
      * 5.4 The product shall be packaged using environmentally friendly materials. (P1)

6. **Safety**
      * 6.1 The product shall provide fail-safe operation to unlock in fire or emergency situations if power is cut. (P9)
      * 6.2 The product shall include finger entrapment and pinch protection in its mechanical design. (P8)
      * 6.3 The product shall resist brute-force attacks up to at least 1,000 pounds of force. (P6)
      * 6.4 The product shall provide tamper detection and issue alerts in case of forced entry. (P5)
      * 6.5 The product shall include overheat protection for the motor and PCB. (P7)


## Requirement Criteria Specifications

* 1.1.1 – The motor shall not exceed 40 dB measured at 1 meter distance under normal operation.
* 1.2.1 – The mechanism shall withstand at least 1,000 lb of direct force without failure.
* 2.1.1 – The mobile app shall be compatible with iOS 15+ and Android 11+.
* 2.2.1 – The system shall support push notifications via mobile app.
* 2.3.1 – The lock shall support API protocols required by Google, Alexa, and Apple ecosystems.
* 2.4.1 – The log shall store at least 500 access events locally.
* 3.1.1 – The device shall provide a vibration within 1 second of access.
* 3.2.1 – The product shall be installable using only a standard screwdriver.
* 3.2.2 – The product shall include a step-by-step installation guide with diagrams.
* 3.3.1 – The main dashboard shall allow one-click lock/unlock.
* 3.4.1 – The app shall support at least English, Spanish, and Mandarin.
* 4.1.1 – At least three finish options shall be available (e.g., coated aluminum, matte black, stainless steel).
* 4.2.1 – The app shall provide at least two theme color schemes.
* 4.3.1 – The product shall include a modular port for expansion modules.
* 5.1.1 – The locking mechanism shall pass a 100,000-cycle test at room temperature.
* 5.1.2 – The locking mechanism shall pass a 50,000-cycle test at elevated humidity (RH ≥ 80%).
* 5.2.1 – The lock shall consume less than 500 µA in standby mode.
* 5.2.2 – The system shall complete at least 50,000 lock/unlock operations on a single set of batteries.
* 5.3.1 – The PCB, motor, and sensor assembly shall be separable via connectors.
* 5.4.1 – Packaging shall use 90% recyclable material by weight.
* 5.4.2 – Plastic packaging shall be biodegradable or recyclable.
* 6.2.1 – The lock shall default to an unlocked state if internal power is lost.
* 6.2.2 – The lock shall provide weeks of prior notice before internal power is lost.
* 6.3.1 – The gap between moving parts shall not exceed 4 mm to prevent finger trapping.
* 6.4.2 – The circuit shall use thermal fuses rated at 85°C.
* 6.5.1 – The mounting hardware shall withstand torque forces up to 100 N·m.
* 6.6.1 – Tamper detection shall trigger a local alarm and send a remote alert within 5 seconds.

## Open Questions

* Can we move towards a recyclable and repairable product, for example, with ZIF connectors and glue-free assembly?
* Can we improve on failing or self-igniting batteries?
