# TI-83

This repository contains several useful files for running assembly code on the TI-83
calculator, or the TI-82 STATS calculator.

It is reccomended to obtain a copy of the ti83.inc file, as it contains many useful defines
that make your job writing assembly far easier.
It is also a good idea to pick up the spasm assembler(https://github.com/alberthdev/spasm-ng)
as it can compile to .83p, .8xp and several other file formats for TI calculators.

To compile with spasm, just run spasm64 inputfile outputfile. This will produce an output
file depending on the file extension you have selected for the output file.
Then you can load the program on to your calculator with a TI SilverLink or by typing out the
hex codes manaully(strongly reccomended to avoid doing this if possible).

To run the assembly once it is on your calculator, run `Send(9prgmASMFILE)` and it will execute
it as assembly code. If it does not work, make sure you have the correct program in the Send(
command and that the hexcodes are correct. If it is still not working, try running a different
assembly program.

In this repository is the ti83.inc file, which will make writing assembly much easier. There is
also a sample assembly program that will output the text Hello, World! to the screen. This has
been tested so if it does not work, there is something else wrong.

There are also several handy scripts for compiling your code, although they do require spasm to
be in the same directory as they are. To use these, simply type either
``
.\spasm-win.bat inputfile outputformat
``
or
``
./spasm-linux.sh inputfile outputformat
``
And it will compile your assembly file into the specified file format.

Note: There is a ti83asm.inc file that can be found in spasm, it is reccomended not to use this
as it does not contain as many defines as the one included in this repo.