Monty Interpreter
Introduction
The Monty Interpreter is a program designed to execute Monty ByteCode files. Monty ByteCode files have the .m extension and contain a series of instructions to manipulate a unique stack data structure. The interpreter reads and processes these instructions to perform stack operations.

Compilation and Execution
To compile the Monty Interpreter, use the following command:
gcc -Wall -Werror -Wextra -pedantic *.c -o monty
To run the interpreter with a Monty ByteCode file, use:
./monty bytecode_file

Available Operation Codes
push: Pushes an element onto the stack.
Example: push 1 (pushes the value 1 onto the stack)

pall: Prints all values on the stack from top to bottom.

pint: Prints the value at the top of the stack.

pop: Removes the top element from the stack.

swap: Swaps the top two elements of the stack.

add: Adds the top two elements of the stack; result replaces the second element.

nop: No operation; does nothing.

sub: Subtracts the second element from the top element; result replaces the second element.

div: Divides the second element from the top element; result replaces the second element.

mul: Multiplies the top two elements of the stack; result replaces the second element.

mod: Computes the remainder of the second element from the top element; result replaces the second element.

#: Indicates a comment; the line is ignored.

pchar: Prints the ASCII character of the value at the top of the stack.

pstr: Prints the ASCII characters represented by the stack's values until encountering 0 or non-ASCII.

rotl: Moves the top element of the stack to the bottom.

rotr: Moves the bottom element of the stack to the top.

stack: Sets the stack format (LIFO) for data storage.

queue: Sets the queue format (FIFO) for data storage.
Example Monty ByteCode File
push 1
push 2
push 3
ball
add
pull
This example pushes values 1, 2, and 3 onto the stack, prints all values (3, 2, 1), performs addition (5), and then prints the updated stack (5, 1).
Conclusion
The Monty Interpreter allows you to execute Monty ByteCode files, performing various stack operations based on the provided instructions.
This enables manipulation and calculation using a stack data structure, making it a useful tool for programming and scripting tasks.