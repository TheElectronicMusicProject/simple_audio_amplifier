# SIMPLE AUDIO AMPLIFIER

## General Information

- Creator of the project: Filippo Graziani aka Circuitry Passion
- First official release of the project: Rev.1.0 (18/08/2025)
- CAD for design: Application: KiCad 9.0.4-9.0.4-0~ubuntu22.04.1, release build

## 1 Introduction

This project is an exercise to correctly use KiCad to design a complete project.  
The amplifier consists of the LM386N audio mono amplifier with some circuitry to adjust:

- Gain
- Volume
- Bass

There is an additional dedicated circuitry to light an LED up when the device is powered on.  
The audio input is a jack socket compatible with TRRS contacts, however only the first ring is actually connected to the amplifier, leaving the second ring unconnected. This mean you must set the audio source to output a monophonic sound. The risk is to loose half of the music if stereo is used.

## 2 Technical Specifications

1) INPUT VOLTAGE  
The device can operate **from 4 V to 12 V** (compatible with the full voltage range of the LM386N). Suggested input current source **at least 500 mA** (lower is permitted but doesn't guarantee the correct operations for all the conditions).  
The external source must be connected to J1 connector, where the dot sign on the PCB corresponds to the + positive voltage.
Through the S1 swith it is possible to turn on and off the device to avoid unnecessary energy consumption.

2) INPUT AUDIO  
This device is compatible with **TRRS connectors** connected to J2. Monophonic audio source is not mandatory but it is suggested to enjoy the amplifier capabilities.  
At the moment, only the **CTIA/AHJ standard** is supported, be sure to use this kind of device.  

3) OUTPUT AUDIO  
The J3 connector must be used to connect the output amplifier to a speaker.  
Compatible output impedance goes **from 4 Ω to 32 Ω** and higher.  
The typical **output power is 325 mW**.

## Schematics

![drawing](./output/simple_audio_amplifier.svg)
