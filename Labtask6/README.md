# 🧪 Riphah International University - Lab 07
**Course**: *Computer Architecture*  
**Student**: [Abubakar Ahmad]  
**Lab Instructor**: Mr. Tabassum Javed  
**SAP-ID**: [54603]

---

## 📌 Lab Objectives

- Understand the functionality of control and status instructions:  
  `SPA` (Skip if Positive), `SNA` (Skip if Negative), `CMA` (Complement Accumulator), and `CLA` (Clear Accumulator).
- Implement these instructions using **machine-level programming**.
- Use conditional skip operations to control **program flow**.
- Observe how sign-based conditions affect instruction execution.
- Gain hands-on experience with **status flags** and **conditional branching** at the machine level.

---

## 🔧 Tools Used

- **Computer System**: Standard desktop/laptop environment.
- **CPU Sim Simulator**: A tool used for simulating simple CPU architectures and debugging low-level programs.

---

## ⚙️ Key Concepts

### SPA (Skip if Positive)
- Skips the next instruction if the value in the **Accumulator (AC)** is **positive** (i.e., the most significant bit is `0`).

### SNA (Skip if Negative)
- Skips the next instruction if the value in the **Accumulator (AC)** is **negative** (i.e., the most significant bit is `1`).

### CMA (Complement Accumulator)
- Inverts all bits of the Accumulator (`AC ← AC'`).
- Used for logical NOT operations and preparing values for Two’s Complement arithmetic.

### CLA (Clear Accumulator)
- Sets the Accumulator value to `0`.
- Useful for resetting values before new operations.

These instructions are crucial for implementing **conditional logic** without high-level constructs.

---

## 🧠 Microinstruction Implementation

### CMA (Complement Accumulator)

- **Opcode**: `E200`
- **Operation**: `AC ← AC'` (Bitwise NOT on Accumulator)
- **Type**: Logical Instruction

Steps:
1. Go to the **Microinstructions Section** in CPU Sim.
2. Define a new instruction.
3. Select **Logical Operation** and choose `AC ← AC'`.

### SPA / SNA

These instructions do not require explicit opcode definitions but are implemented by checking the **sign bit** of the Accumulator and conditionally incrementing the Program Counter (PC) if the condition is met.

- **SPA**: Skip next instruction if AC > 0
- **SNA**: Skip next instruction if AC < 0

They allow for **branching logic** based on the result of previous computations.

---

## 🧪 Lab Tasks

### Task 1: Implement Control Flow Based on Sign Detection

#### ✅ Approach
1. Take an input from the user.
2. Store it in memory and load it back into the accumulator.
3. Use `SPA` to check if the number is positive.
4. If positive, jump to a message indicating positivity.
5. Otherwise, use `SNA` to detect negativity or zero and display appropriate messages.

This demonstrates how conditional skips can be used to simulate **if-else logic** at the machine level.

---

## ⚠️ Challenges Faced

- Understanding how sign detection works at the hardware level.
- Debugging incorrect program flow caused by misinterpretation of the sign bit.
- Configuring the simulator to correctly interpret and execute conditional skips like `SPA` and `SNA`.

---

## 🎯 Conclusion

Through this lab, I gained valuable experience in:

- Controlling program flow using **status-based skip instructions** like `SPA` and `SNA`.
- Performing bitwise manipulation using `CMA` and clearing registers using `CLA`.
- Translating **high-level logic** such as decision-making into **low-level machine instructions**.
- Deepening my understanding of how CPUs evaluate signs and manage execution paths.

