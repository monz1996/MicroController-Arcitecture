# MicroController-Arcitecture

Problem

A microcontroller architecture that is supposed to simulate how input runs through the
datapath and how different operations are applied depending on the type of input, it also
simulates how instruction set architecture operations gets translated into machine code
and how the machine interprets it.

Idea

1- Create the main memory and cache memory using arrays.
2- Create the Program Counter Class and Arithmetic Logic Unit Class.
3- Create a class for the processor. (my part)
4- Create a class for each stage of the processor class.

Implementation

1- Fetch Instruction Stage: The instruction is received in the cache from the main
memory (The Ram), the Program counter is incremented to point at the next empty
position in the memory.
2- Decode Instruction: The Instruction is divided into into sub-parts to determine
the type of the register used, determine which kind of operation we are going to
use by the operation code, is it Arithmetic Operation ? Write in Register
Operation ? Jumping Operation, then we determine what Function is the
instruction.
3- Execute: Now we check the condition of the operation if exist, for example
there is a Jump if Zero operation, if the condition is met we then execute the

instruction.
4- Memory Access: According to the function we either read data from the
Cache memory and send it to the output, or we write in the cache memory.
5- Write Back: We check certain flags to know the register destination of the
instruction, and we send this information.
I implemented the Processor which does all the points mentioned.

Result

The result was very good and it passed all the tests, we followed the Project precisely
and the output was what we expected.

Looking Back

I think that this project was not about challenging our minds or skills, I think the point of
this project was to teach us how the Von Neumann Architecture works and apply this
knowledge to get a strong grasp of the Architecture.

Challenges

Deciding the amount of variables and data types to give the best result was the only
challenging part in this project.

Different

I insisted on a certain distribution of the project among my teammates and ignored all
the ideas that they proposed, thinking that my distribution was the best without even
considering what they were saying, it was pretty arrogant of me and if I were to go back
I would listen to everything they had to say.
