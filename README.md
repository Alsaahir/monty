<h1>The Monty language</h1>

Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). <br />
It relies on a unique stack, with specific instructions to manipulate it. The goal of this Repository<br />
is to create an interpreter for Monty ByteCodes files.<br /><br />

<h3>The monty program</h3>

***Usage:*** *monty file*<br />
where file is the path to the file containing Monty byte code<br />
If the user does not give any file or more than one argument to the program, it prints an error message<br />
If, for any reason, it’s not possible to open the file, it prints the error message **Error: Can't open file <file>** where <file> is the name of the file<br />
If the file contains an invalid instruction, it prints the error message **"L<line_number>: unknown instruction <opcode>"** where L is the line number where the instruction appears.<br />
The monty program runs the bytecodes line by line and stops if either:
    * it executed properly every line of the file
    * it finds an error in the file
    * an error occured
