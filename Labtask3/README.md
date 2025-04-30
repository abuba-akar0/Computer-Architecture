# 🧪 Computer Architecture - Lab Task 03
**Course**: *Computer Architecture*  
**Student**: *Abubakar Ahmad*

**SAP-ID**: *54603*

**Lab Instructor**: *Mr. Tabassum Javed*  


---

## 📌 Lab Objectives

- Understand **Two’s Complement** for subtraction in binary arithmetic.
- Perform subtraction using bitwise operations: `CMA` (Complement Accumulator) and `INC` (Increment Accumulator).
- Analyze step-by-step execution of subtraction in assembly language.
- Apply low-level programming techniques to solve arithmetic expressions.
- Design machine instructions that simulate high-level behavior.

---

## 🔧 Tools Used

- **CPU Sim Simulator**: A simulation tool used to understand CPU architecture, instruction sets, and program execution.
- **Custom Instruction Set**: Extended with new operations (`CMA`, `INC`) to support Two’s Complement subtraction.

---

## ⚙️ Microinstruction Implementation

### CMA (Complement Accumulator)
- **Opcode**: `E200`
- **Operation**: `AC ← AC'` (Bitwise NOT on Accumulator)
- **Type**: Register Instruction | Logical Operation
- **Purpose**: Invert bits for Two’s Complement preparation.

### INC (Increment Accumulator)
- **Opcode**: `E020`
- **Operation**: `AC ← AC + 1`
- **Type**: Register Instruction | Arithmetic Operation
- **Purpose**: Add 1 to complete the Two’s Complement process and get the negative value.

These instructions were added to the microinstruction set in the simulator.

---

## 🧪 Lab Tasks

### Task 1: Implement Machine Instructions to Solve `3 + 5 – 2 + 1`

#### ✅ Approach

1. Take **first two values from the user**.
2. **Hardcode** the remaining values (`2` and `1`).
3. Use `CMA` and `INC` to perform Two’s Complement subtraction.
4. Combine results using addition operations to solve the full expression.

#### 🧪 Execution & Output

- **Inputs**: `3` and `5`
- **Output**: `-1`

This result was achieved by simulating the logic using CPU Sim and verifying each step of the operation.

---

## ⚠️ Challenges Faced

- Understanding how to correctly implement `CMA` and `INC` for subtraction.
- Mapping logical steps into machine-level instructions supported by the simulator.
- Debugging improper sequencing of operations during execution.

---

## 🎯 Conclusion

This lab provided valuable insight into:

- Performing **subtraction at the bit level** using Two’s Complement.
- Extending existing instruction sets with custom operations.
- Writing and executing **machine-level assembly** to simulate complex operations.
- Understanding how **high-level arithmetic** maps to **low-level CPU instructions**.

