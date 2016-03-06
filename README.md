# Cdown
Example of how to shutdown from C code.

   The code is quite simple (just a command line call from C code), however the intertesting point it's how to setup permissions for executing it.
   
   The problem to solve:
   
   Calls like 'shutdown, halt or reboot' must be executed by root user.
   
   Way to solve:
   
   Open Terminal/Console and chage directory to your program. (Use cd <wherever>)
   Use chmod u+s <nameOfAppWhichShutDowns>
   ./<nameOfAppWhichShutDowns>
   
   This allows the program to get superuser rights when the command line call is made.
