# Concepts expplanations

1. gcc option (-Wall -Werror -Wextra -pedantic -std=gnu89
2. Betty linter
3. "System"

-Wall(Enable all common warnings)
   For catching common problems like an uninitialized variable, missing return statement in a function that supposed to return something. Helps make code cleaner and avoid bugs.

-Werror(Treat Warnings as errors)
 Acts as that strict parent. Normally when gcc encounters a warning, it still compiles the code but with this option, if gcc finds any warning, it stops the compilation amd treats it as if it were an error.

	Enforces high code standards and prevents form ignoring warnings which can potentially lead to bugs along the line. Perfect in team environments. You cant proceed without fixing the errors in your code.

-Wextra(Enable even more warnings)
 Mostly warnings about less common like problematic coding constructs or stylistic issues.Example is an unused function parameters like an implicit fall-throug in switch statements without a break stament

-pedantic(strict ANSI C/C++ conformance)
This tells the gcc to be strict about adheering to the official C or C++ standard even if GCC normally accepts them as extensions.(Like saying, Only use the exact words from the official dictionary, no slang!"
This helps for portability of your programs and code.

-std=gnu89(Standard C language to GNU C89)
Tells the compiler t interpret the code based on the C89 standard but with GNU extensions enabled.

Contrast with others: If you used -std=c89 (without gnu), GCC would be more strict and not allow the GNU extensions. Other common standards include c99, c11, c17 (or c18), and c2x for more modern C. 
