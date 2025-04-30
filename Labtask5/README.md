# 🧪 Riphah International University - Lab 04
**Course**: *Computer Architecture*  
**Student**: [Abubakar Ahmad]  
**Lab Instructor**: Mr. Tabassum Javed  
**SAP-ID**: [54603]

---

## 📌 Lab Objectives

- Understand the concept of **bitwise logical operations** (`AND`, `OR`, `XOR`, `NAND`, `NOR`, `NOT`).
- Perform bitwise operations using **machine-level programming**.
- Modify the **machine instruction set** to support new logical instructions.
- Execute **microinstruction sequences** for each logical operation.
- Develop and test programs that apply these operations on user inputs.
- Analyze how logical operations affect **binary data processing** at the CPU level.

---

## 🔧 Tools Used

- **Computer System**: Standard desktop/laptop environment.
- **CPU Sim Simulator**: A tool used for simulating simple CPU architectures and debugging low-level programs.

---

## ⚙️ Key Concepts

### Bitwise Logical Operations

Bitwise operations are performed at the individual bit level and are essential for tasks such as:
- Data encryption/decryption
- Graphics programming
- Hardware register control
- Optimization in embedded systems

In this lab, we focus on implementing the following operations:
- **AND** – returns 1 only if both bits are 1
- **OR** – returns 1 if either bit is 1
- **XOR** – returns 1 if the bits are different
- **NAND** – NOT of AND
- **NOR** – NOT of OR
- **NOT** – inverts all bits

These operations were implemented using available features in the simulator.

---

## 🧠 Microinstruction Implementation

### AND (Bitwise AND)
- **Opcode**: `0`
- **Operation**: `AC ← AC ∧ DR` (Bitwise AND between Accumulator and Data Register)
- **Type**: Logical Instruction | Register & Memory Operation

Steps:
1. Navigate to the **Microinstructions Section** in CPU Sim.
2. Define a new **Logical Instruction**.
3. Set the Opcode and select the operation `AC ← AC ∧ DR`.

### OR (Bitwise OR)

This was implemented similarly by defining a new instruction with the operation: `AC ← AC ∨ DR`.

Other operations like XOR, NAND, NOR, and NOT can be simulated using combinations of base instructions and the `CMA` (Complement Accumulator) instruction.

---

## 🧪 Lab Tasks

### Task 1: Perform Bitwise AND Operation

#### ✅ Approach
1. Take **two input values from the user**.
2. Store one value in memory.
3. Apply the `AND` instruction between the two values.
4. Display the result.

#### 🧪 Execution & Output
- **Inputs**: e.g., `5`, `3`
- **Output**: `1`

This is due to binary comparison of:


---

### Task 2: Implement Other Logical Operations

The following operations were also implemented:
- **OR**
- **XOR**
- **NAND**
- **NOR**
- **NOT**

Each operation involved:
- Taking one or two inputs from the user.
- Applying appropriate machine instructions.
- Verifying correct output based on expected logic gate behavior.

---

## ⚠️ Challenges Faced

- Understanding how to define and integrate custom logical operations into the simulator.
- Mapping higher-level logical functions (like XOR/NAND) using basic CPU instructions.
- Debugging incorrect results caused by improper sequencing or misconfiguration of microinstructions.

---

## 🎯 Conclusion

Through this lab, I gained hands-on experience in:

- Performing **bitwise logical operations** at the machine level.
- Extending machine instruction sets with new logical capabilities.
- Simulating complex logical behavior using basic CPU operations.
- Deepening my understanding of how **binary data is processed** at the lowest hardware layer.

---
