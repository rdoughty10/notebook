---
doc-type:
  - protocol
protocol name:
  - Reverse Transcriptase and PCR - Tiled Amplicon
seq pools:
---

# Reverse Transcriptase and PCR
 #ReverseTranscriptase #RT #PCR  #TiledAmplicon #PrimerPools 

| Version | Date         |
| ------- | ------------ |
| 1.2     | Mar 26, 2025 |

Adapted from: ARTIC SARS-CoV-2 sequencing protocol v4 (LSK114) V.4
DOI: [dx.doi.org/10.17504/protocols.io.bp2l6n26rgqe/v4](https://dx.doi.org/10.17504/protocols.io.bp2l6n26rgqe/v4)
- Josh Quick, University of Birmingham
- Lauren Lansdowne, University of Birmingham
#### Reagents

| Name                                                   | Company                 | Part number | Lot | Notes |
| ------------------------------------------------------ | ----------------------- | ----------- | --- | ----- |
| LunaScript RT SuperMix Kit                             | NEB                     | E3010       |     |       |
| Q5 Hot Start High-Fidelity 2X Master Mix               | NEB                     | M0494       |     |       |
| Nuclease-free water (100 mL)                           | NEB                     | B1500       |     |       |
| AMPure XP beads                                        | Beckman                 | A63881      |     |       |
| Qubit 1X HS-dsDNA Assay Kit                            | Invitrogen/ThermoFisher | Q33231      |     |       |
| D1000 ScreenTape (or D5000 with amplicons over 900 nt) | Agilent                 | 5067-5582   |     |       |

#### Equipment

| Company                          | Model                             | Name/ID          | Notes |
| -------------------------------- | --------------------------------- | ---------------- | ----- |
| Invitrogen/ThermoFisher          | Qubit Flex Fluorometer            | Quantumania      |       |
| Agilent                          | 4150 TapeStation System           | CMMR Tapestation |       |
| ThermoFisher (AppliedBiosystems) | VeritiPro Thermal Cycler (A48141) | Charles          |       |
| ThermoFisher (AppliedBiosystems) | VeritiPro Thermal Cycler (A48141) | Cyndi            |       |

#### Experimental material

| Material             | Notes                                  |
| -------------------- | -------------------------------------- |
| RNA of sample        |                                        |
| Positive control     | Include name and dilution factor       |
| Primer pools (100µM) | Name/ID for all pools for target virus |

## Protocol

### Preparation:
1) Thaw on ice, **flick mix**, spin, keep on ice:
	- RNA samples
	- Positive Control
	- Primer Pool stock (100µM)
2) Prepare a *dilution* of the positive control in nuclease free water as necessary [^2] 
3) Thaw on ice, **pipette/invert mix**, spin, keep on ice:
	- LunaScript RT SuperMix
4) Thaw at Room Temperature, **pipette mix** to break up any precipitate, spin, keep on ice:
	- Q5 Hot Start High-Fidelity 2X Master Mix
### cDNA preparation
1) Prepare RNA samples (at least 11 is typical for 1 flow cell) [^1], and at least 1 negative control and 1 positive control. Flick mix and pulse spin. **Keep samples on ice at all times.**
2) Mix the following components in a PCR strip-tubes/plate [^3]. Gently mix by hand inverting and flicking, then pulse spin the tube to collect liquid. [^4]

>[!Important]
>10 ul of cDNA product is enough for 4 "standard" PCR reactions (2.5 ul/reaction). 1 virus assay typically has two PCR pools/reactions. The volume of samples/reagents for the RT step can be scaled up and down as required.

| Component              | Volume    |
| ---------------------- | --------- |
| LunaScript RT SuperMix | 2 µL      |
| Template RNA           | 8 µL      |
| **Total**              | **10 µL** |
3) Incubate the reaction as follows:

| Temperature (°C) | Time (hr:m:s) |
| ---------------- | ------------- |
| 25 °C            | 00:02:00      |
| 55 °C            | 00:10:00      |
| 95 °C            | 00:01:00      |
| 4 °C             | Hold          |
|                  |               |

> [!Stopping Point]
> cDNA products can be stored at −20°C for up to a month or 4°C overnight.
### Primer Pool preparation
1) Prepare 10µM working stocks by making a 1:10 dilution of the 100µM primer pool in molecular grade water [^5], vortex, and spin.

 > [!Note]
> 	Make multiple 100µl aliquots of 10µM primer dilutions and freeze them to avoid degradation or contamination.

### Multiplex PCR
1) Set up TWO PCR reactions per sample as follows in strip-tubes or plates. Gently mix by pipetting and pulse spin the tube to collect liquid at the bottom of the tube.

