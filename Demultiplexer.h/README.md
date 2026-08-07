# 1-to-4 Demultiplexer using Verilog

## Overview

This project implements a **1-to-4 Demultiplexer (DEMUX)** using Verilog HDL. A demultiplexer routes a single input to one of four outputs based on the values of two select lines.

## Features

- 1-to-4 Demultiplexer implementation
- Combinational logic design
- Modular Verilog code
- Testbench included
- Compatible with Visual Studio Code and Icarus Verilog

## Truth Table

| D | S1 | S0 | Y0 | Y1 | Y2 | Y3 |
|---|----|----|----|----|----|----|
| 1 | 0 | 0 | 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 | 1 | 0 | 0 |
| 1 | 1 | 0 | 0 | 0 | 1 | 0 |
| 1 | 1 | 1 | 0 | 0 | 0 | 1 |

## Simulation

Compile:

```bash
iverilog -o demultiplexer demultiplexer.v demultiplexer_tb.v
```

Run:

```bash
vvp demultiplexer
```

## Expected Output

```text
D S1 S0 | Y0 Y1 Y2 Y3
----------------------
1  0  0 |  1  0  0  0
1  0  1 |  0  1  0  0
1  1  0 |  0  0  1  0
1  1  1 |  0  0  0  1
```

## Requirements

- Visual Studio Code
- Icarus Verilog
- Verilog HDL Extension (optional)

## License

MIT License