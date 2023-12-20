# risc-Assembler-and-Simulator
This repository contains a Python implementation of a simple assembler and simulator for a particular Instruction Set Architecture, integrated with automated testing routines. The project was developed for the [Computer Organization](https://techtree.iiitd.edu.in/viewDescription/filename?=CSE112) course at IIIT Delhi in Winter 2023.

📂 **Folder Structure:**
- `/Simple-Assembler`: Contains the source code for the assembler (assembler.py)
- `/SimpleSimulator`: Contains the source code for the simulator (simulator.py)
- `/automatedTesting`: Automated test suite for ensuring code correctness.

📋 **Usage:** <br>
Follow these steps to use the assembler and simulator: <br>
Make sure that 'assembler.py' file (Assembler code) is in the `/Simple-Assembler` directory.<br>
Make sure that 'simulator.py' file (Simulator code) is in the `/SimpleSimulator` directory.<br>
Navigate to the `/automatedTesting` folder. <br>
To run the Assembler: <pre><code>./run --no-sim</code></pre> 
To run the Simulator: <pre><code>./run --no-asm</code></pre> 
To run both: <pre><code>./run</code></pre>

🛠️ **Features** <br>
- Assembler: Converts assembly code into machine code for the specified [ISA](https://github.com/shobhitraj1/risc-Assembler-and-Simulator/blob/25c5e0a595713494cf1de1e57eb046e7f70ae93f/CO_project%20_2023.pdf). The program is able to handle all the supported instructions of the ISA, labels & variables. The assembler reads the assembly program as an input text file using sys.stdin and prints the binary format of the respective instructions if the assembly program is error free. <br>
- Simulator: Reads the machine code & execute the instructions. It is able to handle several operations, computations & check for overflows. The simulator reads the binary file as an input text file using sys.stdin and prints the program counter & register values after each execution of instruction & also the entire "memory dump" at the end. <br>
- Automated Testing: Includes a suite of automated tests to ensure the correctness and reliability of the assembler and simulator. <br>
- Floating Point Computation: The assembler & simulator are also capable of handling floating point computations (addf, subf & movf) <br>
- Error Handling & flag register: The program is able to generate errors for different types of invalid instructions in assembly code along with the line no. in which the error is encountered. The flag register is set by overflows & comparison instruction. 
- Bonus part: The assembler & simulator also handles 5 instructions that I have designed on my own i.e. increment, decrement, left rotate, right rotate & swap. A brief description of these instructions are given in the `readmeQ4.md` file. (bonus part testcases along with their bins & traces has been added in `/simple` folder in `/tests`) <br>

🧰 **Supported Instruction Set Architecture**
This project supports the [ISA mentioned here](https://github.com/shobhitraj1/risc-Assembler-and-Simulator/blob/25c5e0a595713494cf1de1e57eb046e7f70ae93f/CO_project%20_2023.pdf).

📚 **Course Details:**<br>
Instructor's name - Tammam Tillo (tammam@iiitd.ac.in)<br>
Course Code - CSE112

📌 **Important:**
Please make sure to follow the guidelines and policies outlined by the institution regarding the use of shared coursework materials. Use this repository responsibly and avoid any violations of academic integrity. Codes are provided for reference purposes only. It's recommended to understand the solutions and implement them independently.
