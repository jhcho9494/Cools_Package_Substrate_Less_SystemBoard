# Cools Package-Substrate-Less SystemBoard

## Transferred-RDL Motherboard Platform for AI, HPC and CPO

> **Flatness is borrowed from a carrier.**  
> **Fine-line routing is transferred.**  
> **The motherboard stays coarse.**  
> **The package substrate disappears.**

**Cools** proposes a system-level packaging architecture in which high-density redistribution wiring is fabricated on a separate flat carrier, electrically tested, and transferred directly onto a coarse-pitch system board or thermally active backbone.

The objective is not to make the entire motherboard into a fine-line printed circuit board. The objective is to place fine-line routing only where it creates system value, while retaining the manufacturability, area and mechanical function of the motherboard.

[한국어](README_KR.md) | [中文](README_ZH.md) | [Patent Portfolio](PATENT_PORTFOLIO.md) | [Public Notice](PUBLIC_NOTICE.md)

---

## 1. The Structural Shift

### Conventional advanced packaging

```text
GPU / ASIC / HBM / Chiplets
            ↓
       Interposer
            ↓
   Organic Package Substrate
            ↓
        Motherboard
```

### Fine-line motherboard approach

```text
GPU / ASIC / HBM / Chiplets
            ↓
       Interposer
            ↓
 Fine-Line System PCB at Large Area
```

This approach transfers the package-substrate routing burden to a large, rough and warped system board, creating a major yield and alignment challenge.

### Cools architecture

```text
GPU / ASIC / HBM / Chiplets
            ↓
Transferred High-Density RDL Overlay
            ↓
Coarse-Pitch System Board or Thermal Backbone
```

The transferred redistribution layer provides fine-pitch interconnection, fan-out, signal routing, power/ground redistribution and local die-to-die connection. The underlying system board remains coarse-pitch and does not need to be fabricated as a large-area fine-line PCB.

---

## 2. One Platform, Multiple Scales

The same transfer architecture can be deployed at different physical scales.

### Local RDL Patch

A small redistribution patch is placed only beneath GPU–HBM, chiplet-to-chiplet, switch-ASIC, optical-engine or other high-density interconnect regions.

- Fine-line routing exists only where required.
- The package substrate can be removed.
- The motherboard remains coarse-pitch.
- Local patches may be manufactured, inspected and replaced independently.

### Multi-Zone Fan-Out Overlay

A single transferred structure can contain multiple planar conversion zones, each having a different fan-out ratio for logic dies, HBM stacks, power-management devices or photonic devices.

### Board-Scale RDL Skin

A large-area or substantially full-area redistribution skin can be transferred onto a coarse motherboard to create a redistribution-integrated system board without directly patterning the motherboard at fine pitch.

### Known-Good Tile Network

A large redistribution surface can be assembled from separately manufactured and tested known-good tiles. Adjacent tiles are electrically joined by inter-tile bridge redistribution wiring.

This architecture changes the discard unit from an entire large-area RDL sheet to an individual tile.

---

## 3. Core Platform Building Blocks

| Building block | System function |
|---|---|
| Transferred fine-wiring body | Moves fine-line formation away from the rough system board |
| Local RDL patch | Concentrates advanced routing only at high-value interconnect regions |
| Board-scale RDL skin | Converts a coarse motherboard surface into a high-density routing plane |
| Multi-zone fan-out | Matches different die pitches within one transferred body |
| Known-good RDL tiles | Secures large-area effective yield through pre-test and replacement |
| Inter-tile bridge RDL | Creates a continuous or functionally continuous routing network |
| Reusable carrier | Distributes carrier cost across repeated manufacturing cycles |
| Detectable structural fingerprints | Identifies that the wiring body was fabricated on a carrier and transferred |
| Compliant joint architecture | Replaces the thermo-mechanical buffering previously supplied by an organic package substrate |
| Planar insulating reference surface | Converts rough or conductive thermal materials into a fine-wiring-compatible surface |
| Insulated through-electrode | Enables vertical electrical connection through a conductive thermal backbone |
| Electro-optical overlay | Integrates electrical RDL and optical waveguides in one transferable body |

---

## 4. Manufacturing Routes

The architecture is independent of a single metallization method.

### Route A — Existing Semi-Additive Process

A fine-wiring structure is formed on a flat temporary carrier using the semi-additive process already used by PCB and package-substrate manufacturers.

```text
Flat carrier
→ seed formation
→ resist patterning
→ pattern electroplating
→ seed flash etching
→ multilayer build-up
→ inspection
→ carrier release
→ direct transfer to the system board
```

The critical change is the processing surface, not necessarily the installed factory equipment. Fine patterning is performed on a flat carrier rather than directly on a rough and warped motherboard.

### Route B — Ultra-Thin Copper-Foil Carrier, No Vacuum Seed

An ultra-thin copper foil attached to a carrier acts as the common electroplating feed layer. Pattern electroplating and multilayer build-up can therefore be performed without forming a physical-vapor-deposited seed layer on the carrier side.

After carrier separation, the ultra-thin foil is wholly or selectively etched to expose embedded terminals and detectable recessed terminal structures.

### Route C — Wet Interface-Directed Metallization

Amine-containing interface layers such as polyethyleneimine or ethoxylated polyethyleneimine can direct catalytic metal capture and electroless barrier/seed formation. Adhesion anchoring, nucleation control, metal-ion capture, diffusion blocking and low-resistance copper routing can be assigned to separate functional layers.

This route is applicable to glass, ceramic, insulating films and selected high-aspect-ratio structures.

---

## 5. Thermally Active System Backbone

The transferred RDL concept can be combined with a high-thermal-conductivity structural backbone rather than a conventional organic motherboard alone.

Candidate backbones include reaction-bonded silicon carbide, silicon carbide, metal–ceramic composites and other high-stiffness, high-thermal-conductivity materials.

### Surface conversion

A rough, porous or electrically conductive backbone surface can be converted into a wiring-compatible surface through:

```text
Pore sealing
→ insulating over-deposition
→ lapping / polishing / CMP
→ planar insulating reference surface
→ direct RDL formation or RDL transfer
```

### Cooling-channel integration

The backbone may contain internal or bottom-side cooling channels. Electrical through-connections can pass through the conductive backbone using insulating liners and hermetic isolation from the coolant.

The conductive backbone may additionally serve as a ground reference or electromagnetic shield around selected insulated vias.

### Result

The motherboard becomes more than a passive wiring panel. It can become a unified system backbone providing:

- fine and coarse electrical routing,
- mechanical support,
- vertical interconnection,
- heat spreading,
- direct liquid-cooling compatibility,
- grounding and shielding.

---

## 6. Reliability, Yield and Detectability

### Known-Good Transfer

The fine-wiring body or each tile can be electrically and optically inspected before being attached to the final board. Open/short, resistance, insulation, impedance and continuity tests can be completed before expensive semiconductor devices are committed.

### Replaceable Tiles and Patches

Local release regions, reworkable bond lines and bridge repair routing can allow a defective tile or patch to be removed and replaced without discarding the entire system board.

### Thermo-Mechanical Stress Buffering

Removing the organic package substrate also removes one of the conventional stress-buffering layers. The Cools platform therefore includes joint-level buffering structures such as:

- low-modulus buffer layers,
- compliant conductive pillars,
- curved redistribution interconnects,
- enlarged or dummy peripheral joints,
- reinforcing frames combined with compliant joints.

### Detectable Structural Fingerprints

A transferred body can be distinguished from wiring directly built on a motherboard through measurable features including:

- a carrier-derived planar reference surface,
- reverse via taper or mirror-image build-up order,
- semi-additive seed-etch traces,
- release-layer residue,
- diced sidewalls and bond lines,
- pitch-domain separation between the fine overlay and coarse board.

