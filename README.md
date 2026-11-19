Markdown
# 4-bit ALU using Verilog HDL

## 📌 Project Overview
This project implements a 4-bit Arithmetic Logic Unit (ALU) using Verilog HDL. An ALU is a core building block of a processor, responsible for performing arithmetic, logical, and shift operations on binary inputs.

The ALU supports eight operations selected by a 3-bit control signal (`sel`), along with `carry_out` and `zero` status outputs.

## ✨ Operations Supported

| Select (`sel`) | Operation | Behavior |
| :--- | :--- | :--- |
| `3'b000` | Addition | `A + B` with `carry_out` flag |
| `3'b001` | Subtraction | `A - B` with borrow/carry status |
| `3'b010` | Bitwise AND | `A & B` |
| `3'b011` | Bitwise OR | `A \| B` |
| `3'b100` | Bitwise XOR | `A ^ B` |
| `3'b101` | Bitwise NOT | `~A` |
| `3'b110` | Left Shift | Logical shift left of `A` by 1 bit |
| `3'b111` | Right Shift | Logical shift right of `A` by 1 bit |

## 🛠 Tools Used
- Verilog HDL
- Visual Studio Code
- Icarus Verilog
- Surfer
- GitHub

## 📂 Project Files
- `alu_4bit.v` — 4-bit ALU RTL design module
- `alu_4bit_tb.v` — Testbench for functional simulation and VCD waveform generation
- `waveform.vcd` — Simulation waveform dump file
- `README.md` — Project documentation

## ▶️ Simulation

**Compile:**
```bash
iverilog -o alu alu_4bit.v alu_4bit_tb.v
Run:

Bash
vvp alu
View Waveform:
Open waveform.vcd using Surfer.

📖 Learning Outcomes
Arithmetic Operations

Logic Operations

Shift Operations

Case Statements

Combinational Circuit Design

Verilog Testbench Writing

Digital System Design

👨‍💻 Author
Rohit Bonela

ECE Student, Lendi Institute of Engineering and Technology | Digital Hardware & RTL Design Enthusiast | Aspiring R&D Engineer