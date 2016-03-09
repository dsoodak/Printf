# Printf
printf() function that can print binary and non-decimal floats

It has minimal dependencies (just "stdarg.h" to allow variable number of inputs) to conserve space on small chips, and uses pure c for chips where there is no cpp compiler. It is up to the user to define the function PutChar(). The file SerialIO.cpp has an example of this function for the Windows command line, as well as a non-blocking GetChar(). If you make your own PutChar(), remove "#include SerialIO.h" from the top of "Printf.C".

I put binary in from the very first version (written around 2010-ish) because it makes it so much easier to debug register values when they are displayed in separate characters.  I just added the ability to print floats in binary & hex as I was neatening up the code for publishing. I'm not sure what this feature might be used for but the function seemed somehow incomplete without it. I didn't bother adding octal printing because I never use it.

Dustin Soodak

