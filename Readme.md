# Go Training

## Organization

Each module has the following sections:
- Concepts
- Exercises
- Tips
- Further Reading

## Syllabus

Module 1 - Mechanics (45 minutes)
- [Go Setup](1-Mechanics/1.1.md) (10 minutes)
  - Local install
  - System validation
- [Hello World](1-Mechanics/1.2.md) (10 minutes)
  - Line by line walkthrough
  - Compile and run
- Project Organization (25 minutes)
  - [Packages](1-Mechanics/1.3.0.md)
  - [GOPATH](1-Mechanics/1.3.1.md)
  - [Package Management](1-Mechanics/1.3.2.md)

Module 2 - Basics (40 minutes)
- [Types](2-Basics/2.1.md)
  - Basic types
  - Aliases
- [Variables](2-Basics/2.2.md)
  - Declaration and Assignment
  - Zero values
  - iota
- [Functions](2-Basics/2.3.md)
  - Arguments
  - Multi-valued returns
  - Anonymous functions
  - Closures
- [Control Flow](2-Basics/2.4.md)
  - if/else
  - for/break/continue
  - short statements
  - defer
  - panic/recover

Module 3 - Data Structures
- [Pointers](1-Mechanics/1.3.1.md)
  - Dereferencing
- [Structs](3-Data/3.2.md)
  - Definition
  - Declaration/Assignment
  - Fields
  - Nested Structures
  - Methods
- [Container Types](3-Data/3.3.md)
  - Slices
  - Lists
  - Maps
  - Looping

## Verification

Each module will have a `test/` folder. To verify your knowledge, please create a branch with "test" in the name and ensure that each `test/` passes CI. The completion board will be updated nightly.