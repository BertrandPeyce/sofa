
This is not the official repository

SOFA-Issue: 2021-05-12

This is the IAU Standards of Fundamental Astronomy (SOFA) Libraries product, 
issued on 2021-05-12. The tag `SOFA-Issue' above defines this release and 
differentiates it from previous or subsequent releases of the SOFA product.
The 00READ.ME file must remain with this distribution set.

Changes made since the previous release are noted in the file changes.lis. 

Notes:

1/  Unix users:  The distribution set contains a simple makefile which 
    can be used to create a single object library for the SOFA Libraries.
    To build the object library:

    a/  Examine the makefile to be sure definition of the C compiler
        is correct for your system.  You need an ANSI standard compliant
        C compiler.  Edit the CCOMPC macro in the makefile as necessary.

    b/  To create libsofa.a, execute make:

        % make

        (where % is the shell prompt).

    c/  To remove the object files:

        % make clean

    To link with the SOFA library, include the library in the compile/link
    command in the normal Unix fashion, eg:

        % gcc myprog.c -o myprog libsofa.a

    You should specify the appropriate C compiler name for `gcc'
    in the above command sequence.


2/  Windows/DOS/Mac users:  There is no `build' procedure to create a linkable
    object library or DLL for the SOFA Libraries.  This is due to the many
    different C compilers and development environments available on
    Windows/DOS and Mac machines.  

    To use the SOFA routines with your program(s), you must use your preferred
    development environment to create the appropriate library or DLL.

IAU SOFA Center
2021/05/10
