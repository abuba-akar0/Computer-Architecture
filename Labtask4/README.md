# 🧪 Riphah International University - Lab 04
**Course**: *Computer Architecture*  
**Student**: [Abubakar Ahmad]  
**Lab Instructor**: Mr. Tabassum Javed  
**SAP-ID**: [54603]

---

## 📌 Lab Objectives

- Understand the concept of **bitwise logical operations** (`AND`, `OR`, `NOT`, `XOR`, `NAND`, `NOR`).
- Implement bitwise operations using **machine-level programming**.
- Modify the **machine instruction set** to support new logical instructions.
- Execute **microinstruction sequences** for each logical operation.
- Design and test assembly programs that perform bitwise logic on two input values.
- Analyze how logical operations affect binary data processing at the CPU level.

---

## 🔧 Tools Used

- **Computer System**: Standard desktop/laptop environment.
- **CPU Sim Simulator**: A tool used for simulating simple CPU architectures, helping understand processor design, instruction execution, and debugging.

---

## ⚙️ Microinstruction Implementation

### AND (Bitwise AND)
- **Opcode**: `0`
- **Operation**: `AC ← AC ∧ DR` (Bitwise AND between Accumulator and Data Register)
- **Type**: Logical Instruction | Register & Memory Operation

Steps:
1. Navigate to the **Microinstructions Section** in CPU Sim.
2. Define a new **Logical Instruction**.
3. Set the Opcode and select the operation `AC ← AC ∧ DR`.

### OR (Bitwise OR)
- You can implement this similarly by defining a new instruction with the operation: `AC ← AC ∨ DR`.

Other operations like `XOR`, `NAND`, `NOR`, and `NOT` can be simulated using combinations of `AND`, `OR`, and `CMA` (Complement Accumulator).

---

## 🧪 Lab Tasks

### Task 1: Perform Bitwise AND Operation

#### ✅ Approach
1. Take **two inputs from the user**.
2. Store one input in memory.
3. Use the `AND` instruction to compute the result.
4. Output the final value.

#### 🧪 Execution & Output
- **Inputs**: e.g., `5`, `3`
- **Output**: `1`

This is due to the binary operation:  


---

### Task 2: Implement Other Logical Operations

You are required to implement the following operations:
- **OR**
- **XOR**
- **NAND**
- **NOR**
- **NOT**

Each operation must:
- Accept one or two user inputs.
- Use or simulate appropriate machine instructions.
- Output the correct result based on the selected logic gate.

---

## ⚠️ Challenges Faced

- Understanding how to define and integrate custom logical operations into the simulator.
- Mapping higher-level logical operations (like XOR/NAND) using available base instructions.
- Debugging incorrect results caused by improper sequencing of bitwise instructions.

---

## 🎯 Conclusion

Through this lab, I gained hands-on experience in:

- Performing **bitwise logical operations** at the machine level.
- Extending machine instruction sets with new logical capabilities.
- Simulating complex logical behavior using basic CPU operations.
- Deepening my understanding of how **binary data is processed** at the lowest hardware layer.

---
