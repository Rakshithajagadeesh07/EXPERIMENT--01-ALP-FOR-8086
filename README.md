# EXPERIMENT--01-ALP-FOR-8086
Name : Rakshitha J

Roll no : 212223240135

Date of experiment : 13-08-2024


## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,

8.	 
![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)

9.	Click on emulate to start emulation 


![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)


10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 

![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
org 100h
MOV al,11h;
MOV bl,20h;
ADD al,bl;
MOV [6379h],al;
ret
```

## Output  
![image](https://github.com/user-attachments/assets/03796bc1-e98b-4a41-a675-b49dd015723f)

## Subtraction   of 8 bit numbers  ALP 
```
org 100h
MOV al,20h;
MOV bl,[8778h];
SUB bl,al;
MOV [8798h],bl;
ret
```
 
## Output  
![image](https://github.com/user-attachments/assets/ae4a6573-e547-4976-96d3-2e36ddca61bf)

## Multiplication alp 
```
org 100h
 MOV al,13h;
 MOV bl,2h;
 MUL bl;
 MOV [6063h],bl;
 ret
```

 ## Output 
![image](https://github.com/user-attachments/assets/e43acfb7-6062-4d90-b19c-5931977ba7af)

## Division alp 

```
org 100h
 MOV al,26h;
 MOV bl,[2369h];
 DIV bl;
 MOV [2399h],al;
 ret
```

## OUTPUT
![image](https://github.com/user-attachments/assets/a89100cd-0421-47fe-b3a5-8984bfc2ac3c)

## Programs For Logical Operators:
## AND
```
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
## Output  
![image](https://github.com/user-attachments/assets/79c30438-5641-4ae7-9bd9-23052c417b40)

## OR:
```
MOV SI,0532H;
MOV AX,0A32H;
MOV BX,0B13H;
OR AX,BX;
```
## Output
![image](https://github.com/user-attachments/assets/2ff8b79c-b9ed-4a65-9a1c-23f572799b73)

## NOT:
```
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```
## Output
![image](https://github.com/user-attachments/assets/cc26d576-d21f-44e1-ae66-325a2d276c62)

## XOR:
```
MOV [SI+2],AX;
MOV AX,0A32H;
MOV BX,0B13H;
XOR AX,BX;
```
## Output:
![image](https://github.com/user-attachments/assets/46ab283f-7fa4-464c-82d3-4d154388fafa)

## Result : 
Thus, to write and execute ALP on fundamental arithmetic operations and Logical operations is successful.
