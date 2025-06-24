
A modular, hierarchical **4-bit ALU** designed using **Logisim**, divided into two subcircuits:
- `AU`: Arithmetic Unit (handles add, subtract, carry, overflow)
- `LU`: Logic Unit (handles AND, OR, NOT, XOR, etc.)

## 🚀 Features

- 4-bit operands `A` and `B`
- 4-bit `OPCODE` for selecting operations
- Modular design: separate `AU` and `LU` subcircuits
- Flags generated:
  - `Z` – Zero
  - `N` – Negative (MSB = 1)
  - `C` – Carry
  - `Overflow` – Signed overflow

## 🧠 Supported Operations

| OPCODE (Binary) | Operation   | Description              |
|-----------------|-------------|--------------------------|
| 0000            | A + B       | Unsigned Addition        |
| 0001            | A - B       | Unsigned Subtraction     |
| 0010            | A & B       | Bitwise AND              |
| 0011            | A \| B      | Bitwise OR               |
| 0100            | A ^ B       | Bitwise XOR              |
| 0101            | ~A          | Bitwise NOT (A only)     |
| 0110 - 1111     | (Reserved)  | Extendable up to 16 ops  |

> ✳️ You can easily add more operations by extending the decoder and mux logic.

## 🧪 Simulation

- Use **Poke Tool** 🖐 to toggle bits for A, B, and OPCODE
- Observe output `Y` and flags (`Z`, `N`, `C`, `Overflow`)
- Enable simulation via `Simulate > Simulation Enabled`

## 📂 Files Included

- `alu.circ` – Logisim project file
- `README.md` – This file
- `/screenshots/` – Images of circuit layout

## 🧠 Skills Demonstrated

- Digital design using multiplexers, adders, and logic gates
- Hierarchical circuit structuring in Logisim
- OPCODE-controlled ALU logic
- Simulation and debugging using probe and poke tools

## 👨‍💻 Author

**Saswat Padhy**  
B.Tech, IIT Kharagpur  
[GitHub Profile Link]  
