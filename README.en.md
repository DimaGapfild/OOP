# Object-Oriented Programming

A university course (a continuation of the "Algorithmization and Programming" course).
Implementation language: **Python 3**.

## Structure

Each chapter is a separate folder with these files:

| File | Purpose |
|------|---------|
| `теорія.md` / `теорія.en.md` (theory) | lecture notes: concepts, syntax, examples |
| `практика.md` / `практика.en.md` (practice) | 10 tasks of the same type and difficulty level |
| `проєкт.md` / `проєкт.en.md` (project) | (chapter 12 only) final project specification, stages, and grading criteria |

## Course Outline

| No. | Chapter |
|---|--------|
| 01 | Classes and Objects |
| 02 | Constructors, Attributes, Methods |
| 03 | Encapsulation and Properties |
| 04 | Magic Methods and Operator Overloading |
| 05 | Inheritance |
| 06 | Polymorphism |
| 07 | Abstraction and Interfaces |
| 08 | Composition and Aggregation |
| 09 | Custom Exceptions and Contracts |
| 10 | Collections of Objects, Iterators, dataclass |
| 11 | UML and the SOLID Principles |
| 12 | Design Patterns and the Final Project |

## How to Work with the Material

1. Read the theory file and try out the examples in the interpreter.
2. Complete all 10 tasks from the practice file on your own.

## Grading Criteria for Practical Work

| Score | Requirements |
|-------|--------------|
| 5 | all 10 tasks, readable code, edge cases handled |
| 4 | 8–9 tasks or minor formatting flaws |
| 3 | 6–7 tasks, basic correctness |
| 2 | 4–5 tasks |
| 1 | fewer than 4 tasks |

## Clean Code: Basic Requirements

Every solution, in any language, must follow these rules.

### Size limits

| What | Limit |
|------|-------|
| File | ≤ 100 lines |
| Function / method | ≤ 20 lines |
| Class | ≤ 10 public methods |
| Function parameters | ≤ 3 |
| Nesting depth (`if` / `for` / `while`) | ≤ 3 levels |
| Line length | ≤ 80 characters (≤ 79 for Python, per PEP 8) |

If a limit is exceeded, split the code: move a class to its own file, extract a helper method, or group parameters into an object.

### Rules

1. **Meaningful names.** Names say what a thing is or does (`total_price`, not `tp`). Classes are nouns, methods are verbs, booleans read as questions (`is_empty`, `has_debt`).
2. **One responsibility.** A function does one thing; a class has one reason to change. Prefer one class per file.
3. **Early returns.** Handle invalid cases first and return, instead of wrapping the main logic in deep `if` / `else` blocks.
4. **No duplication (DRY).** Repeated code goes into a function or a method.
5. **No magic numbers.** Use named constants (`MAX_SPEED = 120`).
6. **No global mutable state.** Pass data through parameters and object attributes.
7. **Comments explain *why*, not *what*.** If code needs a comment to be understood, rename or simplify it first.
8. **Clear error handling.** Raise or throw exceptions instead of returning special codes. Never silently swallow errors.
9. **Consistent formatting.** Follow your language's style guide: [PEP 8](https://peps.python.org/pep-0008/) for Python, the [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html) for JS, and the [C++ Core Guidelines](https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines) for C++.
10. **No dead code.** Remove unused variables, functions, imports, and commented-out code.

Source: the rules follow Robert C. Martin, [*Clean Code: A Handbook of Agile Software Craftsmanship*](https://www.informit.com/store/clean-code-a-handbook-of-agile-software-craftsmanship-9780132350884) (Prentice Hall, 2008). The exact numbers in the size limits are set for this course.
