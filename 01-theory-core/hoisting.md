Hoisting refers to the behavior where JavaScript moves the declarations of variables, functions, and classes to the top of their scope during the compilation phase.

---->>>>>Hoisting applies to variable and function declarations.
---->>>>>Initializations are not hoisted; they are only declarations.
---->>>>>'var' variables are hoisted with undefined, while 'let' and 'const' are hoisted but remain in the Temporal Dead Zone until initialized.