As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.

Veriog code is being executed and the waveforms are generated using the gtkwave

Aim: To verify the Functional Simulation

Table of contents

1.RISC-V RV32I
2.BLOCK DIAGRAM OF RISC-V RV32I
3.INSTRUCTION SET OF RISC-V RV32I
4.FUNCTIONAL SIMULATION
4.1 About iverilog and gtkwave
4.2 Installing iverilog and gtkwave
4.3 The output waveform

1. RISC-V RV32I
This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

2. BLOCK DIAGRAM OF RISC-V RV32I
   ![image](https://github.com/Mamthag17/lib-/assets/161347200/16bd8c07-0e8a-43fc-a618-0193f7ce6ebb)

3. INSTRUCTION SET OF RISC-V RV32I
   ![image](https://github.com/Mamthag17/lib-/assets/161347200/4444f5d7-5a9c-4728-bab1-dae48d438644)
   ![image](https://github.com/Mamthag17/lib-/assets/161347200/056463fb-5584-47bf-841e-4eb877417419)

4. FUNCTIONAL SIMULATION

4.1 About iverilog and gtkwave
Icarus Verilog is an implementation of the Verilog hardware description language.
GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.

4.2 Installing iverilog and gtkwave
For Ubuntu
Open your terminal and type the following to install iverilog and GTKWave

$   sudo apt get update
$   sudo apt get install iverilog gtkwave
![image](https://github.com/Mamthag17/lib-/assets/161347200/7a4467bf-84b4-4ab0-83e5-ac6bdadfa2fb)
To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.
git clone https://github.com/Mamthag17/lib-
cd lib-
![image](https://github.com/Mamthag17/lib-/assets/161347200/1e4c8790-5eb7-4a26-a3f8-c711d957b6ba)
To simulate and run the Verilog code, enter the following commands in your terminal.
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
![image](https://github.com/Mamthag17/lib-/assets/161347200/9fd7b1f7-1490-4c4b-91f3-3276411ba582)
To see the output waveform in gtkwave, enter the following commands in your terminal.
$ gtkwave hello.vcd
![image](https://github.com/Mamthag17/lib-/assets/161347200/22175cb2-3b80-4426-8b57-15fb1d456f22)
4.3 The output waveform
The output waveform showing the instructions performed in a 5-stage pipelined architecture.
Instruction 1:add r6,r2,r1
![image](https://github.com/Mamthag17/lib-/assets/161347200/66b93205-9d42-4a87-a3fd-3f4d86f58c85)
Instruction 2:sub r7,r1,r2
![image](https://github.com/Mamthag17/lib-/assets/161347200/9a17d924-61b0-4697-9bd4-f9cd5ca072fa)
Instruction 3:and r8,r1,r3 
![image](https://github.com/Mamthag17/lib-/assets/161347200/b2cca211-3956-4293-83f0-de456efc598c)
Instruction 4:or r9,r2,r5
![image](https://github.com/Mamthag17/lib-/assets/161347200/1a1a31b5-70a0-4cca-a2e0-f0c55060d750)
Instruction 5:xor r10,r1,r4
![image](https://github.com/Mamthag17/lib-/assets/161347200/3530cf70-386f-46ff-a131-c51f0e360a16)
Instruction 6:slt r11,r2,r4
![image](https://github.com/Mamthag17/lib-/assets/161347200/bbef6d6f-79a5-4ad2-9acb-05b27cd32363)
Instruction 7:addi r12,r4,5
![image](https://github.com/Mamthag17/lib-/assets/161347200/465e0f6e-0505-4712-a6a8-b3777e7aa2c6)
Instruction 8:sw r3,r1,2 
![image](https://github.com/Mamthag17/lib-/assets/161347200/e3e9a52e-4bf8-4d8f-9e08-22c588014e46)
Instruction 9:lw r13,r1,2 
![image](https://github.com/Mamthag17/lib-/assets/161347200/8023eafc-73ab-420c-9ac1-4b7ae612457a)
Instruction 10:beq r0,r0,15
![image](https://github.com/Mamthag17/lib-/assets/161347200/7aba7c13-127c-45e5-acd9-9b82522df93f)
After branching, performing Instruction 11:add r14,r2,r2
![image](https://github.com/Mamthag17/lib-/assets/161347200/3c7c5199-901f-40d2-8118-79022cfb8c41)
Full 5-stage instruction pipeline and pc-increment description Waveform
![image](https://github.com/Mamthag17/lib-/assets/161347200/16208cd1-cdf2-42ca-a6df-6edca82dfc42)
![image](https://github.com/Mamthag17/lib-/assets/161347200/9894596f-5930-4aca-87bc-d0890fb179c4)
![image](https://github.com/Mamthag17/lib-/assets/161347200/6e8bdc6a-bdd1-4449-abb5-567d519a2aee)
















