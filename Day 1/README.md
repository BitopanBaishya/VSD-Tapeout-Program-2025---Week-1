# Day 1: Introduction to Verilog RTL Design & Synthesis.
 
The focus of today is 

---

## 📜 Table of Contents
[1. Introduction to RTL design, Design, Simulator and Test-Bench.](#1-introduction-to-rtl-design-design-simulator-and-test-bench)

---

## 1. Introduction to RTL design, Design, Simulator and Test-Bench.

**1. <ins>RTL Design**</ins>
   - **What is RTL design?**
     
     RTL (Register-Transfer Level) is a way of describing digital circuits at a high level. It focuses on:

     * **Registers (storage elements):** where data is stored (flip-flops).
     * **Transfers (data movement):** how data flows between registers.
     * **Logic (combinational circuits):** how data is processed between registers.

     RTL is written in hardware description languages like Verilog or VHDL. It is the bridge between circuit design and gate-level implementation.

   - **RTL vs other levels.**

     * **Behavioral level** → describes what the system should do, not how.
     * **RTL level** → describes how data moves and is stored on clock edges.
     * **Gate level** → actual logic gates and connections.
     * **Transistor level** → physical transistor circuits.

  - **RTL Design Flow**

     1. Write RTL code in Verilog (modules).
     2. Create testbench to verify functionality.
     3. Simulate RTL (using iverilog, gtkwave).

**2. <ins>Design (Verilog codes)</ins>**
   - **What is a Verilog Design?**
     
     A design file in Verilog is the main description of your hardware module. It defines:

     * Inputs and outputs of the circuit.
     * Logic that processes inputs to produce outputs.
     * Registers and wires used inside the design.

     Verilog design files represent the hardware RTL that will eventually be synthesized into real circuits.

   - **Structure of a Verilog Module.**

     Every design starts with a `module` and ends with `endmodule`.
     <br><br>
     Template:
  
     ```
      module <module_name> (
        <port declarations>
      );
      // internal signals
      // logic (combinational + sequential)
      endmodule

     ```
     Key parts:

     * **Module name** → unique identifier for your design.
     * **Ports** → inputs and outputs of the module.
     * **Internal logic** → wires, registers, assignments, `always` blocks.

**3. <ins>Simulator (Icarus Verilog)</ins>**
   - **What is a Simulator?**
     
     A simulator is a tool that allows you to run your Verilog design in a virtual environment to check if it behaves correctly.

     * **Purpose:** Verify functionality before hardware implementation.
     * **How:** It executes the Verilog code step by step with time, showing how signals change.

     A simulator evaluates the output(s), each time one or more input(s) is/are changed.

   - **Icarus Verilog (iverilog).**

     Icarus Verilog (iverilog) is a free, open-source Verilog simulator.
     <br>
     It is widely used for:
  
     * Compiling Verilog designs and testbenches.
     * Running simulations.
     * Generating output files in `.vcd` format.
<br>
     <img src="Images/Iverilog.png" alt="Alt Text" width="600"/>

**4. <ins>Testbench</ins>**
   - **What is a Testbench?**
     
     A testbench is a Verilog file used to verify a design module. It is not synthesizable (cannot be implemented in hardware). Instead, it:

     * Provides stimulus (inputs) to the design.
     * Observes and checks outputs.

     Think of it as a virtual laboratory where you test your hardware before building it.
<br>
     <img src="Images/Testbench.png" alt="Alt Text" width="600"/>

   - **Structure of a Testbench.**

     Unlike design modules, testbenches usually:
  
     * Have no ports (inputs/outputs).
     * Contain:
       * Register declarations for inputs.
       * Wire declarations for outputs.
       * Instantiation of the Design Under Test (DUT).
       * Stimulus (initial blocks, clocks).
