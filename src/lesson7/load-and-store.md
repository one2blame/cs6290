# Load and Store

Now that we've discussed how Tomasulo's algorithm handles data dependencies for
floating point instructions, how does it handle **memory dependencies**? Well
first, what memory dependencies are there? They're actually the same three
categories as data dependencies:

* **RAW** - an instruction stores a word to some address and then a different
instruction loads a word from that same address - this is a true dependency.
* **WAR** - an instruction loads a word from memory and then another instruction
stores a word into memory; if these instructions got re-ordered, we could
possibly load the value from the store, thus giving us incorrect program
execution.
* **WAW** - two instructions both write to the same address; if these
instructions are re-ordered, it's possible that a stale value is written to the
address.

So what do we do about this?:

* In Tomasulo's algorithm, we execute load and store instructions in order. Even
if a load instruction is ready to execute, it will be stalled until the store
instruction preceding it is completed - even if that store instruction is
stalled waiting on some value.
* Modern processors identify dependencies, re-order load instructions, etc.
similar to how floating point instructions are handled by Tomasulo's algorithm.
These techniques will not be discussed in this lesson, however, they will be
touched upon later.