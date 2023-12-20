
Q4: (Bonus) Designing New Instructions -

My custom Assembler is able to handle these instructions in addition to the given instructions, & convert the assembly language code to machine code. The assembler is also 
able to handle errors (if any) in these instructions like typos in instruction name, reg name, invalid Imm value, etc.

My custom Simulator is able to execute these instructions in addition to the given instructions. The Increment and Decrement instructions can also set the overflow bit in
Flags register if there's an overflow.

I have created testcases for verifying the upgraded assembler & simulator (added in `/tests` to support automated testing).
- `testBonusN` files contain the assembly program added in `/tests/assembly/simpleBin` folder.
- `testBonusN` files contain the corresponding binary machine code for the assembly added in `/tests/bin/simple` folder.
- `testBonusN` files contain the traces/result of simulator when the corresponding machine code is given as input added in `/tests/traces/simple` folder.

The description of the instructions along with their opcode, semantics etc. are as follows -

1. Increment: 
Opcode - 10100
Instruction - Increment
Semantics - Increment the value of a register by a specified amount $Imm, where Imm is a 
7 bit value.
Syntax - incf reg1 $Imm
Type - B (register and immediate type)

2. Decrement:
Opcode - 10101
Instruction - Decrement
Semantics - Decrement the value of a register by a specified amount $Imm, where Imm is a 
7 bit value.
Syntax - decf reg1 $Imm
Type - B (register and immediate type)

3. Rotate Left: 
Opcode - 10110
Instruction - Rotate Left
Semantics - Rotate the bits of a register to the left by a specified number of positions 
$Imm, where Imm is a 7 bit value.
Syntax - rrl reg1 $Imm
Type - B (register and immediate type)

4. Rotate Right: 
Opcode - 10111
Instruction - Rotate Right
Semantics - Rotate the bits of a register to the right by a specified number of positions 
$Imm, where Imm is a 7 bit value.
Syntax - rrr reg1 $Imm
Type - B (register and immediate type)

5. Swap: 
Opcode - 11000
Instruction - Swap
Semantics - Swap the contents of two registers.
Syntax - swap reg1 reg2
Type - C (2 registers type)

