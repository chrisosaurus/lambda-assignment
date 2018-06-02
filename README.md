# lambda-assignment

THIS REPO HAS BEEN MOVED TO https://github.com/mkfifo/calculi

Minimum-viable lambda calculus with assignment interpreter.

Lambda calculus terms are represented by a Haskell ADT,
there is no external syntax and thus no lexer or parser.

## running

To run the unit tests:

    # you don't actually want to do this
    $ make

Output:

    lambda-assignment-0.1.0.0: test (suite: lambda-assignment-test)

    Progress: 1/2
    LambdaAssignment.Data.Exp
      testing is_trivial_expression positive cases
        Location
        AbsEnv
        Unit
        True
        False
      testing is_trivial_expression negative cases
        Var
        App
        New
        Read
        Write
        IfElse
        Abs
      testing simple env operations
        write & read
        overwrite
    LambdaAssignment.Data.Store
      testing simple store operations
        alloc
        write & read
        overwrite
    LambdaAssignment.Eval
      simple eval tests
        Unit
        Location
        True
        False
        IfElse True
        IfElse False
      lambda tests
        simple lambda
        simple application
      state tests
        new
        new & read
        new & write

    Finished in 0.0009 seconds
    28 examples, 0 failures