| Component                                | Reaction 1 | Reaction 2 |
| ---------------------------------------- | ---------- | ---------- |
| Q5 Hot Start High-Fidelity 2X Master Mix | 12.5 µL    | 12.5 µL    |
| Pool 1 (10µM)                            | 4 µL       | 0 µL       |
| Pool 2 (10µM)                            | 0 µL       | 4 µL       |
| Nuclease-free water                      | 6 µL       | 6 µL       |
| Total                                    | 22.5 µL    | 22.5 µL    |
> [!Note]
> 	Make a master mix of each Primer Pool reaction for the total number of samples and aliquot to each PCR tube (or plate well).

2) Add 2.5 µl of cDNA to each of the PCR reactions, gently mix by pipetting and pulse spin the tube to collect liquid at the bottom of the tube. [^6]
3) Incubate [^7]  the reaction as follows : 

|                 | Temperature (°C) | Time (hr:m:s) | Cycles |
| --------------- | ---------------- | ------------- | ------ |
| Heat Activation | 98 °C            | 00:00:30      | 1      |
| Denaturation    | 98 °C            | 00:00:15      | 35     |
| Annealing       | 65 °C            | 00:05:00      | ^       |
| Hold            | 4 °C             | Hold          | 1      |

4) In clean 0.2 ml thin-walled PCR tubes (or a clean 96-well plate), combine equal volumes of each PCR reaction for each sample.
> [!Stopping Point]
> PCR products can be stored at −20°C for up to a month.

### PCR Bead Cleanup
#### Preparation
- Thaw at Room Temperature for at least 30 minutes, **vortex mix**, keep at Room Temperature: 
	- AMPure Beads
- Prepare 500 μl per sample of fresh 80% ethanol in Nuclease-free water
#### Steps
1) Perform a bead clean up (see table) by adding appropriate amount of AMPure XP beads to 50µL pooled PCR product. Mix until homogenous via gentle pipetting.

| Aplicon Size | Ampure Bead Concentration | Bead Volume (50 ul product) |
| ------------ | ------------------------- | --------------------------- |
| 280          | 1X                        | 50 ul                       |
| 400          | 0.8X                      | 40 ul                       |
| 1,000        | 0.6X                      | 30 ul                       |

1) Incubate for 5 minutes at room temperature.
2) Spin down the sample, then pellet on a magnet. Keep the tube on the magnet, and pipette off the supernatant.
3) Keep on magnet, wash beads with 200 µl of freshly prepared 80% ethanol without disturbing the pellet. Remove the 80% ethanol using a pipette and discard.
4) Repeat the previous step with new pipet tips.
5) Spin down and place the tube back on the magnet. Pipette off any residual 80% ethanol. Briefly allow to dry. *Max 2 minutes.*
6) Remove the tube from the magnetic rack and resuspend pellet in 16 µl Nuclease-free water. Mix via gentle pipetting until pellet is resuspended. 
7) Incubate for 2 minutes at RT.
8) Pellet beads on magnet until the eluate is clear and colourless
9) Remove and retain 15 µl of eluate into a clean 1.5 ml Eppendorf DNA LoBind tube.

>[!warning]
>Try to avoid beads at this step.
>Leave behind ~1 ul of liquid to reduce bead carryover.

> [!Stopping Point]
> 	Cleaned PCR products can be stored at −20°C for up to a month.

### Quantification of PCR Amplicons
1) Quantify 1 µl of PCR amplicon using a Qubit dsDNA HS Assay Kit
2) Verify the quality of the PCR amplicon using TapeStation D1000 or D5000 DNA ScreenTape assays
3) Calculate the fmol of each PCR amplicon and move forward with 200 fmol (*53 ng for 430 nt amplicons*) to Library Prep: [[Library Prep - Ligation sequencing (SQK-NBD114.24) - Tiled Amplicon]]

## Footnotes

[^1]: At least 11 samples are required to have sufficient material to load on the sequencer at the end. If you process >23 you will need the EXP-NBD196 expansion kit.

[^2]: A positive control can also be included which may be a synthetic RNA constructs or hightitre clinical sample which can be diluted. This can help monitor run performance.

[^3]: To prevent pre-PCR contamination the mastermix should be added to the PCR striptubes/plate in the mastermix cabinet which should should be cleaned with decontamination wipes and UV sterilised before and after use.

[^4]: Viral RNA input from a clinical sample should be between Ct 18-35. If Ct is between 12-15, then dilute the sample 100-fold in water, if between 15-18 then dilute 10-fold in water. This will reduce the likelihood of PCR-inhibition.

[^5]: Primers are used at a final concentration of 15 nanomolar (nM) per primer. In this case ARTIC SARS-CoV-2 V3 pools have 110 primers in pool 1 and 108 primers in pool 2. so the requirement is ~ 4 µL primer pool ( 10 micromolar (µM) ) per 25 µL reaction.

[^6]: Up to 5 µL cDNA can be added to each PCR reaction (in place of nuclease-free water) to improve amplification of low titre samples. Using 5 µL cDNA will require a 20 µL cDNA reaction and may be more likely to cause inhibition so use cautiously.

[^7]: Cycle number should be 25 for Ct 18-21 up to a maximum of 35 cycles for Ct 35.


