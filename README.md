RPx
==========================================

This is an automatic theorem prover [RPx][RPx] for first order logic without equality. 
It accepts problems in [TPTP format][TPTP] but only cnf problems have been tested.

This software is released under the [MIT License][MITLicense].

The TPTP Parser and the clausifier is based on Metis development version a0e808d746fa1f14cf944bed0d395d0df991320d
http://www.gilith.com/software/metis/
https://github.com/gilith/metis


Install
-------

Installing requires the [Poly/ML][PolyML] compiler, as well as standard system tools including GNU Make and Perl.

Build
-----

    make init

    make polyml

The executable can then be found at

    bin/polyml/rpxprover

Test
----

A simple test is to display a usage message:

    path/to/rpxprover --help

Troubleshoot
------------

You can use

    make clean

to clean out any object files.

[RPx]: https://bitbucket.org/isafol/isafol/src/master/Functional_Ordered_Resolution_Prover/ "The RPx Prover"
[MetisDevelopment]: https://github.com/gilith/metis "Metis Development"
[MetisIssues]: https://github.com/gilith/metis/issues "Metis Issues"
[MetisRelease]: http://www.gilith.com/software/metis/ "Metis Release"
[MLton]: http://www.mlton.org/ "MLton compiler"
[PolyML]: http://www.polyml.org/ "Poly/ML compiler"
[MoscowML]: http://www.dina.dk/~sestoft/mosml.html "Moscow ML compiler"
[MITLicense]: https://github.com/gilith/metis/blob/master/LICENSE "MIT License"
[TPTP]: http://www.tptp.org "TPTP"

Acknowledgements
-----------------------
RPx relies on the TPTP Parser and the clausifier from the Metis theorem prover, which is due to Joe Leslie-Hurd.
The file RPx.sml was generated by Isabelle2018. It contains code generated from theory (.thy) files by us
(Anders Schlichtkrull, Jasmin Christian Blanchette, Dmitriy Traytel -- the authors of RPx), as well
as from theory files loaded from the Isabelle distribution (https://isabelle.in.tum.de), the Archive 
of Formal Proofs (https://www.isa-afp.org) and IsaFoR (http://cl-informatik.uibk.ac.at/isafor/).
