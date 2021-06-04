# Stellio JS

Stellio JS is a Visual Programming Language intended to use as a Scripting Language for a website builder.
As of now it is in the stage of a very small programming language with minimal features.

## Features

- numbers
- strings
- variables
- functions
- lambda functions
- other data types (like arrays and dictionaries) can be supported via
  adding runtime functions

## Code Example

The following code example contains all of the features of the language:

```
print("Hello, world")
print("3 + 5 =" add(3 5))

hello = (subject) => {
    print(concat("Hello, " subject))
    print(concat("Hello, " subject))
}

doIt = () => {
    print("Do it!")
}

doIt()

hello("Brother")

classmates = split("Jerry Jordan Johnny Jack Jeffery" " ")

each(classmates (peep) =>
    print(concat("Hello " peep))
)

fib = (n) =>
    if(eq(n 1)
        () => 1
        () =>
            if(eq(n 2)
                () => 1
                () =>
                    add(
                        fib(subtract(n 1))
                        fib(subtract(n 2))
                    )
            )
        )

print(fib(9))
```

## Todo List

Steps taken in building this language

- parser ----------------- []
  - define moo lexer ----------------- []
    - number literal ----------------- []
    - string literal ----------------- []
    - assignment operator ----------------- []
    - identifier ----------------- []
    - parans ----------------- []
    - braces ----------------- []
    - fat arrow ----------------- []
    - whitespace ----------------- []
    - newline ----------------- []
  - make a parse.js that creates .ast files []
  - variable assignment ----------------- []
  - function call ----------------- []
  - multiple lines ----------------- []
  - lambda function ----------------- []
  - comments ----------------- []
- generator ----------------- []
  - make a generate.js that creates .js files []
  - variable assignment ----------------- []
  - function call ----------------- []
  - runtime functions ----------------- []
  - lambda function ----------------- []
  - comments ----------------- []
- code testing ----------------- []
