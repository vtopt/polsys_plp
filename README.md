# ACM TOMS Algorithm 801: POLSYS_PLP: a partitioned linear product homotopy code for solving polynomial systems of equations

POLSYS_PLP consists of Fortran 90 modules for finding all isolated solutions of a complex coefficient polynomial system of equations. The package is intended to be used in conjunction with HOMPACK90 (Algorithm 777), and makes extensive use of Fortran 90 derived data types to support a partitioned linear product (PLP) polynomial system structure. PLP structure is a generalization of m-homogeneous structure, whereby each component of the system can have a different m-homogeneous structure. The code requires a PLP structure as input, and although finding the optimal PLP structure is a difficult combinatorial problem, generally physical or engineering intuition about a problem yields a very good structure. POLSYS_PLP employs a sophisticated power series end game for handling singular solutions, and provides support for problem definition both at a high level and via hand-crafted code. Different PLP structures and their corresponding Bezout.

 - This code has been re-uploaded with the permission of Dr. Layne Watson.
   All comments and questions should be directed to him (see contact info at
   the bottom of this file).

## Structure and Usage

The original source code, exactly as distributed by ACM TOMS, is included in
the ``src`` directory.
The ``src`` directory also contains its own ``README``, build instructions,
and a test case.
Comments at the top of each subroutine document their proper usage.

## Reference and Contact

To cite this work, use:

```
    @article{10.1145/347837.347885,
        author = {Wise, Steven M. and Sommese, Andrew J. and Watson, Layne T.},
        title = {Algorithm 801: POLSYS_PLP: A Partitioned Linear Product Homotopy Code for Solving Polynomial Systems of Equations},
        year = {2000},
        volume = {26},
        number = {1},
        journal = {ACM Trans. Math. Softw.},
        pages = {176–200},
        doi = {10.1145/347837.347885}
    }
```

Inquiries should be directed to

Layne T. Watson,
Department of Computer Science, VPI&SU,
Blacksburg, VA 24061-0106;
(540) 231-7540;
ltw@vt.edu

