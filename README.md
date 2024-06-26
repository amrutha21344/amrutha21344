# VSDS QUARDRON MINI INTERNSHIP

Overview of VSDSquadron Mini Kit

TASK 1

TASK 2

TASK 3

TASK 4


# Description: 

The VSDQuadron Mini Internship offers a hands-on experience focused on developing and working with a state-of-the-art development board. This internship is designed for aspiring engineers and developers who are keen to delve into the world of embedded systems and hardware design. Participants will gain practical knowledge and experience in programming, interfacing, and utilizing various features of the VSDQuadron development board.

# Board Features:

**32-bit RISC-V Core:**

   The heart of the VSDQuadron development board is a powerful 32-bit RISC-V processor. This open-source instruction set architecture (ISA) is known for its flexibility and scalability, making it an excellent choice for educational and development purposes.
   
**Multiple Clock Options:**

   The board provides various clock configurations, allowing participants to explore different operational frequencies and power modes. This feature is crucial for optimizing performance and energy consumption in embedded applications.
15 GPIO Pins: The board is equipped with 15 General Purpose Input/Output (GPIO) pins. These versatile pins can be programmed for various functions, including digital input, digital output, and more. They are essential for interfacing with external sensors, actuators, and other peripherals.

# TASK 1

*Installing the required programmes for this internship, such as Ubuntu on VMBox, Visual C++, and writing an example of C code along with evaluating RISC assembly code for the sample C code, are the tasks at hand.*

Step 1. Virtual box Installed

