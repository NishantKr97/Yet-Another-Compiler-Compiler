# Yet Another Programming Language

This is a basic interpreter built using `bison` and `flex` for the a programming language defined by the following grammar:

<br>
Yacc (Yet Another Compiler-Compiler) is a computer program for the Unix operating system developed by Stephen C. Johnson. It is a Look Ahead Left-to-Right (LALR) parser generator, generating a parser, the part of a compiler that tries to make syntactic sense of the source code, specifically a LALR parser, based on an analytic grammar written in a notation similar to Backus–Naur Form (BNF). Yacc is supplied as a standard utility on BSD and AT&T Unix.GNU-based Linux distributions include Bison, a forward-compatible Yacc replacement.

<br>

```
<expr> := [ <op> <expr> <expr> ] | 
                 <symbol> | <value>
<symbol> := [a-zA-Z]+
<value> := [0-9]+
<op> := ‘+’ | ‘*’ | ‘==‘ | ‘<‘
<prog> := [ = <symbol> <expr> ] |
          [ ; <prog> <prog> ] |
          [ if <expr> <prog> <prog> ] |
          [ while <expr> <prog> ] |
          [ return <expr> ]
```

## Requirements

To build the interpreter you need `flex` and `bison` installed.

For installing bison and flex on Ubuntu, use the following command:

```bash
sudo apt install build-essential bison flex
```

## Building the Interpreter

To build the interpreter use the following command:

```bash
bash build
```

To clear the build files for a new build, use the following:

```bash
bash clean
```


