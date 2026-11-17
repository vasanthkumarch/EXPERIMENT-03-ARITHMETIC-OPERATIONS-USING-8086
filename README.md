# EXPERIMENT 3 :8086 MICROPROCESSOR – BASIC ARITHMETIC OPERATIONS

## DATE: 17/11/2026
## NAME: sheikh hamza
## ROLL NUMBER: RA2511030010360
## DEPARTMENT: NWC

---

## AIM:

To write and execute 8086 Assembly Language programs to perform basic arithmetic operations such as Addition, Subtraction, Multiplication, and Division using an Online 8086 Emulator.

## SOFTWARE REQUIRED:

1. Computer or Laptop
2. Web Browser (Google Chrome / Microsoft Edge)
3. Online 8086 Emulator
4. Internet Connection

## THEORY:

### 8086 Microprocessor

The Intel 8086 is a 16-bit microprocessor developed by Intel. It has a 16-bit data bus and a 20-bit address bus, which allows it to access up to 1 MB of memory. It consists of an Execution Unit (EU) and a Bus Interface Unit (BIU).

The 8086 microprocessor supports various arithmetic and logical instructions to perform mathematical and logical operations.

### Technical Specifications of 8086:

| Specification | Description |
|---|---|
| Microprocessor | Intel 8086 |
| Architecture | 16-bit |
| Data Bus | 16-bit |
| Address Bus | 20-bit |
| Maximum Memory | 1 MB |
| Operating Modes | Minimum and Maximum |
| Registers | AX, BX, CX, DX, SI, DI, BP, SP |
| Instruction Set | Arithmetic, Logical, Data Transfer, Control Transfer |
| Clock Frequency | 5 MHz, 8 MHz or 10 MHz (depending on version) |

## 8086 REGISTER ORGANIZATION

The 8086 microprocessor contains general-purpose registers used for arithmetic and data manipulation.

- **AX (Accumulator):** Used for arithmetic and logical operations.
- **BX (Base Register):** Used for addressing and data storage.
- **CX (Count Register):** Used for loop and count operations.
- **DX (Data Register):** Used in multiplication and division operations.

## ARITHMETIC INSTRUCTIONS

| Instruction | Description |
|---|---|
| ADD | Adds two operands |
| SUB | Subtracts the second operand from the first |
| MUL | Performs unsigned multiplication |
| DIV | Performs unsigned division |
| MOV | Transfers data between registers |
| HLT | Stops program execution |

## PROCEDURE:

1. Open the Online 8086 Emulator.
2. Select the 8086 microprocessor environment.
3. Enter the required Assembly Language program.
4. Assemble or compile the program.
5. Check the program for errors.
6. Execute the program using the Run or Step option.
7. Observe the register values.
8. Verify the output for each arithmetic operation.

## ONLINE 8086 EMULATOR:

https://yjdoc2.github.io/8086-emulator-web/

## EXPERIMENT 1: ADDITION

### AIM:
To perform the addition of two 8-bit numbers using the 8086 microprocessor.

### PROGRAM:

MOV AL,05H
MOV BL,03H
ADD AL,BL
HLT

### EXPLANATION:

1. Load the first number 05H into AL.
2. Load the second number 03H into BL.
3. Perform addition using the ADD instruction.
4. The result is stored in AL.

### EXPECTED OUTPUT:

<img width="445" height="446" alt="image" src="https://github.com/user-attachments/assets/0fabc98f-86f0-498a-9456-900bd2f9a1b5" />


**Result:** 05H + 03H = 08H.

## EXPERIMENT 2: SUBTRACTION

### AIM:
To perform the subtraction of two 8-bit numbers using the 8086 microprocessor.

### PROGRAM:

MOV AL, 09H
MOV BL, 04H
SUB AL, BL
HLT

### EXPLANATION:

1. Load the first number 09H into AL.
2. Load the second number 04H into BL.
3. Perform subtraction using the SUB instruction.
4. The result is stored in AL.

### EXPECTED OUTPUT:

<img width="421" height="412" alt="image" src="https://github.com/user-attachments/assets/ba89ea1b-d43a-4070-ad9b-d8a78b89f05e" />


**Result:** 09H - 04H = 05H.

## EXPERIMENT 3: MULTIPLICATION

### AIM:
To perform the multiplication of two 8-bit unsigned numbers using the 8086 microprocessor.

### PROGRAM:

MOV AL, 05H
MOV BL, 04H
MUL BL
HLT

### EXPLANATION:

1. Load the first number 05H into AL.
2. Load the second number 04H into BL.
3. Perform multiplication using the MUL instruction.
4. The 16-bit result is stored in AX (AH:AL).

### EXPECTED OUTPUT:

<img width="416" height="396" alt="image" src="https://github.com/user-attachments/assets/c76ecd46-822e-485b-8b38-0b8921e80421" />


**Result:** 05H × 04H = 14H.

## EXPERIMENT 4: DIVISION

### AIM:
To perform the division of two 8-bit unsigned numbers using the 8086 microprocessor.

### PROGRAM:

```asm
MOV AX, 0014H
MOV BL, 04H
DIV BL
HLT
```

### EXPLANATION:

1. Load the dividend 0014H into AX.
2. Load the divisor 04H into BL.
3. Perform division using the DIV instruction.
4. The quotient is stored in AL.
5. The remainder is stored in AH.

### EXPECTED OUTPUT:

| Register | Value |
|---|---|
| AL | 05H |
| AH | 00H |

**Result:** 14H ÷ 04H = 05H, Remainder = 00H.

## OUTPUT OF SIMULATION:

### FIGURE-01: ADDITION OUTPUT

Upload the addition program execution screenshot here.

![Addition Output](img/addition.png)

### FIGURE-02: SUBTRACTION OUTPUT

Upload the subtraction program execution screenshot here.

![Subtraction Output](img/subtraction.png)

### FIGURE-03: MULTIPLICATION OUTPUT

Upload the multiplication program execution screenshot here.

![Multiplication Output](img/multiplication.png)

### FIGURE-04: DIVISION OUTPUT

Upload the division program execution screenshot here.

![Division Output](img/division.png)

## RESULT:

The 8086 Assembly Language programs for Addition, Subtraction, Multiplication, and Division were successfully written and executed using the Online 8086 Emulator. The results were verified by observing the corresponding register values.

## LEARNING OUTCOMES:

1. Understand the architecture and register organization of the 8086 microprocessor.
2. Learn basic arithmetic instructions in 8086 Assembly Language.
3. Understand the working of ADD, SUB, MUL, and DIV instructions.
4. Execute assembly programs using an online emulator.
5. Analyze the results stored in 8086 registers.

---

**Platform:** Online 8086 Emulator  
**Programming Language:** 8086 Assembly Language  
**Experiment:** Basic Arithmetic Operations
