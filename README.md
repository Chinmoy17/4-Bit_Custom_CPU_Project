# 4-Bit Custom CPU Design

This repository contains the design and implementation of a custom 4-bit CPU, created using fundamental logic gates (AND, OR, NOT). The CPU is tailored to meet specific requirements, including a 4-bit word size, basic ALU operations, limited registers, and an 8x15 SRAM. The project provides a functional demonstration of CPU components, including an Arithmetic Logic Unit (ALU), Control Unit, and memory design.

---

## **Project Highlights**

### **CPU Features**
- **Word Size**: 4 bits
- **ALU Operations**: 3 (XOR, Left Shift, ADD)
- **Number of Registers**: 3 (R0, R1, R2)
- **RAM Size**: 8 words, each 15 bits wide
- **Instruction Set**: 4 instructions, including ALU operations and jumps
- **Instruction Word Size**: 15 bits
- **ISA Formats**: ALU (Register Mode & Immediate Mode) and Jump Instructions

---

## **Instruction Set Architecture (ISA)**

### **ALU Instruction - Register Mode**
- **Opcode**: 4 bits
- **Register 1 (Ra)**: 2 bits (00 to 10)
- **Register 2 (Rb)**: 2 bits (00 to 10)
- **Unused**: 2 bits
- **Type of Instruction**: 2 bits
- **Operations**: 2 bits
  - **XOR (00)**  
  - **Left Shift (01)**  
  - **ADD (10)**  

### **ALU Instruction - Immediate Mode**
- **Opcode**: 4 bits
- **Register 1 (Ra)**: 2 bits
- **Immediate Value**: 5 bits (0000 to 1111)
- **Unused**: 4 bits
- **Type of Instruction**: 2 bits
- **Operations**: 2 bits

### **Jump Instructions**
- **Opcode**: 4 bits
- **Address**: 8 bits
- **Unused**: 3 bits
- **Type of Instruction**: 2 bits
- **Operations**: 2 bits
  - **JMP (00)**  
  - **JNZ (01)**  

---

## **Project Structure**

---

## **Diagrams**

### **1. Full CPU Diagram**
![Full CPU Diagram](diagrams/full_cpu_diagram.png)

---

### **2. Control Unit**
![Control Unit Diagram](diagrams/control_unit.png)

---

### **3. 8x15 SRAM**
![8x15 SRAM Diagram](diagrams/sram_8x15.png)

---

## **How to Use**
### **Prerequisites**
- Basic understanding of digital logic design
- Tools for circuit simulation (e.g., Logisim, Digital, or any custom logic simulator)
- Git for cloning the repository

### **Steps to Run**
1. Clone the repository:
   git clone https://github.com/yourusername/4-Bit_Custom_CPU_Project.git

2.Open the diagrams folder to explore the CPU design.
3.Use a circuit simulation tool to recreate and test the CPU functionality.
4.Customize the instruction set or components as needed for experimentation.

## **Key Components**
- **Arithmetic Logic Unit (ALU)**: Performs basic operations like XOR, left shift, and addition.
- **Control Unit**: Decodes instructions and manages CPU control signals.
- **8x15 SRAM**: Small RAM module designed to hold program instructions and data.

---

## **Future Enhancements**
- Add more registers to expand CPU capabilities.
- Increase RAM size to support larger programs.
- Implement additional ALU operations like subtraction and multiplication.
- Design a pipelined version for performance improvement.

---

## **Contributing**
Contributions are welcome! Feel free to fork this repository and submit pull requests for improvements or feature additions.

---

## **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## **Acknowledgments**
- Inspired by basic computer architecture principles.
- Designed and implemented as an academic exercise in CPU design.
