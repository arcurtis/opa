# Change Log

All notable changes to this project will be documented in this file. This
project adheres to [Semantic Versioning](http://semver.org/).

## Unreleased

## 0.2.0

### Language

- Set literals
- Composite and reference values in Rule head
- Complete Rule definitions containing variables
- Builtins for regular expressions, string concatenation, casting to numbers

### Compiler

- Improved error reporting in parser and compiler

### Evaluation

- Iteration over base and virtual documents (in the same reference)
- Query tracing and explanation support

### Storage

- Pluggable data storage support

### Documentation

- GoDoc strings with examples
- REST API specification
- Concise language reference

### Performance

- Per-query cache of virtual documents in topdown

And many other small improvements and fixes.

## 0.1.0

### Language

- Basic value types: null, boolean, number, string, object, and array
- Reference and variables types
- Array comprehensions
- Built-in functions for basic arithmetic and aggregation
- Incremental and complete rule definitions
- Negation and disjunction
- Module system

### Compiler

- Reference resolver to support packages
- Safety check to prevent recursive rules
- Safety checks to ensure successful evaluation will bind all variables in head
  and body of rules

### Evaluation

- Initial top down query evaluation algorithm

### Storage

- Basic in-memory storage that exposes JSON Patch style API

### Tooling

- REPL that can be run to experiment with ad-hoc queries

### APIs

- Server mode supports HTTP APIs to manage policies, push and query documents, and execute ad-hoc queries.

### Infrastructure

- Basic build infrastructure to produce cross-platform builds, run
  style/lint/format checks, execute tests, static HTML site

### Documentation

- Introductions to policy, policy-enabling, and how OPA works
- Language reference that serves as guide for new users
- Tutorial that introduces users to the REPL
- Tutorial that introduces users to policy-enabling with a Docker Authorization plugin