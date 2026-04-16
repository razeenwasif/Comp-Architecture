# Codebase Guide

Welcome to the 16-bit CPU and Compiler project. This guide
will help you navigate the repository.

## Hardware (hw/)
The hardware is designed using Digital.
- The main CPU circuits are located in the root of hw/src.
- Look at basic-cpu.dig and extended-cpu.dig as the
  primary entry points.
- Extenders, ALUs, and Decoders are modularized into
  separate .dig files.

## Compiler (compiler/)
The compiler is designed to take high-level code and compile
it down to our custom 16-bit ISA.
- lexer/: Breaks source code into tokens.
- parser/: Builds the Abstract Syntax Tree (AST).
- semantic/: Validates rules and types.
- codegen/: Translates the AST into assembly.

## Best Practices
- Keep line lengths under 70 characters in documentation.
- Ensure all hardware modules are independently testable.
- Write unit tests for each compiler stage.
