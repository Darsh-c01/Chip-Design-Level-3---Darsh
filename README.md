# Chip-Design-Level-3-Darsh
## <ins>Basics of a chip</ins>
![image](https://github.com/user-attachments/assets/a31b1591-51ee-4627-81c8-64287c3e60a1)  
This is a package with a chip in the centre and represents how the pins in the package are connected to the chip. 
![image](https://github.com/user-attachments/assets/dbccbe88-435e-4080-97a6-4d3507455e9d) 
This is essentially how a chip is from the inside  
>Some important terminologies here are: \
1.Pads: They are basically like doors which help the core send and recive signals \
2.Core: This is the part where all the logic gates are and the main processing happens 

![image](https://github.com/user-attachments/assets/a9eb95ff-ecbf-4e1d-b452-3f09c29cb087) 
This is a representation of the core of the chip  
>Foundry IPs: \
 Foundy is basically the place where a chip is manufactures \
 IP = Intelectual Property

## Introduciton to RISCV
It is a instruction set architecture(ISA). \
We first write the specifications in a language like C whis is then converted to the assembly level language , which in turn is converted to an RTL.

### <ins>Flow from a app to the chip:(software to hardware) </ins>
![image](https://github.com/user-attachments/assets/abee7640-7367-4a00-9348-ddc399b5f0f7)
>The steps involved in this process are:
> 1. The input coming form the os is usually in one of the languages mentioned above 
> 2. Now what the compiler does is , it converts these into a set of instructions whose syntax is subjective to the hardware being used , for example a RISC-V hardware or a intel hardware will have a difference in the instructions 
> 3. After this , these instructions are then converted into binary by the assembler which then transfers it to the chip.

![image](https://github.com/user-attachments/assets/aad0f6b8-6e0c-4bb9-bfe5-a8f534299989)
The instuction set which is the output of the compiler is basically a abstract interface between the software and the hardware OR it is the "architecture of the computer" 

## The flow for a chip to be designed:
![image](https://github.com/user-attachments/assets/07532fbf-792e-4505-ae5a-5967f3c3efdf)

What essentially happens here is that the output of the assembler is converted to RTL which is then converted into a netlist , followed by a physical implementation of it.

## <ins>Digital ASIC design</ins>

ASIC stands for : Aplication Specific Integrated Cirucit , which as the name suggest is designed to execute a specific function and not multiple functions \
For us to design a ASIC chip we need the following: 
![image](https://github.com/user-attachments/assets/761e5784-e6e8-4566-ac73-085ea6d3d72a)

>The full forms of the above are:\
>RTL = Register Transfer Level\
>EDA = Electronic Design Automation\
>PDK = Process Design Kits (It is the interface between the Fab and the Designer)

### <ins> Steps in ASIC Design / flow </ins>
>1.Specification\
>2.Architecture Design\
>3.RTL\
>4.RTL to Netlist conversion\
>5.Floor Planning\
>6.Placement and Routing\
>7.Physical Verification\
>8.Timing Analysis (Clock tree analysis)\
>9.Simulation\
>10.Final Verification\
>11.TapeOut











