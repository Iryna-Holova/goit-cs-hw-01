# goit-cs-hw-01

## Task 1: Assembler program

### Task Description:

Develop a program in assembler that computes the arithmetic expression `b - c + a`.

### Step-by-Step Instructions:

- The program code should calculate `b - c + a`.
- Compile and run the program to verify that it correctly computes the expression `b - c + a`.
- Your program should output the result of the computation to the screen.
- After running the program in DOSBox, take a screenshot of the DOSBox window displaying the execution result.

## Task 2: Interpreter

### Task Description:

You have the initial code of an interpreter from the lecture notes, which can process arithmetic expressions including addition and subtraction.
Your task is to extend this interpreter to also support multiplication and division operations, and correctly handle expressions containing parentheses.

### Step-by-Step Instructions:

**Lexer (`Lexer` Class)**

- Add new token types for multiplication (`MUL`), division (`DIV`), and parentheses (`LPAREN` and `RPAREN`) to the `Lexer`.
- Modify the `get_next_token` method of the `Lexer` class to recognize these new symbols.

**Parser (`Parser` Class)**

- Add a `factor` method to handle numbers and expressions within parentheses.
- Modify the `term` method to include multiplication and division.
- Make appropriate changes to the `expr` method to support the new hierarchy of operations.

**Interpreter (`Interpreter` Class)**

- Enhance the `visit_BinOp` method in the `Interpreter` class to handle multiplication and division operations.

### Testing:

Verify the correctness of the interpreter's functionality on various arithmetic expressions, including expressions with parentheses. For example, `(2 + 3) \* 4` should result in 20.
