---
title: Software Security
---

# Types of memory

<Definition name="DRAM">
{`
1 Transistor per bit
* Slow
* Cheap
`}
</Definition>

<Definition name="SRAM">
{`
4+ Transistors per bit
* Fast
* Expensive
* Takes up space on die
`}
</Definition>

# Computer Architecture

![image](/img/Year_2/Networks_and_Systems/Software/Computer_Architecture.png)

# GPU

**GDDR5** is "slow" and cheap

# The Stack

![image](/img/Year_2/Networks_and_Systems/Software/stack.png)

- When a program thread starts, the operating system reserves some
  amount of space for the stack - stack memory does not grow during
  runtime

The stack being full is cased by

- Badly written recursive functions

- Too much local memory allocated (especially with multi-threading)

# The Heap

![image](/img/Year_2/Networks_and_Systems/Software/heap.png)

- Memory is not guaranteed to be initialised to zero

- Can malloc memory to same size of some sensitive data

- Stack is in registers, heap is in main memory

# Understanding the platform

- The key to writing good, secure software is to understand the
  platform

- Hardware is the base platform (for software)

- Lots of things get in the way