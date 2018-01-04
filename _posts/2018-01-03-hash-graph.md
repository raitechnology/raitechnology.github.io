---
layout: post
title: Hashing for Free
---

Using hashtable prefetches to hide memory latency.

One of the more difficult to use instructions is the prefetch code which allows
you to hide memory latency.  Memory latency can be significant, especially for
large in-memory databases, it is on the order of 100ns and is not decreasing
very much with each new CPU generation.  Around 4 hash codes can be computed in
the same time that a memory access completes.  The question is this:  Can the
hashing and the memory loads be pipelined such that hashing and memory fetching
are concurrent?

<a href="https://github.com/raitechnology/raitechnology.github.io/blob/master/public/2018-01-03-hash-graph.adoc">Continue</a>

