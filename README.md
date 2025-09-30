# Week 1: Introduction to RTL Design Flow.
 
The focus of this week is on **understanding the complete RTL design flow.**

---

## 📑 Objectives
- Day 1: Introduction to Verilog RTL Design and Synthesis.
- Day 2: Timing Libraries, Hierarchical vs Flat Synthesis, and Efficient Flip-Flop coding styles.
- Day 3: Combinational and Sequencial Optimizations.
- Day 4: Gate-Level Simulation (GLS), Blocking vs Non-Blocking in Verilog, and Synthesis-Simulation Mismatch.
- Day 5: Optimization in Synthesis.

---

## 📋 Prerequisites
- Basic understanding of Verilog codes.
- Basic understanding of Linux commands.
- Successful installation of the tools shown in [Week 0.](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-0.git)

---

## 📈 Proceedings
- Proceed to [Day 1](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/39ab28880dd3ad3f48bbed38bf4fd0e14b621c49/Day%201/README.md)
- Proceed to [Day 2](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/39ab28880dd3ad3f48bbed38bf4fd0e14b621c49/Day%202/README.md)
- Proceed to [Day 3](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/490086415cc2debc8c392e9c1e41805c871aac59/Day%203/README.md)
- Proceed to [Day 4](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/375e2128e691f2ef6fc6c438972b87ab7c131df6/Day%204/README.md)
- Proceed to [Day 5](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/main/Day%205/README.md)

---

## ⚠️ Challenges

- **Week 1**:
  * **Yosys shows Command Error**: While synthesizing the Verilog MUX design in Yosys, the synthesis completed successfully. However, executing the `show` command to generate the schematic diagram resulted in the error: `ModuleNotFoundError: No module named 'distutils'`. [Learn more.](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/main/Day%201/README.md#1-yosys-shows-command-error)

- **Week 5**:
  * **Syntax and Port Mismatch Errors in Testbench**: While simulating the Verilog design `partial_case_assign.v` using Iverilog, the testbench `tb_partial_case_assign.v` failed to compile and produced errors. [Learn more.](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/main/Day%205/README.md#1-syntax-and-port-mismatch-errors-in-testbench)
  * **Embedded images in Github not updating**: Updating errorneous images with correct images in the Github repository did not reflect in the README.md documentation. [Learn more](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/main/Day%205/README.md#2-embedded-images-in-github-not-updating)
  * **Doubt: Hierarchical Netlist and GLS Setup**: Doubt regarding the RTL Simulation, Yosys Synthesis and Gate Level Simulation when more than two RTL Design Verilog files are present. [Learn more.](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025---Week-1/blob/main/Day%205/README.md#3-doubt-hierarchical-netlist-and-gls-setup)

---

## 🏁 Final Remarks
The completion of Week 1 marks a significant step forward from merely setting up the environment to actually engaging with the foundations of digital design using Verilog and synthesis tools.
This week primarily focused on:<br>
- Gaining a working understanding of RTL design, testbenches, simulation, synthesis, and netlist generation.
- Exploring timing libraries, hierarchical vs. flattened synthesis, and flip-flop coding styles.
- Learning optimization techniques for both combinational and sequential logic.
- Performing Gate-Level Simulation (GLS) to detect and resolve synthesis-simulation mismatches.
- Strengthening concepts of control flow, such as if-else, case constructs, and looping mechanisms, while also identifying how incomplete constructs can cause inferred latches.<br>
Along the way, several challenges were encountered, ranging from tool-related issues like Yosys dependency errors, to debugging syntax and port mismatches in testbenches, to conceptual doubts about hierarchical synthesis and GLS setup. Each of these challenges provided valuable lessons in both practical debugging and theoretical clarity, reinforcing the importance of precision and attention to detail in digital design.<br>
By the end of this week, the progression from basic RTL coding to recognizing and addressing real-world synthesis issues highlights the essence of hardware design: it is as much about writing efficient code as it is about verifying, analyzing, and refining it.<br>
  


>[!IMPORTANT]
> For easy navigation to all the weeks of the program, please visit the [Master Repository](https://github.com/BitopanBaishya/VSD-Tapeout-Program-2025.git).
