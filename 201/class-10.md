# Class 10 reading notes

## From the Duckett JS & JQuery Book

### Chapter 10: "Error Handling & Debugging" (pg 449-486)

The JavaScript interpreter uses the concept of execution contexts. Every statement in a script lives in one of three execution contexts:

* Global Context
* Function Context
* Eval Context

The first two execution contexts correspond with the notion of scope.

* Global Scope: If a variable is declared outside a function it can be used anywhere because it has a global scope.
* Funtion-Level Scope: When a variable is declared within a function, it can only be used within that function.

The JavaScript interpreter processes one line of code at a time. When a statment needs data from another function, it STACKS the new function on top of the current task.

Each time a script enters a new execution context, there are two phases of activity:

* Prepare
  * The new scope is created
  * Variables, functions and arguments are created
* Execute
  * Now it can assign values to variables
  * Reference functions and run their code
  * Execute statements

In the interpreter each, each execution context has its own "variables" object. It holds variables, functions, and parameters available within it. Each execution context can also access its parent's "variables" object.

JavaScript functions have LEXICAL SCOPE - they are linked to the object they were defined WITHIN.
