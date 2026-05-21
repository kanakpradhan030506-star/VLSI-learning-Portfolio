# Flip Flops — SR, JK, D, T
**Tool:** Xilinx ISE 14.7
**Language:** VHDL,Verilog
**Topic:** Sequential Logic Design

## Overview
All four flip flops implemented in three
coding styles each:
- Behavioral — describes what circuit does
- Dataflow — describes data movement
- Structural — gate level connections

## SR Flip Flop
**Truth Table**
| S | R | Q | Action |
|---|---|---|--------|
| 0 | 0 | Q | Hold |
| 0 | 1 | 0 | Reset |
| 1 | 0 | 1 | Set |
| 1 | 1 | X | Invalid |

### Schematic
![SR Schematic](SR-FlipFlop/schematic.png)

### Behavioral Waveform
![SR Behavioral](SR-FlipFlop/waveform_behavioral.png)

### Structural Waveform
![SR Structural](SR-FlipFlop/waveform_structural.png)

### Dataflow Waveform
![SR Dataflow](SR-FlipFlop/waveform_dataflow.png)

---

## JK Flip Flop
**Resolves invalid state of SR when J=K=1 by toggling**

### Schematic
![JK Schematic](JK-FlipFlop/schematic.png)

### Behavioral Waveform
![JK Behavioral](JK-FlipFlop/waveform_behavioral.png)

### Structural Waveform
![JK Structural](JK-FlipFlop/waveform_structural.png)

### Dataflow Waveform
![JK Dataflow](JK-FlipFlop/waveform_dataflow.png)

---

## D Flip Flop
**Most widely used FF — foundation of registers**

### Schematic
![D Schematic](D-FlipFlop/schematic.png)

### Behavioral Waveform
![D Behavioral](D-FlipFlop/waveform_behavioral.png)

### Structural Waveform
![D Structural](D-FlipFlop/waveform_structural.png)

### Dataflow Waveform
![D Dataflow](D-FlipFlop/waveform_dataflow.png)

---

## T Flip Flop
**Toggles on every clock — used in counters**

### Schematic
![T Schematic](T-FlipFlop/schematic.png)

### Behavioral Waveform
![T Behavioral](T-FlipFlop/waveform_behavioral.png)

### Structural Waveform
![T Structural](T-FlipFlop/waveform_structural.png)

### Dataflow Waveform
![T Dataflow](T-FlipFlop/waveform_dataflow.png)

---

## Key Learnings
- All three styles produce identical simulation results
- Behavioral is fastest to write, structural shows gate details
- Dataflow using assign statements is cleanest for simple logic
- JK and T can be derived from SR and D respectively

## Connection to Future Work
These sequential elements form the register file
and pipeline stages of my upcoming RISC processor project.
