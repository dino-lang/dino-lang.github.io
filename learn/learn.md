---
layout: default
title: Learn Dino
---

* [Overview of the Programming Language Dino and its implemenation](overview.html)

* [Introduction into Dino by writting a small generator of syntactic parsers](intro.html)

* [Implementation of the Programming Language Dino -- A Case Study in Dynamic Language Performance](dino.pdf):
    The article gives a brief overview of the current state of programming
    language Dino in order to see where its stands between other dynamic
    programming languages.  Then it describes the current implementation,
    used tools and major implementation decisions including how to
    implement a stable, portable and simple JIT compiler.

    We study the effect of major implementation decisions on the
    performance of Dino on x86-64, AARCH64, and Powerpc64. In brief,
    the performance of some model benchmark on x86-64 was improved by
    **3.1** times after moving from a stack based virtual machine to
    a register-transfer architecture, a further **1.5** times by
    adding byte code combining, a further **2.3** times through the
    use of JIT, and a further **4.4** times by performing type
    inference with byte code specialization, with a resulting overall
    performance improvement of about **47** times. To put these
    results in context, we include performance comparisons of Dino
    with widely used implementations of Ruby, Python 3, PyPy and
    JavaScript on the three platforms mentioned above.

    The goal of this article is to share the experience of Dino
    implementation with other dynamic language implementors in hope that
    it can help them to improve implementation of popular dynamic
    languages to make them probably faster and more portable, using less
    developer resources, and may be to avoid some mistakes and wrong directions
    which were experienced during Dino development.
