          Hoisting refers to the behavior where JavaScript moves the declarations of variables, functions, and classes to the top of their scope during the compilation phase.

     ---->>>>>Hoisting applies to variable and function declarations.
     ---->>>>>Initializations are not hoisted; they are only declarations.
     ---->>>>>'var' variables are hoisted with undefined, while 'let' and 'const' are hoisted but remain in the Temporal Dead Zone until initialized.

     Hoisting is a powerful feature of JavaScript, but it can also be dangerous if not used correctly. By understanding how hoisting works and taking steps to avoid hoisting problems, you can write more reliable and maintainable JavaScript code.

     Some additional things to keep in mind about hoisting:

       1. Hoisting only applies to functions and variables. Other types of declarations, such as classes and modules, are not hoisted.
       2. Hoisting only occurs within a single scope. If you declare a function or variable in a nested scope, it will not be hoisted to the outer scope.
       3. Hoisting is a static process. This means that it happens before any of the code in the scope is executed. This can lead to unexpected behavior if you try to                modify a variable before it is initialized.
           Overall, it is best to avoid hoisting whenever possible. By declaring your variables and functions at the top of their scope, you can make your code more                   readable and easier to maintain.







