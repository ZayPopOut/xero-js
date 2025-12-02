# **Xero**

A compact, directive-driven language built for custom tooling, modular workflows, and Discord-focused development. Xero skips the typical programming-language baggage and leans into a clean instruction format that’s fast to parse and simple to extend.

---

``` npm i xero-js```
## **What Xero Is**

Xero uses `.xr`, `.xro`, and `.x` files.
Every file follows a straight, instruction-per-line structure. No semicolons, no curly braces, no borrowed syntax from anywhere else. The interpreter handles all translation into Node.js at runtime.

The language is intentionally minimal. You write the instruction, Xero does the heavy lifting.

---

## **Why It Exists**

* A small instruction set that stays readable
* Easy extension through modules
* A full Discord environment written for Xero
* Zero dependence on common languages
* Works seamlessly with a Node.js interpreter

Xero’s goal is to give devs a format that’s predictable and flexible without turning into another kitchen-sink language.

---

## **How Xero Files Work**

Each line is a directive.
Each directive maps to a function or action in the interpreter.
Modules live under the `::X::` namespace and behave like importable objects.

It’s simple on purpose.

---

## **Editor Support**

The Visual Studio Code extension adds:

* Syntax highlighting
* Directive formatting
* Module recognition
* Autocomplete for core instructions

Nothing fancy, just the essentials you actually need.

---

## **Project Status**

Xero is still evolving. Features shift, modules grow, syntax gets tuned.
Expect updates as the ecosystem expands and stabilizes.

---

## **License**

Use it, extend it, or build entire systems on it.
Just keep attribution to the original project.
