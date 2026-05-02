# Multi-Cycle Risc-V Processor

## 📘 Overview
This project implements a **multi-cycle computer processor architecture** with a custom instruction set.  
The design executes instructions across multiple clock cycles to improve hardware efficiency and reduce datapath complexity.

The processor uses an **accumulator-based architecture** to simplify arithmetic and logical operations while minimizing unnecessary data transfers.

---

## 🏗 Architecture

**Key Specifications:**

- **Word Size:** 16-bit  
- **Memory:** 16K × 4 bits  
- **Processor Type:** Multi-cycle, register-based  
- **Core Component:** Accumulator  
- **Execution Model:** Multi-stage instruction execution  

---

## ⚙️ ALU Operations

The Arithmetic Logic Unit (ALU) supports:

- **Addition**
- **Subtraction**
- **Logical AND**
- **Logical OR**
- **Logical NOT**
- **Pass / Data Transfer**

---

## 🧩 Instruction Set

The processor supports **four instruction types**:

### 🔹 Type A — Memory & Jump Instructions
- `Load`
- `Store`
- `Jump`

### 🔹 Type B — Conditional Branch
- `BranchZ`

### 🔹 Type C — Register & ALU Operations
- `MoveTo`
- `MoveFrom`
- `Add`
- `Sub`
- `And`
- `Or`
- `Not`
- `Nop`

### 🔹 Type D — Immediate Operations
- `Addi`
- `Subi`
- `Andi`
- `Ori`

---

## 🔄 Execution Cycle

Each instruction is executed in multiple stages:

1. **Instruction Fetch**
2. **Instruction Decode**
3. **Execute**
4. **Memory Access** (if required)
5. **Write Back**

This multi-cycle design allows hardware components to be reused efficiently across stages.

---

## 🎯 Project Goals

- Design a custom **multi-cycle CPU architecture**
- Implement structured **instruction formats**
- Generate appropriate **control signals**
- Organize a functional **datapath**
- Demonstrate instruction execution flow

---

## 🚀 Future Improvements

- Implement in **Verilog / VHDL**
- Add a **simulation environment**
- Extend the **instruction set**
- Introduce **pipelining**
- Add debugging tools

---

## 👤 Author

Computer Architecture Project