These features support objective identification of the transfer architecture in a finished product.

---

## 7. Electrical–Optical Extension

The transferable body can integrate both an electrical redistribution layer and an optical-waveguide layer.

```text
Electrical fine RDL
+ optical waveguide routing
+ electrical pads and optical couplers
+ photonic-integrated-circuit interface
= transferable electro-optical overlay
```

Potential implementations include polymer, glass, silicon-nitride or silicon-dioxide waveguides, together with grating couplers, edge couplers, mirrors or optical vias.

This extends the platform from AI/HPC electrical interconnection toward co-packaged optics and board-level optical input/output.

---

## 8. System-Level Comparison

| Item | Conventional package stack | Fine-line motherboard approach | Cools transferred-RDL platform |
|---|---|---|---|
| Package substrate | Required | Reduced or removed | Removed in the target architecture |
| Fine-line fabrication location | Interposer and package substrate | Large system PCB | Separate flat carrier |
| Motherboard pitch | Coarse | Must become fine | Remains coarse |
| Large-area yield unit | Package/interposer | Entire fine-line board | Patch, sheet or known-good tile |
| Rework | Limited | Board-level difficulty | Patch/tile replacement architecture |
| Thermal integration | Added cooling hardware | PCB-limited | Compatible with high-conductivity cooling backbone |
| Electrical–optical integration | Separate structures | Board-specific | Transferable integrated overlay |

---

## 9. Target Applications

- AI accelerator boards
- GPU and High Bandwidth Memory systems
- Chiplet-based heterogeneous integration
- Package-substrate-less semiconductor modules
- Co-packaged optics boards
- High-speed switch and optical-engine boards
- High-performance computing systems
- Power-semiconductor modules
- Liquid-cooled computing backbones
- Large-area panel-level redistribution systems

---

## 10. Patent Architecture

The Cools portfolio is organized as a connected system rather than a single isolated invention.

### Core architecture

- Temporary-carrier-transferred high-density redistribution body
- Local fine-RDL patch directly attached to a coarse system board
- Board-scale transferred RDL skin
- Package-substrate-function-integrated motherboard

### Manufacturing

- Semi-additive processing on a flat carrier
- Ultra-thin-copper-foil carrier without vacuum seed deposition
- Wet interface-directed metallization
- Reusable carrier with permanent protection and consumable release layers

### Yield and reliability

- Known-good tile network and inter-tile bridge RDL
- Multi-zone fan-out conversion
- Compliant thermo-mechanical joint structure
- Detectable transfer fingerprints

### Thermal and vertical integration

- Planar insulating reference surface on a rough thermal backbone
- Insulated through-electrode through a conductive cooling backbone
- Surface-bonded-carbon reaction-bonded silicon-carbide material platform

### Future system extension

- Transferable electro-optical redistribution overlay

See [PATENT_PORTFOLIO.md](PATENT_PORTFOLIO.md) for the detailed public portfolio map.

---

## 11. Development and Collaboration Scope

Cools is open to discussions concerning:

- patent licensing,
- field-limited or region-limited rights,
- process and architecture transfer,
- joint development,
- prototype and sample evaluation,
- strategic investment,
- assignment or transfer of related registered or pending patent rights.

Target collaborators include semiconductor manufacturers, advanced-packaging companies, PCB and package-substrate manufacturers, glass and ceramic substrate companies, cooling-system companies, photonics companies and AI/HPC system integrators.

---

## 12. Public Technical Notice

This repository provides a public technical and commercial overview of the Cools platform. It does not disclose all implementation details, process windows, material specifications, drawings, claim language or non-public know-how.

The disclosed concepts may be protected by pending patent applications, future applications and confidential know-how. Publication in this repository does not grant any license, waiver, authorization or right to manufacture, use, sell, import or transfer the disclosed technology.

**Cools — Jinhyun Cho**  
Republic of Korea
