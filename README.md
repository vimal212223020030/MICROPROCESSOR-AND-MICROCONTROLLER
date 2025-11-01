# MICROPROCESSOR-AND-MICROCONTROLLER
## 15. Write an assembly language program in 8051 to exchange the contents of two memory blocks of equal length
## Aim
To develop an 8051 Assembly Language program that generates the contents of two memory blocks of equal length. and stores them in RAM.

## Apparatus Required

1. 8051 Microcontroller or Emulator (e.g., Keil uVision)
2. PC/Laptop with Windows/macOS/Linux
3. Text editor or IDE to write and assemble 8051 assembly code
4. Basic knowledge of 8051 instructions and registers
## Algorithm

1. Initialize pointers (RO, R1) to point to the start of the two memory blocks.
2. Load a counter (R2) with the length of the blocks
3. Repeat until the counter is zero:
4. Generate or copy content to memory block 1.
5. Generate or copy content to memary block 2.
6. Increment memory pointers..
7. Decrement counter
8. End program when all memory locations are filled.

## Program

ORG OCH SJMP 30H ORG 30H MOV RO, #30H MOV R1, #40H MOV R2,#OSH LOOP: MOV A, GRO XCH A, ER1 MOV @RO, A INC RO INC R1 DINZ R2, LOOP HERE SIMP HERE END

## OUTPUT
![WhatsApp Image 2025-11-01 at 09 11 59_e5ed9c96](https://github.com/user-attachments/assets/65e1e5f1-5a99-4006-aae8-0fd56427653b)
![WhatsApp Image 2025-11-01 at 09 12 31_100ae27c](https://github.com/user-attachments/assets/8832dec2-0fef-48b4-b3ee-95dcb410a20d)
![WhatsApp Image 2025-11-01 at 09 13 08_3d5be6d2](https://github.com/user-attachments/assets/a3dc43b3-3b83-4349-9afd-05492751b9d5)
![WhatsApp Image 2025-11-01 at 09 13 35_996a935f](https://github.com/user-attachments/assets/9a68be0f-274d-4dbe-9acb-d5a8f3a28489)

## Result
The program successfully generates the contents of two memory blocks of equal length and stores them in RAM.
