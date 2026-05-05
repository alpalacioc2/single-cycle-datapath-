#  Single-Cycle Datapath Processor (LEGv8 - Logisim)

##  Overview
This project implements a **single-cycle processor datapath** based on the LEGv8 (ARMv8) architecture using Logisim.

The processor executes each instruction in a single clock cycle and integrates all major CPU components including control logic, memory, and execution units.

---

##  Features
- Single-cycle execution model
- Supports arithmetic, logic, memory, and branch instructions
- Fully integrated datapath and control unit
- Instruction fetch, decode, execute, memory, and write-back in one cycle

---

##  Supported Instructions
- ADD – Register addition  
- SUB – Register subtraction  
- AND – Bitwise AND  
- ORR – Bitwise OR  
- LDUR – Load from memory  
- STUR – Store to memory  
- CBZ – Conditional branch (if zero)  
- B – Unconditional branch  

---

##  System Architecture

###  Core Components
- Program Counter (PC)
- Instruction Memory
- Control Unit
- Register File
- ALU
- Data Memory
- Multiplexers (MUXes)
- Sign Extend Unit
- Branch Logic

---

###  Datapath Flow
1. Fetch instruction from memory  
2. Decode opcode using Control Unit  
3. Read operands from Register File  
4. Execute operation using ALU  
5. Access memory if required  
6. Write result back to register  

---

###  Control Unit
- Generates control signals based on instruction opcode  
- Controls:
  - Register writes  
  - ALU operations  
  - Memory access  
  - Branch decisions  

---

###  Branch Logic
- Uses ALU Zero flag and control signals  
- Determines next PC:
  - Sequential (PC + 4)
  - Branch target address  

---

##  Testing
A test program was implemented including:
- Load/store operations  
- Arithmetic instructions  
- Conditional and unconditional branches  

The processor correctly executed all instructions and demonstrated proper datapath behavior.

---

##  Challenges
- Designing accurate control signals for each instruction  
- Debugging datapath connections and signal flow  
- Implementing correct branch behavior  

---

##  Key Takeaways
- Deep understanding of CPU architecture  
- Experience with datapath and control unit design  
- Insight into instruction execution at the hardware level  

---

##  Tools Used
- Logisim  
- Computer Architecture (LEGv8 concepts)  

---
