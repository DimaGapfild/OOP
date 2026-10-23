# Object-Oriented Programming

A university course (a continuation of the "Algorithmization and Programming" course).
Main implementation language: **Python 3**. Every example in the lectures is also given in **JavaScript** (ES2022+) and **C++** (C++20; some examples are marked C++23).

## Structure

Each chapter is a separate folder with these files:

| File | Purpose |
|------|---------|
| `теорія.md` / `теорія.en.md` (theory) | lecture notes: concepts, syntax, examples |
| `практика.md` / `практика.en.md` (practice) | 10 tasks of the same type and difficulty level |
| `проєкт.md` / `проєкт.en.md` (project) | (chapter 13 only) final project specification, stages, and grading criteria |

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
| 12 | GRASP: Assigning Responsibilities |
| 13 | Design Patterns and the Final Project |

## How to Work with the Material

1. Read the theory file and try out the examples in the interpreter.
2. Complete all 10 tasks from the practice file on your own.

## Grading Criteria for Practical Work

| Grade | Requirements |
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

## Points and Admission to the Final Assessment

The maximum for the course is **100 points**: **60** for continuous
assessment + **40** for the final assessment (a credit test or an exam, at
the instructor's discretion).

| Component | Max | How it is calculated |
|-----------|-----|----------------------|
| Practical work (chapters 1–13) | 50 | the average grade over the chapters (1–5, per the table above) × 10; a chapter not submitted counts as 0 |
| Final project | 10 | the rubric in `проєкт.en.md` (max 10) |
| **Continuous assessment** | **60** | the sum of the two rows above |
| Credit test / exam | 40 | theory part 20 + practical task 20 |
| **Total** | **100** | |

### Admission to the Credit Test or Exam

A student is admitted to the final assessment if **all** of the following
conditions are met:

1. continuous assessment — **at least 35 points out of 60**;
2. the final project is **defended** and scored **at least 5 out of 10**;
3. practical work is submitted **for at least 10 of the 13 chapters**
   (each with a grade of 3 or higher).

Students who are not admitted may rework their practical work and project and
resubmit them before the start of the exam session.

### Final Grade

The credit test/exam is passed if **at least 24 out of 40** points are earned.
The final total (continuous assessment + credit test/exam):

| Points | Grade (ECTS) | National scale |
|--------|--------------|----------------|
| 90–100 | A | excellent |
| 82–89 | B | good |
| 74–81 | C | good |
| 64–73 | D | satisfactory |
| 60–63 | E | satisfactory |
| below 60 | F | unsatisfactory (retake) |

For a **credit test** the result is "passed" (60 points or more and the
conditions above met) or "not passed".

> The exact thresholds may be refined by the instructor at the start of the semester.
