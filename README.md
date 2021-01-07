This repository contains some programs from Rustan Leino's book
"Program Proofs" verified with Why3.

Author: Jean-Christophe Filliâtre (CNRS)

Rustan Leino's book "Program Proofs" is an introduction to program
verification using the programming language
[Dafny](https://github.com/dafny-lang/dafny) and its program verifier.
[Why3](http://why3.lri.fr/) is another tool for deductive program
verification, with its own programming language, WhyML, and its
program verifier.

This repository follows the structure of Rustan's book, with one
subdirectory per chapter. When relevant, source files contains
comments about the differences between Dafny and Why3.

The Why3 programs have been verified using Why3 version 1.3.3 and
off-the-shelf SMT solvers, namely Alt-Ergo 2.3.0, CVC4 1.7, and Z3
4.8.6. Most of the time, any of the three suffices to complete the
verification. It can be done on the command line, e.g.

    why3 prove -P alt-ergo file.mlw

or interactively using Why3's GUI

    why3 ide file.mlw

