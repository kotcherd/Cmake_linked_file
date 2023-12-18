# Cmake_linked_file

===== to test:
source @go

=====START
I had issues building a library with CMake where some of the source files were links.  Here is a contrived example to re-create that situation... it works! 
The original library didn't work because some of the links were broken.  For this example, be sure that three.f90 points into the THREE directory.
Anyhow, I think it is a useful fortran example.  It has interdependent modules to experiment with proper compilation order.
