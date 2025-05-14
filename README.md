# EEE3088F-Project-PCB-Files-Group-36-TRKJON002-MTMTAD006

EEE3088F Project Power PCB KiCad Design

## Project Overview

This repository contains the design files for the power PCB subsystem of a micro mouse robot, a project undertaken as part of the EEE3088F course. The power PCB is a crucial component responsible for providing and managing power for the entire micro mouse system, enabling its autonomous navigation capabilities.

## Project Requirements

The power PCB design is required to meet the following specifications:

* Operate up to 4 motors bidirectionally. These include 2x brushed DC motors which could each draw 200mA at the highest voltage of a 1S1P battery. The other 2x motors are for the auxiliary connection and need to operate 500mA each.
* Place an INA219 for monitoring the battery on the I2C Bus and configure it correctly with respect to the hardware (cannot have BOTH A0 AND A1 on GND).
* Charge the battery from the 9V input pin.
* Have two charging modes for a higher and lower charging current for the battery (200mA ±100mA, and approximately 600mA±100mA from the battery perspective).
* Integrate USB C and get 9V out of the USB Host.
* Provide 2x External Load Switching at 1A each (High Side connected to your 5V).
* Provide a 3v3 5% accuracy (300mA max) and 5V Out 5% accuracy (1.5A max).
* Provide an ON/OFF switch. **OFF state:** battery draw <30uA. **ON state:** can provide your robot peak current of 2A. The switch needs to shut down 5V and 3V3.

## Repository Structure

This repository utilizes the following branches to manage the project's development:

* **main:** This branch contains the first iteration of the PCB design.
* **jonathans\_branch:** This branch includes separate modifications that were developed and subsequently merged into the `main` branch.
* **design2:** This branch represents the culmination of all changes made throughout the project and contains the final design of the power PCB. For the latest and final version of the design, please refer to this branch.

## Cloning Instructions
To obtain the latest version of the power PCB design, you can clone the `design2` branch directly using the following command:

```bash
git clone -b design2 [https://github.com/GoldenExperienceR/EEE3088F-Project-PCB-Files-Group-36-TRKJON002-MTMTAD006.git](https://github.com/GoldenExperienceR/EEE3088F-Project-PCB-Files-Group-36-TRKJON002-MTMTAD006.git)
