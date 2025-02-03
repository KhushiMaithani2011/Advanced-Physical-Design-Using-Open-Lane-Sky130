# Advanced-Physical-Design-Using-Open-Lane-Sky130
Khushi Maithani

DAY 1 UNDERSTANDING OPEN SOURCE EDA, OPENLANE AND SKY 130

Arduino Board :
 
 ![A000062_00 front_934x700](https://github.com/user-attachments/assets/e7ae93af-e652-4a7b-9e04-0737c25fa0c6)   

 High Level View represented through a block diagram

 ![image](https://github.com/user-attachments/assets/cc0f9f97-76f5-4f52-a8e5-8e49fdf1e6ee)

 SoC - System on a Chip (Circled Component)
 A chip is inside a package. It is connected to pins or inputs and outputs.Its major components are-
 Chip (IC): The core functional unit containing electronic circuits for processing and logic operations.
 
 Pads: Metallic contact points on the silicon die, ensuring electrical connectivity.

 Core: The processing unit within the chip, containing logic gates, memory, and computational elements.
 
 Die: A single slice of a silicon wafer that holds the semiconductor circuits.

 IPs (Intellectual Property blocks): Pre-designed functional modules like CPU cores, memory blocks, and communication interfaces (SPI, I2C, USB, etc.).

![image](https://github.com/user-attachments/assets/24371bec-5d39-4a75-afe3-e94927b6d3c2)

 
 What is QFN-48?
 
 The Quad Flat No-Lead (QFN-48) package is a compact, surface-mount IC package with 48 pins. It is widely used for microcontrollers, RF devices, and power management ICs due to its 
 excellent thermal dissipation, low electrical parasitics, and cost-effectiveness.

Advantages of QFN-48:
✔️ Small form factor, ideal for compact devices.

✔️ Enhanced thermal and electrical performance with exposed pad design.

✔️ Low parasitic inductance, suitable for high-speed applications.

✔️ Cost-effective and easy to manufacture.

Schematic Representation :-

![image](https://github.com/user-attachments/assets/2dce7a99-742a-43d0-ad18-155e58e3b100)

![image](https://github.com/user-attachments/assets/053e84fd-1db5-49d0-b8c9-e239a55e0456)



Foundry : A semiconductor foundry is a company that manufactures chips on behalf of other companies, which may design the chips themselves but lack the facilities (fab) to actually produce them. Companies like TSMC (Taiwan Semiconductor Manufacturing Company) and Samsung are prominent foundries. They take in designs (often developed by fabless companies) and fabricate the physical chips.

IP (Intellectual Property): In the context of semiconductors, IP refers to pre-designed and pre-verified blocks of logic or circuitry that can be used in creating a chip. Examples include processor cores, memory controllers, and various other functional blocks. Companies like ARM or Imagination Technologies provide IP that others integrate into their own custom chip designs.


![image](https://github.com/user-attachments/assets/bcb44a87-cbc1-4bf2-8551-87eddda27c13)

Macros refer to pre-designed, reusable blocks of logic or circuits that perform specific functions. These macros can be components like:
Standard cells: Basic building blocks (such as logic gates, flip-flops, etc.) that are used in chip design.

Memory macros: Pre-designed memory blocks, such as SRAM, ROM, or DRAM, that can be integrated into a design without the need to design the memory from scratch.

Analog macros: Pre-designed analog circuits, like amplifiers or voltage regulators.

![image](https://github.com/user-attachments/assets/0ec85211-1704-411e-b611-d23314f51ab1)


RISC-V   (Reduced Instruction Set Computing - Five) is an open-source instruction set architecture (ISA) based on the principles of RISC. It defines a set of simple, efficient commands that a processor can execute. RISC-V is unique because it's open (publicly available for anyone to use) and modular (allowing customization based on the needs of different applications).


Key Features:
Open-source: Free to use and modify.

Modular Architecture: Supports various instruction set extensions (e.g., floating-point, vector processing).

Scalability: Suitable for devices ranging from microcontrollers to supercomputers.

Energy Efficiency: Optimized for low-power applications.

Customization: Enables custom processor designs without licensing restrictions.


Applications:

Embedded systems (IoT, microcontrollers).

AI and Machine Learning accelerators.

Data centers and cloud computing.

Automotive and industrial automation.

Custom hardware research and development.


From Software applications to Hardware


![image](https://github.com/user-attachments/assets/5b552e4f-0a4d-4336-a67d-615b4879e733)


![image](https://github.com/user-attachments/assets/bea0b3e2-f6b3-4bf8-bae8-ed416798775e)


For any application to run in a particular device, there is a certain flow which drives the process:

First, the application is fed to the system software or the Operation System whose output is small functions in C++, Java etc.
The output of the Operating System is taken up the COMPILER which converts it into specific instructions according to the chip present in the device. The syntax of this is dependent on the architecture of the hardware.
The output of the compiler is next given to the ASSEMBLER which converts those instructions to binary language.
Finally, this is given to the chip which does the specific functions based on the instructions given to it.

We need an RTL (Hardware Description Language) which understands the instruction and implements it. Then, this is synthesized into a netlist containing logic gates.


![image](https://github.com/user-attachments/assets/238b20db-9697-486b-8dc8-f0b0fc862b8d)


This is how the netlist looks like:

![image](https://github.com/user-attachments/assets/b70d6b62-cccc-4abe-9867-7d4ca1aa6353)








