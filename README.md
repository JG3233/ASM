# asm
A repository for writing simple x86 assembly programs.

## Compilation
Running on my 64-bit Intel, I compile my .asm files in 2 steps.

1. Produce an object file from the asm
2. Link the object file and produce an executable ELF file

`nasm -f elf64 hello.asm`

This will produce our hello.o file.

`ld -o hello hello.o` 

Now we have an executable called 'hello'. To run it, make sure it is an ELF file and has the executable permissions, and then execute the command!

`file hello`       
`ls -l`      
`./hello` 

We can do the same with any similar simple .asm file.
