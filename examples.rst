---
title: Futhark by Example
---

The following is a hands-on introduction to Futhark through a
collection of commented programs, listed in roughly increasing order of
complexity.  You can load the programs into `the interpreter
<https://futhark.readthedocs.io/en/stable/man/futhark-repl.html>`_ to
experiment with them.  For a conventional introduction to the
language, `Parallel Programming in Futhark`_ may be a better choice.
For more examples, you can check the `examples directory in the
Futhark repository`_, or our implemented benchmarks_.  We also
maintain a list of `projects using Futhark`_.

.. _`Parallel Programming in Futhark`: https://futhark-book.readthedocs.io
.. _`projects using Futhark`: #projects-using-futhark
.. _`examples directory in the Futhark repository`: https://github.com/diku-dk/futhark/tree/master/examples

Some of the example programs use `directives
<https://futhark.readthedocs.io/en/latest/man/futhark-literate.html>`_
for plotting or rendering graphics.

* `Basic usage with the factorial function <examples/fact.html>`_

* `Primitive values <examples/values.html>`_

* `Functions <examples/functions.html>`_

* `Arrays <examples/arrays.html>`_

* `Basic parallelism <examples/basic-parallelism.html>`_

* `Tuples and records <examples/tuples-and-records.html>`_

* `Scans and reductions <examples/scan-reduce.html>`_

* `Parametric polymorphism <examples/parametric-polymorphism.html>`_

* `Gather and scatter <examples/gather-and-scatter.html>`_

* `Pipe operators <examples/piping.html>`_

* `Sum types and pattern matching <examples/sum-types.html>`_

* `Loops <examples/loops.html>`_

* `Benchmarking <examples/benchmarking.html>`_

* `Counting elements that satisfy property <examples/filter-length.html>`_

* `Reducing the result of a filter <examples/filter-reduce.html>`_

* `Scattering the result of a filter <examples/filter-scatter.html>`_

* `Size parameters <examples/size-parameters.html>`_

* `Matrix multiplication <examples/matrix-multiplication.html>`_

* `Pairwise L₁ distances <examples/pairwise-l1.html>`_

* `Searching <examples/searching.html>`_

* `Computing histograms <examples/histograms.html>`_

* `Moving average <examples/moving-average.html>`_

* `Radix sort <examples/radix-sort.html>`_

* `Abstract data types <examples/abstract-data-types.html>`_

* `Testing for associativity <examples/testing-associativity.html>`_

* `Reducing or scanning without a neutral element <examples/no-neutral-element.html>`_

* `Random numbers <examples/random-numbers.html>`_

* `Gaussian blur (with Python integration) <examples/gaussian-blur.html>`_

* `Three-dimensional vectors <examples/3d-vectors.html>`_

* `Faking nominal types <examples/nominal-types.html>`_

* `Triangular matrices <examples/triangular.html>`_

* `Binary search <examples/binary-search.html>`_

* `AD with dual numbers <examples/dual-numbers.html>`_

Literate Futhark
----------------

* `Basic use of literate Futhark <examples/literate-basics.html>`_

Examples from Dex
-----------------

The following examples are ported from `Dex
<https://github.com/google-research/dex-lang>`_, a dependently typed
functional array language that uses a somewhat different approach to
describing loop processing.  We've tried to keep the original naming
scheme and programming style.

* `Prelude <examples/dex-prelude.html>`_

* `Mandelbrot set <examples/dex-mandelbrot.html>`_

* `Multi-step ray tracer <examples/dex-raytrace.html>`_

* `Monte Carlo estimates of pi <examples/dex-pi.html>`_

* `Brownian motion <examples/dex-brownian-motion.html>`_

* `Sierpinski triangle <examples/dex-sierpinski.html>`_

Projects using Futhark
----------------------

The majority of written Futhark code is probably still Futhark's own
test and benchmark suites.  However, there are some programs that have
been written in Futhark because it was a good tool for the job, and
not just to test the compiler.  A possibly incomplete list:

`Diving Beet <https://github.com/Athas/diving-beet>`_ is a *falling
sand* game, which is a kind of simple particle simulator toy.  Its
main purpose is to produce pretty effects.  There is a `blog post
</blog/2016-12-04-diving-beet.html>`_ with details and a video.

`Futball <https://github.com/Athas/futball>`_ is a game about avoiding
getting hit by balls.  The rendering engine is a ray tracer written in
Futhark.

`Futcam <https://github.com/nqpz/futcam>`_ is an application that
applies stacks of interactively configurable filters to a webcam
stream.  Futhark is used to implement the filters.

`Futracer <https://github.com/nqpz/futracer>`_ is a fairly slow
brute-force ray tracer written in Futhark.

`Futswirl <https://github.com/nqpz/futswirl>`_ is a fractal generator
based on `iterated function systems
<https://en.wikipedia.org/wiki/Iterated_function_system>`_.

`Neptune <https://github.com/filecoin-project/neptune>`_ is an
implementation of the `Poseidon hash function
<https://www.poseidon-hash.info/>`_ tuned for `Filecoin
<https://filecoin.io/>`_, where `the GPU parts
<https://github.com/filecoin-project/neptune-triton>`_ have been
implemented in Futhark.

`Palathark <https://githepia.hesge.ch/orestis.malaspin/palathark>`_ is
a Futhark implementation of the lattice Boltzmann method.

`Ray Tracing in One Weekend in Futhark
<https://github.com/athas/raytracinginoneweekendinfuthark>`_ and `Ray
Tracing: the Next Weekend in Futhark
<https://github.com/athas/raytracingthenextweekinfuthark/>`_ are
implementations based on Peter Shirley's book series.  These are by no
means real-time ray tracers, but support advanced effects and make use
of acceleration structures like BVH trees.