![Virtual Box](https://github.com/amrutha21344/amrutha21344/assets/150883697/6e1471c9-9cb4-4dfc-8a1f-3fbdbe3ebe41)


Step 2. Ubuntu Installed

![UBUNTU](https://github.com/amrutha21344/amrutha21344/assets/150883697/139d657d-70e9-4021-8f56-37d44c586a1e)


Step 3. C code to execute The Sum of Numbers 1 to N

![C PROGRAM OF SUM OF NUMBERS](https://github.com/amrutha21344/amrutha21344/assets/150883697/b4c50b05-8cc2-44f7-b706-b3f78192046f)


Step 4. RISC-V Compiler Code Compilation

![RISC-V INSTRUCTION SET](https://github.com/amrutha21344/amrutha21344/assets/150883697/f52a6d4d-677a-41f2-b17d-46c13ff0dd15)


Step 5. Calculation RISC-V instruction

![WhatsApp Image 2024-06-26 at 13 12 19_947c88bc](https://github.com/amrutha21344/amrutha21344/assets/150883697/5a90ef85-27fe-4e41-8c79-33e23a040414)

***CONCLUSION***
# 



# Task 2

 # Project 1 - Ticket Terminal Designer: Developing an Automated Parking Ticket Vending Machine

Developing an automated parking ticket vending machine in C involves managing hardware interactions, user inputs, payment processing, and ticket dispensing. Below is a simplified example that covers basic functionalities using console inputs to simulate user interactions.

# Explanation

**Main Function:** Controls the flow of the program, interacting with users until the ticket is purchased.

**Global Variables:** total_collected keeps track of the amount inserted by the user, ticket_available indicates whether a ticket is available for purchase.

# Functions

**display_instructions():** Prints initial instructions to the user.

**accept_coin(float coin):** Accepts coins and updates total_collected.

**process_payment():** Checks if enough money has been collected to print a ticket.

**print_ticket():** Simulates printing a ticket after successful payment.

**cancel_transaction():** Cancels the transaction and resets total_collected.

# CODE

![Screenshot (212)](https://github.com/amrutha21344/amrutha21344/assets/150883697/9fdfbf9d-ea21-4ce8-a905-fd78aa7ea8a9)

# USER INPUTS

![Screenshot (213)](https://github.com/amrutha21344/amrutha21344/assets/150883697/fec63a5a-5743-4b0a-973f-aab252076c91)

# OUTPUT

![Screenshot (214)](https://github.com/amrutha21344/amrutha21344/assets/150883697/c7c399e3-342e-42a2-9156-2a03094572f6)

![Screenshot (215)](https://github.com/amrutha21344/amrutha21344/assets/150883697/16dc5209-c059-4a1f-b174-96d3c0580055)

![Screenshot (216)](https://github.com/amrutha21344/amrutha21344/assets/150883697/ff434bac-a7e5-4bad-a48a-38d65119eb5c)

 # Converting the C program to RISC-V instruction set

![Screenshot (218)](https://github.com/amrutha21344/amrutha21344/assets/150883697/34cf6ba4-2287-4c58-b262-00ae38831641)

![Screenshot 2024-06-26 161011](https://github.com/amrutha21344/amrutha21344/assets/150883697/4abeac22-0044-47ef-bc7a-2c115bac5f22)

***CONCLUSION***
# 

# Task 3

# SPIKE simulation and verification with -O1 and -OFast along with running the RISK-V Objdump

SPIKE Simulation

SPIKE is a RISC-V ISA Simulator, which can simulate RISC-V processors. It's often used for testing RISC-V software and running RISC-V assembly code. To simulate and verify your RISC-V design using SPIKE:

1. Compile your RISC-V program: Assume you have a RISC-V program written in assembly or C (which can be compiled to RISC-V assembly). Compile it with different optimization levels using a RISC-V cross-compiler. For example, if you have a program program.c, you might compile it with:
   
       riscv64-unknown-elf-gcc -O1 -march=rv64imafdc program.c -o program_O1.elf
       riscv64-unknown-elf-gcc -Ofast -march=rv64imafdc program.c -o program_Ofast.elf

![Screenshot 2024-06-28 122727](https://github.com/amrutha21344/amrutha21344/assets/150883697/b44e5907-25ca-4fe4-af12-e7e200e04833)


  Replace program.c with your actual program file name.

3. Run the simulation with SPIKE: SPIKE typically takes the ELF executable file generated by the RISC-V compiler and simulates its execution. To run your program with SPIKE:

       spike pk program_O1.elf
       spike pk program_Ofast.elf
   
![Screenshot 2024-06-28 123047](https://github.com/amrutha21344/amrutha21344/assets/150883697/9b48d63b-01bf-4eef-96a6-dc39412a24a7)


 Here, pk is the proxy kernel that SPIKE uses to run programs. Replace program_O1.elf and program_Ofast.elf with your actual executable names.

5. Observe and verify results: SPIKE will simulate the execution of your program with the specified optimization level (-O1 or -Ofast). You can observe the program’s output, performance, and behavior to verify correctness and performance differences between different optimization levels.

7. ![Screenshot 2024-06-28 123716](https://github.com/amrutha21344/amrutha21344/assets/150883697/8dd8bced-b9ad-468b-9865-85459ee09d95)


**Objdump Analysis**

Objdump is a utility that can display information about ELF files, including the assembly instructions. To analyze the assembly output:

1. Generate assembly code: Use objdump to generate assembly listings from your compiled ELF files:

       riscv64-unknown-elf-objdump -d program_O1.elf > program_O1.asm
       riscv64-unknown-elf-objdump -d program_Ofast.elf > program_Ofast.asm

      This will create program_O1.asm and program_Ofast.asm files containing the disassembled code for -O1 and -Ofast optimizations, respectively.

2. Compare assembly listings: Open these .asm files and compare the generated assembly code for the different optimization levels. Look for differences in instruction sequences, loop unrolling, function inlining, or other optimizations performed by the compiler.

3. Analyze performance implications: Understand how different optimization levels affect the size and efficiency of the generated code. -Ofast typically enables more aggressive optimizations compared to -O1, which can result in faster but potentially larger code.

![Screenshot 2024-06-28 124311](https://github.com/amrutha21344/amrutha21344/assets/150883697/b2b7efd5-bb72-48b3-8971-c3df2314606d)

***CONCLUSION***

# TASK 4


# Identify various RISC-V instruction type (R, I, S, B, U, J) and exact 32-bit instruction code in the instruction type format for below RISC-V instructions

let's break down the RISC-V instruction types (R, I, S, B, U, J) and provide the 32-bit instruction codes for each type:

# **R-Type (Register Type):**


Used for arithmetic and logic operations between registers.

Format: opcode rd rs1 rs2 funct3 rs2 funct7

Example instruction: add rd, rs1, rs2

Instruction Code Example:

add rd, rs1, rs2: 0000000 rs2 rs1 000 000 rd 0110011


# **I-Type (Immediate Type):**

Used for arithmetic and logical operations with an immediate value.

Format: opcode rd funct3 rs1 imm[11:0]

Example instruction: addi rd, rs1, immediate

Instruction Code Example:

addi rd, rs1, immediate: imm[11:0] rs1 000 rd 0010011


# **S-Type (Store Type):**

Used for storing a value from a register to memory.

Format: opcode imm[11:5] rs2 rs1 funct3 imm[4:0]

Example instruction: sw rs2, offset(rs1)

Instruction Code Example:

sw rs2, offset(rs1): imm[11:5] rs2 rs1 010 imm[4:0] 0100011


# **B-Type (Branch Type):**

Used for conditional branches based on comparison results.

Format: opcode imm[12|10:5] rs2 rs1 funct3 imm[4:1|11]

Example instruction: beq rs1, rs2, offset

Instruction Code Example:

beq rs1, rs2, offset: imm[12] imm[10:5] rs2 rs1 000 imm[4:1] imm[11] 1100011


# **U-Type (Upper Immediate Type):**

Used for setting the upper bits of a register with an immediate value.

Format: opcode rd imm[31:12]

Example instruction: lui rd, immediate

Instruction Code Example:

lui rd, immediate: imm[31:12] rd 0110111


# **J-Type (Jump Type):**

Used for unconditional jumps and procedure calls.

Format: opcode rd imm[20|10:1|11|19:12]

Example instruction: jal rd, offset

Instruction Code Example:

jal rd, offset: imm[20] imm[10:1] imm[11] imm[19:12] rd 1101111

These formats and examples cover the basic RISC-V instruction types and their corresponding 32-bit instruction codes. Each instruction type serves different purposes within the RISC-V instruction set architecture, allowing for efficient and versatile programming and execution.


ADD r1, r2, r3 *SUB r3, r1, r2 *AND r2, r1, r3 *OR r8, r2, r5 *XOR r8, r1, r4 *SLT r10, r2, r4 *ADDI r12, r3, 5 *SW r3, r1, 4 *SRL r16, r11, r2 *BNE r0, r1, 20 *BEQ r0, r0, 15 *LW r13, r11, 2 *SLL r15, r11, r2 Upload the 32-bit pattern***

**Here are the 32-bit instruction codes for each of the given RISC-V instructions:**

 **ADD r1, r2, r3:**  
 

     add r1, r2, r3: 0000000 00011 00010 000 00011 0110011

     Instruction Code: 0000000 00010 00001 000 00011 0110011 (hex: 0x00210033)

 **SUB r3, r1, r2:**
 

     sub r3, r1, r2: 0100000 00011 00001 000 00010 0110011

     Instruction Code: 0100000 00001 00011 000 00010 0110011 (hex: 0x00118033)

**AND r2, r1, r3:**


    and r2, r1, r3: 0000000 00010 00001 111 00011 0110011

    Instruction Code: 0000000 00011 00010 111 00001 0110011 (hex: 0x00311033)

 **OR r8, r2, r5:**
 

    or r8, r2, r5: 0000000 01000 00010 110 00101 0110011

    Instruction Code: 0000000 00101 01000 110 00010 0110011 (hex: 0x28502133)

 **XOR r8, r1, r4:**


    xor r8, r1, r4: 0000000 01000 00001 100 00100 0110011

    Instruction Code: 0000000 00100 01000 100 00001 0110011 (hex: 0x24408133)

 **SLT r10, r2, r4:**
 

    slt r10, r2, r4: 0000000 01010 00010 010 00100 0110011

    Instruction Code: 0000000 00100 01010 010 00010 0110011 (hex: 0x2520A133)

 **ADDI r12, r3, 5:**


    addi r12, r3, 5: 0000010 01100 00011 000 00001 0010011

    Instruction Code: 0000010 00001 01100 000 00011 0010011 (hex: 0x00130013)


 **SW r3, r1, 4:**


    sw r3, 4(r1): 0000010 00011 00001 010 00000 0100011

    Instruction Code: 0000010 01000 00011 010 00001 0100011 (hex: 0x08418303)

 **SRL r16, r11, r2:**


    srl r16, r11, r2: 0000000 10000 01011 101 00010 0110011

    Instruction Code: 0000000 00010 10000 101 01011 0110011 (hex: 0x1250A033)

 **BNE r0, r1, 20:**


    bne r0, r1, 20: 0001011 00000 00001 001 10100 1100011

    Instruction Code: 0001011 10100 00000 001 00001 1100011 (hex: 0xB0406E63)

 **BEQ r0, r0, 15:**


    beq r0, r0, 15: 0001000 00000 00000 000 01111 1100011

    Instruction Code: 0001000 01111 00000 000 00000 1100011 (hex: 0x0800F063)

 **LW r13, r11, 2:**


    lw r13, 2(r11): 0000011 01101 01011 010 00010 0000011

    Instruction Code: 0000011 00010 01101 010 01011 0000011 (hex: 0x1A56A303)

 **SLL r15, r11, r2:**


    sll r15, r11, r2: 0000000 01111 01011 001 00010 0110011

    Instruction Code: 0000000 00010 01111 001 01011 0110011 (hex: 0x02B1A033)

These codes represent the 32-bit binary encodings (in hexadecimal) for each of the specified RISC-V instructions, following the respective instruction formats for R, I, S, B, U, and J types.













