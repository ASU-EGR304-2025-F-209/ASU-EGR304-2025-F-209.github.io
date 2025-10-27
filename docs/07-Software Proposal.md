---
title: Software Proposal
---

## Introduction

The door controller firmware operates as a finite-state machine (FSM) which runs inside a cooperative main loop that follows this sequence: Read Inputs → Update State → Set Outputs. The system starts its operation by setting hardware registers to their initial values and clearing all software variables and establishing communication links between MCUs through UART and I²C interfaces and then it enters State 001 (Closed). The system checks debounced sensor inputs from magnetic reed/limit switches and distance/UART and current/thermal flags and user override buttons during each cycle. The Update State routine checks transition predicates after which Set Outputs determines motor driver and indicator output values based on the current state. The design structure produces reliable operation while making testing easier and blocking any potential output irregularities.

## Images

![image caption](StateMachineDiagram.png)

## Logic Flow

The door controller firmware operates on a series of loops that are capable of simultaneous processing among the individual subsystems. 
The system starts its operation by setting hardware registers to their initial values and clearing all software variables, and establishing communication links between MCUs.


### UltraSonic Sensor Subsystem
The Ultrasonic Sensor Subsystem initializes and runs throughout the device’s power-on time. It repeatedly sends a distance value, converted from an analog reading from the sensor to a range of values by the UART module in the MCU, to the other MCUs in the System


### Pushbutton Subsystem 
The Unlock Sequence is the first loop that follows in the flow of operations. It works using a series of push buttons that act as a number pad that enables the user to lock and unlock the door.
The pushbuttons, all connected to the MCU, draw a high value when pushed down. This is mapped to a character that is stored in the memory. 
The MCU compares the sequence of characters entered against a previously stored array of characters, either from the manufacturer or during the first startup, to check if the “Password” is correct. 
If correct, the Pushbutton subsystem sends a signal to the motor subsystem; else, a reinput is needed for unlock.


### Motor Subsystem
The motor system is initialized on State 001. It receives a signal from the “numberpad” and changes states depending on either a locking or an unlocking sequence.

**Motor State Semantics**
State 001 (Closed/Locked, Idle): The motor remains disabled while the lock remains engaged, and the status LED displays "closed."

State 002 (Moving): The H-bridge enables motor operation through direction control from commands. The H-Bridge sends power to control the direction the motor spins, which decides whether it is an unlock or lock operation.

State 003 (Open, Idle/Unlocked): The motor stays disabled while the status LED shows "open" and the auto-close timer operates in the background.

|From |Condition |to|Immediate action|
|-----------|--------|--------|---------|
|001|Unlock request| 002|Unlock
|Enable H-bridge
Start motor
Turn on LED|
|002|Open limit reached |003|Disable motor Start auto-close timer (if enabled)|
|003|Lock Request|002|Reverse H-Bridge
Start Motor|
|002|Close Limit Reached|001|Disable Motor
Turn off LED|



### Alarm Subsystem
The Alarm system is enabled as soon as the Motor subsystem's internal timer finishes counting down or the distance value exceeds the closed door value for a period of time. This Subsystem serves as a measure to ensure the door is not left open too long. 

**Alarm State Semantics**
State 001 (Closed, Idle): The alarm subsystem is idle; no components are running.

State 002 (Open/Unlocked): The timer from the motor subsystem sends a signal to the alarm subsystem. This enables the speaker that plays the warning sound and the red LED as a visual signal for the warning.

State 003 (Alarm Switch): This mode allows the user to open the door for extended periods of time when hauling a load through or for other reasons. The switch is toggled, and this disables all output to the speaker, allowing for quiet use. The warning LED is still turned on to serve as an indicator for the open door



### Determinism & Safety
* The system implements mechanical input debouncing with hysteresis to stop motor oscillations caused by chattering.
* The system will exit State 002 through watchdog and motion timeout mechanisms when the set limits are not achieved.
* The system performs a safe shutdown when it detects any obstructions through current and thermal monitoring systems.
* The system enables motor operation only after it detects valid sensor data and state verification during startup.

## Conclusions and Future Work


## References


