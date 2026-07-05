\# Reference Design Study



This document explains how the DC2150C reference design was used as the basis for this PCB portfolio project.



\## Purpose



The purpose of this project was not to create a completely new surge protection architecture from scratch.



Instead, the goal was to study an existing high-quality reference design, understand its functional blocks, extract the recommended component structure, and recreate the schematic and PCB layout independently in Altium Designer.



This approach was used as a learning exercise for:



\- Reading reference design documentation

\- Understanding protection circuit architecture

\- Reconstructing a schematic

\- Preparing a manufacturable PCB layout

\- Generating production files

\- Documenting a hardware design project for portfolio use



\## Reference Design



The project was inspired by the Analog Devices DC2150C reference design.



The DC2150C architecture was studied to understand how LTC4366 and LT4363-based protection stages can be combined in a harsh DC input protection board.



This project follows the general functional structure of the reference design, but the schematic and PCB layout were recreated as an independent Altium Designer exercise.



\## Functional Blocks Studied



The following functional blocks were studied and recreated:



\- Input protection section

\- LTC4366 front-end protection stage

\- Power MOSFET control path

\- Anti-ripple capacitor bank

\- Charge pump section

\- LT4363 surge stopper section

\- Current sense network

\- Protected output section

\- Status and connection section



\## Component Selection Approach



The component selection was based on the recommended BOM structure of the reference design.



The goal was to understand why each major component exists in the protection chain rather than only copying component values.



The most important component groups are:



\- Protection controllers

\- External MOSFETs

\- TVS diode

\- Power diode

\- Current sense resistor

\- Timing and feedback resistors

\- Gate resistors

\- Ripple capacitors

\- Output capacitor

\- Indicator components

\- Input and output connectors



\## Schematic Recreation



The schematic was recreated in Altium Designer using a block-based organization.



The major schematic sections are:



\- Power Guardian

\- LTC4366

\- Anti-Ripple

\- Charge Pump

\- Surge Stopper

\- Connection



This structure makes the schematic easier to review and helps show the functional role of each part of the design.



\## PCB Recreation



The PCB was designed as a two-layer board.



The layout was created to reflect the main power flow from input to output.



The main layout priorities were:



\- Wide copper areas for high-current paths

\- Thermal via arrays for heat spreading

\- Clear input/output separation

\- Short gate and sense routing

\- Readable functional labels

\- Manufacturable two-layer structure

\- Clean production output generation



\## Why This Project Matters



Reference designs are an important part of real hardware engineering.



A good engineer should be able to:



\- Read a reference design

\- Understand the purpose of each block

\- Identify critical components

\- Recreate the design in a CAD tool

\- Make layout decisions based on current flow and thermal behavior

\- Generate manufacturing outputs

\- Clearly document design assumptions and limitations



This project was created to demonstrate exactly that workflow.



\## Difference Between Inspired and Certified



This board should be described as:



\- DC2150C-inspired

\- MIL-STD-1275D-inspired

\- Design-only

\- Portfolio-oriented

\- Not manufactured

\- Not electrically tested



It should not be described as:



\- MIL-STD-1275D-certified

\- MIL-STD-1275D-compliant

\- Production-ready

\- Field-validated

\- Tested for military vehicle use



The project demonstrates design understanding and PCB implementation skill, not formal compliance.



\## Future Improvements



Future development could include:



\- Manufacturing the PCB

\- Assembly and visual inspection

\- Low-voltage bring-up

\- Current-limited power testing

\- Gate waveform validation

\- Surge response testing

\- Thermal measurement under load

\- Reverse input test

\- Comparison with the original reference design measurements

\- Design revision after test results



A manufactured and tested revision could later be documented as Rev-B.

