***********What is Execution Context?**************

        Execution Context is the environment where JavaScript code is created and executed.


>>>>>>>>Before running any code, JavaScript first sets up an environment that decides:

--------Which variables exist

--------Which functions exist

--------Where variables are accessible from

--------What this refers to

********JavaScript never executes code directly*****
  ***It always creates an execution context first***

  #Types of Execution Context

JavaScript has two main types of execution contexts:

1. Global Execution Context (GEC)

    =>Created when the JavaScript file starts running

    =>Created only once

    =>Associated with the global object (window in browsers)

    =>this refers to the global object

2. Function Execution Context (FEC)

   =>Created every time a function is called

   =>Each function call gets a new execution context

   =>Has its own variables and scope

  ****Phases of Execution Context (Most Important)****

Each execution context works in two phases:

Phase 1: Creation Phase (Memory Creation)

         In this phase, JavaScript prepares the environment.

What happens:

    Memory is allocated for variables → set to undefined

      Function declarations are stored completely in memory

           Scope chain is created

             Value of this is determined

⚠️ No code is executed in this phase!!!!!!!

This phase is the reason hoisting exists in JavaScript.

Phase 2: Execution Phase (Code Execution)

    In this phase, JavaScript:

          Executes code line by line

             Assigns actual values to variables

                 Executes function calls

Example Walkthrough :-

var a = 10;

function greet() {
  console.log("Hello");
}

greet();

    ***Step-by-step Execution:***
1. Global Execution Context is created

Creation Phase:

a → undefined

greet → function stored in memory

Execution Phase:

a is assigned value 10

greet() is called

2. Function Execution Context for greet() is created

Creation Phase:

Local variables (none here)

this keyword set

Scope chain created

Execution Phase:

console.log("Hello") is executed

After execution, the function execution context is destroyed.

Execution Context and Call Stack

JavaScript uses a Call Stack to manage execution contexts.

Global Execution Context is pushed first

Function Execution Context is pushed when a function is called

When function execution finishes, its context is popped

Global context is popped when the program ends

 #Key Points to Remember

      =>Execution context is created before code runs

      =>JavaScript executes code in two phases

      =>Each function call creates a new execution context

      =>Execution contexts are managed using the call stack

      =>Understanding execution context helps in understanding:

