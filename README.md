opipe
=====

More generic version of the UNIX pipe

specification
=============
 - it is always possible to write in an opipe
 - if there is too much data into the pipe, it will
   be be backed by a file on disk
 - one can only read if something has previously written one record
 - be able to specify the field seperator function/program to use
   (a demultiplexer)
 - be able to specify the field aggregator function/program to use
   (a multiplexer)
 - be able to specify the function/program to use during map
 - set the number of cores to use during computation
 - set the number of blocks to read at once (default to 1)

dependencies
============

- OCaml
- OCaml batteries for an extended library
- Parmap for parallelization
- OPAM for packaging
- obuild would be nice to compile

TODO
====

- complete the specification
