# Full Adder using Verilog

## Overview
This project implements a **1-bit Full Adder** using Verilog HDL. A Full Adder adds three 1-bit binary inputs (`A`, `B`, and `Cin`) and produces two outputs: `Sum` and `Carry Out (Cout)`.

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

## Boolean Expressions

- **Sum = A ⊕ B ⊕ Cin**
- **Cout = (A & B) + (B & Cin) + (A & Cin)**

## Files

- `full_adder.v` - Verilog implementation
- `full_adder_tb.v` - Testbench for simulation
- `README.md` - Project documentation

## Simulation

Compile the design and testbench using any Verilog simulator such as:
- ModelSim
- Vivado
- Xilinx ISE
- Icarus Verilog

Example (Icarus Verilog):

```bash
iverilog -o fulladder full_adder.v full_adder_tb.v
vvp fulladder
```

## Expected Output

```
A B Cin | Sum Cout
------------------
0 0 0 | 0 0
0 0 1 | 1 0
0 1 0 | 1 0
0 1 1 | 0 1
1 0 0 | 1 0
1 0 1 | 0 1
1 1 0 | 0 1
1 1 1 | 1 1
```

## Applications

- Arithmetic Logic Units (ALUs)
- Binary Adders
- Digital Signal Processing
- Processors and Microcontrollers
- Embedded Systems

## Author

**Your Name**

GitHub: https://github.com/your-username