# The Cursed HTTP Tour

A guided tour, for curious non-experts, of **cursed-http**, a deliberately over-engineered entry for the
[$12 server challenge](https://github.com/arjaythedev/twelve-dollar-server-challenge): the goal is to hold 500,000
simulated users on one 1-core, 2 GB Xeon box.

**Read it: https://public.github.io/cursed-http-tour/**

It follows one request through the server: io_uring with multiple rings of direct descriptors, SIMD and
lane-parallel HTTP parsing, multi-buffer AVX-512 JWT checks, direct SQLite B-tree reads and patches, WAL
write-coalescing, the checkpoint write gate, `Connection: close` memory shedding, and the real-Xeon experiment broker.
It includes diagrams, real code excerpts and two live demos.

This repo holds only the page (`index.html`, one self-contained file). The server's source isn't public yet.

MIT licence.
