# Table of Contents
- [Table of Contents](#table-of-contents)
- [Chapter 1: Preliminaries](#chapter-1-preliminaries)
  - [1.1: Reasons for Studying Concepts of Programming Languages](#11-reasons-for-studying-concepts-of-programming-languages)
    - [Increased Capacity to express ideas:](#increased-capacity-to-express-ideas)
    - [Improved Background for choosing appropriate languages](#improved-background-for-choosing-appropriate-languages)
    - [Increased Ability to learn a new language](#increased-ability-to-learn-a-new-language)
    - [Better use of languages that are already known](#better-use-of-languages-that-are-already-known)
    - [Overall advancement of computing](#overall-advancement-of-computing)
    - [Better understanding of significance of implementation](#better-understanding-of-significance-of-implementation)
  - [1.2 Programming Domains](#12-programming-domains)
    - [**Might have talked about these in class:**](#might-have-talked-about-these-in-class)
    - [**In the textbook *know these!!!***:](#in-the-textbook-know-these)
  - [1.3 Language Evaluation Criteria](#13-language-evaluation-criteria)
    - [Criteria Definitions](#criteria-definitions)
    - [Evaluation Criteria: Cost](#evaluation-criteria-cost)
    - [Evaluation Criteria: Other](#evaluation-criteria-other)
  - [1.4 Influences on Language Design](#14-influences-on-language-design)
    - [Computer Architecture](#computer-architecture)
    - [Programming Design Methodologies](#programming-design-methodologies)
  - [1.5 Language Categories](#15-language-categories)
  - [1.6 Language Design Trade-offs](#16-language-design-trade-offs)
  - [1.7 Implementation Methods](#17-implementation-methods)
  - [Other Useful Tidbits:](#other-useful-tidbits)
- [Chapter 2: Evolution of the Major Programming Languages](#chapter-2-evolution-of-the-major-programming-languages)
  - [Individuals:](#individuals)
  - [Languages:](#languages)
  - [Other Useful Tidbits 2:](#other-useful-tidbits-2)
- [Chapter 3: Describing Syntax and Semantics](#chapter-3-describing-syntax-and-semantics)
  - [3.2 The General Problem of Describing Syntax](#32-the-general-problem-of-describing-syntax)
  - [3.3 Formal Methods of Describing Syntax](#33-formal-methods-of-describing-syntax)
    - [Backus-Naur Form (BNF) and Context-Free Grammars](#backus-naur-form-bnf-and-context-free-grammars)
    - [3.3.1.3 Fundamentals](#3313-fundamentals)
    - [3.3.1.4 Describing Lists](#3314-describing-lists)
    - [3.3.1.5 Grammars and Derivations](#3315-grammars-and-derivations)
    - [3.3.1.4 Describing Lists](#3314-describing-lists-1)
    - [3.3.1.5 Grammars and Derivations](#3315-grammars-and-derivations-1)
    - [3.3.1.7 Ambiguity](#3317-ambiguity)
    - [3.3.1.8 Operator Precedence](#3318-operator-precedence)
    - [3.3.1.9 Associativity of Operators](#3319-associativity-of-operators)
    - [3.3.1.10 An Unambiguous Grammar for if-else](#33110-an-unambiguous-grammar-for-if-else)
    - [3.3.2 Extended BNF](#332-extended-bnf)
  - [3.4 Attribute Grammars](#34-attribute-grammars)
    - [3.4.1 Static Semantics](#341-static-semantics)
    - [3.4.2 Basic Concepts](#342-basic-concepts)
    - [3.4.3 Attribute Grammars Defined](#343-attribute-grammars-defined)
    - [3.4.4 Intrinsic Attributes](#344-intrinsic-attributes)
    - [3.4.5 Examples of Attribute Grammars](#345-examples-of-attribute-grammars)
    - [3.4.6 Computing Attribute Values](#346-computing-attribute-values)
    - [3.4.7 Evaluation](#347-evaluation)
  - [3.5 Dynamic Semantics](#35-dynamic-semantics)
      - [Review Weakest Precondition in Textbook (Pg170):](#review-weakest-precondition-in-textbook-pg170)
- [Chapter 5: Names, Bindings, and Scopes](#chapter-5-names-bindings-and-scopes)
  - [5.2 Names](#52-names)
    - [5.2.1 Design Issues](#521-design-issues)
    - [5.2.2 Name Forms](#522-name-forms)
  - [5.3 Variables](#53-variables)
  - [5.4 Binding](#54-binding)
  - [5.5 Scope](#55-scope)
  - [5.6 Scope and Lifetime](#56-scope-and-lifetime)
  - [5.7 Referencing Environments](#57-referencing-environments)
  - [5.8 Named Constraints](#58-named-constraints)
- [Chapter 15: Functional Programming Languages](#chapter-15-functional-programming-languages)
  - [15.2 Mathematical Functions](#152-mathematical-functions)
    - [Named Constants:](#named-constants)
    - [Initialization:](#initialization)
    - [Example:](#example)
  - [15.3 Fundamentals of Functional Programming Languages](#153-fundamentals-of-functional-programming-languages)
    - [Functional Programming Paradigm:](#functional-programming-paradigm)
    - [Features of Functional Languages:](#features-of-functional-languages)
    - [Evolution of Functional Languages:](#evolution-of-functional-languages)
  - [15.5 An introduction to Scheme](#155-an-introduction-to-scheme)
    - [15.5.1 and 15.5.2 Origins and Interpreter](#1551-and-1552-origins-and-interpreter)
    - [15.5.3 Primitive Numeric Functions](#1553-primitive-numeric-functions)
    - [15.5.4 Defining Functions](#1554-defining-functions)
    - [15.5.5 Output Functions](#1555-output-functions)
    - [15.5.6 Numeric Predicate Functions](#1556-numeric-predicate-functions)
    - [15.5.7 Control Flow](#1557-control-flow)
    - [15.5.8 List Functions in Scheme](#1558-list-functions-in-scheme)
    - [15.5.9 QUOTE Function](#1559-quote-function)
    - [15.5.10 CAR, CDR, and CONS Functions](#15510-car-cdr-and-cons-functions)
    - [15.5.11 Predicate Functions: EQ?, NULL?, and LIST?](#15511-predicate-functions-eq-null-and-list)
    - [15.5.12 Example Scheme Functions](#15512-example-scheme-functions)
    - [15.5.13 LET Function](#15513-let-function)
    - [15.5.14 Tail Recursion in Scheme](#15514-tail-recursion-in-scheme)
    - [15.5.15 Functional Forms](#15515-functional-forms)
    - [15.5.16 Functions That Build Code](#15516-functions-that-build-code)

# Chapter 1: Preliminaries

## 1.1: Reasons for Studying Concepts of Programming Languages

There are various reasons for students to study programming languages, some of which include:

### Increased Capacity to express ideas:
Learning different programming languages can expand a programmer's thinking by introducing new concepts and structures. Even if a language lacks certain features, programmers can simulate them using techniques from other languages they know. Overall, understanding various programming languages helps programmers think more creatively and solve problems more effectively.

### Improved Background for choosing appropriate languages
When starting new projects, many stick to familiar languages, even if they're not ideal. Expanding their language repertoire would help them choose better-suited tools. While some language features can be mimicked in others, it's better to use built-in features for smoother, safer, and more elegant solutions.

### Increased Ability to learn a new language
Computer programming is always evolving, requiring continuous learning. Understanding fundamental concepts makes learning new languages easier. Like with natural languages, knowing one well helps learn others. The TIOBE index tracks language popularity, showing the need for programmers to adapt. Understanding language basics is crucial for navigating language descriptions and choosing which ones to learn.

### Better use of languages that are already known
Most contemporary programming languages are large and complex. Accordingly, it is uncommon for a
programmer to be familiar with and use all of the features of a language he or she uses. By studying the concepts of programming languages, programmers can learn about previously unknown and unused parts of the languages they already use and begin to use those features.

### Overall advancement of computing
Understanding programming language concepts provides a global perspective on computing. Popular languages aren't always the best; sometimes, lesser-known ones are superior. Lack of familiarity with language concepts can lead to the adoption of less optimal languages. For instance, ALGOL 60 was considered more elegant than Fortran but wasn't widely adopted due to a lack of understanding among programmers and managers. Better-informed language choices could lead to superior languages prevailing over inferior ones in the long run.

### Better understanding of significance of implementation
Understanding implementation significance involves grasping how programming languages translate into machine code and interact with hardware during execution. This knowledge enhances programmers' ability to optimize code for efficiency and resource usage, leading to better software performance and user experiences.

## 1.2 Programming Domains

### **Might have talked about these in class:**
1. **Game Development:** Creating video games for various platforms, including consoles, PCs, and mobile devices.

2. **Mobile Development:** Building applications specifically for mobile devices, such as smartphones and tablets, often using platforms like iOS (Swift) or Android (Java/Kotlin).

3. **Embedded Systems:** Developing software for specialized computing devices with limited resources, such as microcontrollers, IoT devices, and automotive systems.

4. **Data Science and Analytics:** Utilizing programming languages to analyze and derive insights from large datasets, often involving statistical analysis, machine learning, and data visualization.

5. **Networking and Security:** Writing software for managing and securing computer networks, including tasks like firewall configuration, network monitoring, and intrusion detection.

6. **Graphics and Multimedia:** Creating software for processing and rendering graphics, audio, and video, commonly used in areas like animation, digital art, and multimedia applications.

7. **Financial Technology (FinTech):** Developing software solutions for financial services, such as banking, trading platforms, payment processing, and financial analytics.

### **In the textbook *know these!!!***: 
1. **Scientific Applications:** Utilizing programming to solve scientific problems, such as mathematical modeling, simulations, and data analysis in fields like physics, biology, and chemistry. A language used: <mark>Fortran</mark>

2. **Business Applications:** Developing software to support business processes and operations, including enterprise resource planning (ERP), customer relationship management (CRM), and inventory management systems. A language used: <mark>Cobol</mark>

3. **Artificial Intelligence:** Creating intelligent systems and algorithms that can mimic human intelligence, including machine learning, natural language processing, computer vision, and robotics. A language used: <mark>Lisp</mark>

4. **Systems Programming:** Writing low-level software to manage hardware resources and interact with the operating system, often used in areas like operating systems development, device drivers, and embedded systems. A language used: <mark>C</mark>

5. **Web Software:** Building applications and services for the web, including websites, web applications, e-commerce platforms, and content management systems (CMS). Uses a colection of languages for various purposes. Ex: markup: <mark>HTML</mark>, scripting: <mark>PHP</mark>, and general purpose: <mark>Java</mark>

## 1.3 Language Evaluation Criteria

| Criteria               | Readability | Writability | Reliability |
|------------------------|-------------|-------------|-------------|
| Simplicity             |      ✔      |      ✔      |      ✔      |
| Orthogonality          |      ✔      |      ✔      |      ✔      |
| Data types             |      ✔      |      ✔      |      ✔      |
| Syntax design          |      ✔      |      ✔      |      ✔      |
| Support for abstraction|             |      ✔      |      ✔     |
| Expressivity           |             |      ✔      |      ✔      |
| Type checking          |             |             |      ✔      |
| Exception handling     |             |             |      ✔      |
| Restricted aliasing    |             |             |      ✔      |

### Criteria Definitions

1. **Simplicity**: This criterion evaluates how easy it is to understand and use the language. Languages that are simple tend to have clear and straightforward syntax, making them easier for programmers to learn and use effectively.

2. **Orthogonality**: Orthogonality refers to the degree to which language features can be combined and used independently of each other. A highly orthogonal language allows for a wide range of expressions and combinations without unnecessary restrictions or complications.

3. **Data types**: This criterion assesses the types of data structures and data types supported by the language. A language with robust data type support provides programmers with flexibility and control over how data is organized and manipulated within their programs.

4. **Syntax design**: Syntax design concerns the structure and rules governing the formation of statements and expressions in the language. Well-designed syntax enhances readability and writability by promoting clarity, consistency, and conciseness in code.

5. **Support for abstraction**: Abstraction allows programmers to hide implementation details and focus on higher-level concepts. Languages that support abstraction provide mechanisms such as classes, modules, and functions to encapsulate complex functionality and promote code reusability and maintainability.

6. **Expressivity**: Expressivity refers to the language's ability to concisely and effectively express computational ideas and concepts. A highly expressive language allows programmers to write concise and clear code that accurately represents their intentions.

7. **Type checking**: Type checking is the process of verifying the correctness of data types used in a program. Languages with strong type checking perform rigorous checks at compile time or runtime to ensure type safety, reducing the likelihood of errors related to data type mismatches.

8. **Exception handling**: Exception handling mechanisms enable programmers to gracefully handle runtime errors and exceptional conditions that may occur during program execution. Effective exception handling promotes robustness and reliability by allowing programs to recover gracefully from unexpected situations.

9. **Restricted aliasing**: Aliasing occurs when two or more references or pointers in a program refer to the same memory location. Restricted aliasing refers to language features or restrictions that limit the potential for aliasing, reducing the risk of unintended side effects and improving program reliability and maintainability.

### Evaluation Criteria: Cost
- Training programmers to use the language
- Writing programs (closeness to particular applications)
- Compiling programs
- Executing programs
- Language implementation system: availability of free compilers
- Reliability: poor reliability leads to high costs
- Maintaining programs

### Evaluation Criteria: Other

- Portability
  - The ease with which programs can be moved from one implementation to
another
- Generality
  - The applicability to a wide range of applications
- Well-definedness
  - The completeness and precision of the language’s official definition

## 1.4 Influences on Language Design

### Computer Architecture
The design of programming languages is heavily influenced by factors such as computer architecture and programming methodologies. <mark>The von Neumann architecture, which has been prevalent in computers since the 1940s, plays a significant role in shaping imperative languages.</mark> These languages emphasize variables, assignment statements, and iterative forms of repetition, reflecting the pipelining operation between memory and the CPU in von Neumann computers.

The fetch-execute cycle is a fundamental process in von Neumann architecture, where instructions are fetched from memory and executed in the CPU. Imperative languages are well-suited for this architecture due to their efficient handling of variables and iterative operations. <mark>Imperative languages are the most dominant due to von neumann computers.</mark> Data and programs stored in memory. Memory is separate from the CPU, instructions and data are piped from memory to the CPU.

Functional languages, on the other hand, prioritize the application of functions to parameters and often lack variables, assignment statements, and iteration. While functional languages like Scheme offer benefits, they may not displace imperative languages until non-von Neumann computers are developed to efficiently execute functional programs.

Despite the structural alignment of imperative languages with machine architecture, some argue for the naturalness of imperative languages over functional ones. They believe that even if functional programs were as efficient, imperative languages would still dominate due to perceived ease of use.

Overall, the design of programming languages is intricately linked to the underlying computer architecture and the preferences of language users.

### Programming Design Methodologies

During the late 1960s and early 1970s, the structured-programming movement spurred an in-depth analysis of software development processes and programming language design. This shift was driven by the increasing prominence of software development costs as hardware costs decreased, and as computers tackled larger and more complex tasks.

New methodologies emerged, such as top-down design and stepwise refinement, aimed at improving programmer productivity and tackling complex problems more effectively. In this era, concerns were raised about deficiencies in programming languages, particularly regarding type checking and control statements.

<mark>By the late 1970s, there was a shift towards data-oriented program design methodologies instead of process oriented</mark>, which emphasized data design and abstract data types. Data abstraction became a key aspect of software system design, supported by languages like SIMULA 67, albeit in a limited capacity initially. However, the benefits of data abstraction became more widely recognized in the early 1970s, leading to its adoption in most languages designed thereafter.

The evolution continued into the <mark>early 1980s with the emergence of object-oriented design, which builds upon data abstraction by incorporating concepts like inheritance and dynamic method binding</mark>. Object-oriented programming languages like Smalltalk introduced these concepts, which have since become integral parts of popular imperative languages such as Java, C++, and C#. Object-oriented concepts have also influenced other paradigms, including functional and logic programming.

Despite the dominance of data-oriented methods, procedure-oriented programming has not been abandoned. Recent research has focused on concurrency, leading to the development of language features to support concurrent programming units, as seen in languages like Java and C#.

Overall, these evolutionary steps in software development methodologies have led to the introduction of new language constructs to support them, reflecting the continuous evolution of programming languages.

## 1.5 Language Categories

Programming languages are often grouped into four categories: imperative, functional, logic, and object-oriented. However, object-oriented languages are usually considered extensions of imperative ones, sharing similar syntax. Scripting languages, like Perl and JavaScript, are often categorized separately, but they're essentially imperative. Logic languages, such as Prolog, use rules for computation and differ notably from other types. 

**Imperative**: 
- Central features are variables,assignment statements, and iteration
- Include languages that support object-oriented programming
(OOP)
- Includes scripting languages
- Includes the visual languages
- Language examples: C, C++, C#, Objective-C, Java, Perl, Python, Ruby, JavaScript, Visual BASIC .NET

**Functional**:
- Main means of making computations is by applying functions to given parameters
- Functions are “first class citizens”
- “Variables”, functions, and names
- Lambda calculus
- Language examples: LISP, Haskell, Racket (PLT Scheme),
Clojure, Scala, ML, F#

**Logic**:
- Rule-based (rules are usually specified in no particular order)
- Formal logic system
  - First order logic
  - Second order logic
  - Description Logic
- Language examples: Prolog, Answer Set Programming (ASP), Datalog

**Quantum**:
- Uses a single memory, not separate RAM (volatile) and
Disk (non-volatile)
- Memory in qubits that have both 1 and 0 values simultaneously
- Instruction set is very different from von Neumann architecture
  - Quil, OpenQASM
- Language examples:
  - Imperative-like: QCL, Q#, Q Language, qGCL
  - Functional-like: QFC, QPL, QML

**Markup/Programming Hybrid**
- Markup languages extended to support some other programming
- Examples: JSTL, XML, XSLT, JSON, SQL
- Many are more accurately labeled as Protocols, not full (i.e. Turing Complete) Languages

## 1.6 Language Design Trade-offs

The criteria used to evaluate programming languages often conflict with each other, making language design a challenging task. For instance, the Java language prioritizes reliability by enforcing array index range checking, which slows down program execution compared to languages like C. APL, known for its expressive array operators, sacrifices readability for writability due to its compact syntax. Similarly, the conflict between writability and reliability is evident in the flexibility of C++ pointers versus their exclusion in Java to avoid potential reliability issues. These trade-offs illustrate the complex decision-making process involved in programming language design.

## 1.7 Implementation Methods

1. **Compilation:**
   - Compilation involves translating the entire source code of a program into machine code or bytecode before execution. This process typically involves several stages, including lexical analysis, parsing, optimization, and code generation. The resulting compiled code is then executed directly by the computer's hardware. Used in large commercial applications. Has a slow translation but a fast execution. Translation consists of lexical analysis, semantic analysis, and code generation

2. **Pure Interpretation:**
   - In pure interpretation, the source code of a program is executed line-by-line or statement-by-statement by an interpreter. The interpreter reads each instruction, translates it into machine code or intermediate code, and executes it immediately. This approach does not produce an intermediate compiled form, resulting in slower execution compared to compilation. This is primarily used in small programs or when efficiency is not a concern. Easier implementation but much slower execution and requires more memory. Significant comeback for some web scripting languages: such as Javascript and PHP.

3. **Hybrid:**
   -  Hybrid implementation methods combine elements of both compilation and interpretation. Typically, the source code is initially compiled into an intermediate representation or bytecode. This bytecode is then executed by a virtual machine or interpreter. This approach offers a balance between the performance benefits of compilation and the flexibility of interpretation. Used in small/medium systems where efficiency is not the primary concern. Compromise. Perl programs are an example, the programs are partially compiled.
  
Just-In-Time: Essentially delayed compilers. .Net languages are implemented with a JIT system.

Preprocessors: A preprocessor is a program that handles code before compilation. Preprocessor instructions are embedded in programs and serve various purposes, such as including code from other files or defining symbols for expressions. For example, the C preprocessor instruction #include "myLib.h" copies the contents of myLib.h into the program at the specified position. Another common use is defining macros like #define max(A, B) ((A) > (B) ? (A) : (B)), which allows finding the maximum of two expressions. However, caution is needed with macros, as they can lead to issues like unintended side effects, especially when expressions with side effects are used as parameters. For instance, if one of the expressions passed to the max macro contains a side effect like z++, it could be evaluated multiple times, causing unexpected behavior.

## Other Useful Tidbits:

- In Computability Theory, a system of data-manipulation rules is said to be Turing Complete if it can be used to simulate any single-taped Turing machine.
- Natural Languages have ambiguous grammar while Programming languages have unambiguous grammar
- Constructed Languages or Conlangs are artificially created languages such as: programming languages, fictional languages (klingon), or gesture/sign languages. Includes more

# Chapter 2: Evolution of the Major Programming Languages

## Individuals:
1. **Charles Babbage**: An English mathematician, philosopher, inventor, and mechanical engineer who originated the concept of a programmable computer.
2. **Ada Lovelace**: An English mathematician and writer, chiefly known for her work on Charles Babbage's proposed mechanical general-purpose computer, the Analytical Engine.
3. **John von Neumann**: A Hungarian-American mathematician, physicist, computer scientist, and polymath who made major contributions to a vast range of fields, including mathematics, physics, economics, and computer science.
4. **John Backus**: An American computer scientist who developed the high-level programming language FORTRAN (Formula Translation).
5. **Donald Knuth**: An American computer scientist, mathematician, and professor emeritus at Stanford University, best known for his multi-volume work, "The Art of Computer Programming."
6. **Brian Kernighan and Dennis Ritchie**: Kernighan is a Canadian computer scientist who co-authored several seminal books on programming languages, while Ritchie, who passed away in 2011, was an American computer scientist who created the C programming language and contributed significantly to the development of Unix.

## Languages:
1. **Plankalkül**: An early programming language designed for engineering purposes by Konrad Zuse in the late 1940s and early 1950s. Not published until 1972. Never implemented in its original form but had advanced data structures.
2. **“Pseudocode”**: A high-level description of an algorithm or a program written in plain English, used as a tool for planning and sketching algorithms before coding.
3. **IBM 704 & Fortran**: The IBM 704 was an early mainframe computer, and Fortran (short for "Formula Translation") was the first high-level programming language designed for numerical and scientific computing.
4. **LISP**: A high-level programming language known for its unique approach to symbolic computation and its influence on the development of artificial intelligence.
5. **Prolog**: A logic programming language associated with artificial intelligence and computational linguistics.
6. **Java**: A general-purpose programming language known for its "write once, run anywhere" approach, widely used for building enterprise-scale applications, web servers, and Android apps.
7. **C/C++**: C is a procedural programming language developed by Dennis Ritchie, while C++ is an object-oriented extension of C designed by Bjarne Stroustrup. Both languages are widely used for systems programming, game development, and application software.
8. **Perl**: A high-level, interpreted programming language known for its powerful text-processing features and practical extraction and reporting capabilities.
9.  **Python**: A versatile, high-level programming language known for its simplicity and readability, widely used in web development, data analysis, artificial intelligence, and scientific computing.
10. **Ruby**: A dynamic, reflective, object-oriented programming language known for its simplicity and productivity, often used for web development and scripting.
11. **Ada**: A structured, statically typed, imperative, and object-oriented high-level programming language, developed by a team led by Jean Ichbiah of CII Honeywell Bull under contract to the United States Department of Defense.
12. **COBOL**: Common Business-Oriented Language, primarily used in business, finance, and administrative systems for companies and governments.
13. **SNOBOL**: A high-level programming language known for its powerful string manipulation capabilities, especially for text processing.
14. **Pascal**: A procedural programming language designed for teaching programming, known for its structured programming constructs.
15. **Smalltalk**: An object-oriented, dynamically typed, reflective programming language known for its simplicity and flexibility, often used for GUI development.
16. **Scheme, Racket**: Lisp dialects known for their simple syntax and powerful macro system, widely used in education and research.
17. **Haskell**: A purely functional programming language known for its strong static typing and lazy evaluation, often used in academia and industry for research and production.

## Other Useful Tidbits 2:
- The first programming language was related the the computation of Bernoulli Numbers. In 1843 on the Analytical Engine pioneered by <mark>Charles Babbage</mark> and programmed by <mark>Ada Lovelace</mark>
- Source code is stored in files. File structure is composed of pages and sectors
- EsoLangs: languages that are created as a joke.

# Chapter 3: Describing Syntax and Semantics

## 3.2 The General Problem of Describing Syntax

**Syntax Rules of Programming Languages**
- *Definition*: A language consists of all valid statements, or strings, in that language, potentially infinite in number.
- *Grammar*: A formal description of a language, characterized by a finite set of rules.
- *Syntax*: A formal method used to determine if a statement belongs to a language's set of valid statements.
- *Example*: Consider a language composed of non-zero even numbers of the letter "a". While this set has infinitely many members, its syntax can be concisely described using a finite set of Backus-Naur Form (BNF) rules, such as S ⟶ aa | aaS.
- *Grammars*: Can be utilized in two distinct ways: for recognition and for generation.
  
**Language Recognizers**
- *Recognition Method*: Defines languages by constructing a recognition device capable of determining if a given string of characters is in the language.
- *Syntax Analysis*: Syntax analyzers (parsers) in compilers act as recognizers, determining if programs are syntactically correct.
- *Purpose*: Recognition devices, like filters, separate legal sentences from those that are incorrectly formed. They indicate whether a given string is in the language or not.

**Language Generators**
- *Generation Method*: Involves a device that generates sentences of a language.
- *Purpose*: Although less precise than recognizers, generators are easier for humans to understand and compare with program structures.
- *Usefulness*: While syntax-checking portions of compilers are useful for programmers in trial-and-error mode, generators provide a clearer understanding of the language's structure.

**Other notes and definitions**
- The lexemes of a programming language include
its numeric literals, operators, and special words, among others. One can think of programs as strings of lexemes rather than of characters
- The strings of a language are called
sentences or statements
- A token of a language is a category of its lexemes, Ex: Lexeme: + may have Token: plus_op.

## 3.3 Formal Methods of Describing Syntax

### Backus-Naur Form (BNF) and Context-Free Grammars

**Development of Formal Syntax Description**
- **Chomsky and Backus**: In the 1950s, Noam Chomsky and John Backus independently developed a syntax description formalism, which became widely used for programming language syntax.
  
**Context-Free Grammars**
- **Chomsky's Work**: Noam Chomsky, primarily a linguist, described four classes of generative devices or grammars, two of which, context-free and regular, were found useful for programming language syntax.
- **Applicability**: Context-free grammars, though initially aimed at natural languages, were later applied to programming languages due to their effectiveness in describing syntax.

**Origins of Backus-Naur Form (BNF)**
- **ALGOL 58**: The ACM-GAMM group, during the design of ALGOL 58, introduced a new formal notation for specifying programming language syntax.
- **John Backus and Peter Naur**: John Backus presented a landmark paper describing ALGOL 58 in 1959, which later influenced Peter Naur's modification for ALGOL 60, resulting in Backus-Naur Form (BNF).
- **Historical Context**: BNF's concept dates back to the syntax description used by Panini to describe Sanskrit several hundred years before Christ.

**Popularity of BNF**
- **Acceptance**: Although initially not widely accepted, BNF soon became the most popular method for concisely describing programming language syntax.
- **Equivalence with Context-Free Grammars**: BNF closely resembles Chomsky's context-free grammars, often used interchangeably in discussions of syntax description.

In subsequent discussions, BNF and grammars are used synonymously to describe programming language syntax concisely and effectively.

### 3.3.1.3 Fundamentals
**A metalanguage** is a language that is used to describe another language. **BNF** is a metalanguage for programming languages. BNF uses abstractions for syntactic structures. A simple Java assignment statement, for example, might be represented by the abstraction `<assign>`. The actual definition of `<assign>` can be given by `<assign> → <var> = <expression>`. The text on the left side of the arrow, which is aptly called the left-hand side (LHS), is the abstraction being defined. The text to the right of the arrow is the definition of the LHS, called the right-hand side (RHS), and consists of some mixture of tokens, lexemes, and references to other abstractions.

Nonterminal symbols in a BNF description, or grammar, are often called **nonterminals**, and the lexemes and tokens of the rules are called **terminals**. A BNF description, or grammar, is a collection of rules. Nonterminal symbols can have two or more distinct definitions, representing two or more possible syntactic forms in the language. Multiple definitions can be written as a single rule, with the different definitions separated by the symbol `|`, meaning logical OR. Though simple, BNF is powerful enough to describe almost all of the syntax of programming languages.

### 3.3.1.4 Describing Lists
Variable-length lists in mathematics are often written using an ellipsis (...); 1, 2, ... is an example. BNF does not include the ellipsis, so an alternative method is required for describing lists of syntactic elements in programming languages. For BNF, the alternative is recursion. A rule is recursive if its LHS appears in its RHS. Recursion is used to describe lists in many of the example grammars in the remainder of this chapter.

### 3.3.1.5 Grammars and Derivations
A grammar is a generative device for defining languages. The sentences of the language are generated through a sequence of applications of the rules, beginning with a special nonterminal of the grammar called the start symbol. This sequence of rule applications is called a derivation. In a grammar for a complete programming language, the start symbol represents a complete program. Derivations that use leftmost order of replacement are called leftmost derivations. By choosing alternative RHSs of rules with which to replace nonterminals in the derivation, different sentences in the language can be generated. However, due to the infinite nature of most languages, it's impossible to generate all sentences in finite time.

### 3.3.1.4 Describing Lists
Variable-length lists in mathematics are often written using an ellipsis (. . .); 1, 2, . . . is an example. BNF does not include the ellipsis, so an alternative method is required for describing lists of syntactic elements in programming languages (for example, a list of identifiers appearing on a data declaration statement). For BNF, the alternative is recursion. A rule is recursive if its LHS appears in its RHS. The following rules illustrate how recursion is used to describe lists:

- `<ident_list>` → `identifier`
- `<ident_list>` → `identifier, <ident_list>`

This defines `<ident_list>` as either a single token (identifier) or an identifier followed by a comma and another instance of `<ident_list>`. Recursion is used to describe lists in many of the example grammars in the remainder of this chapter.

### 3.3.1.5 Grammars and Derivations
A grammar is a generative device for defining languages. The sentences of the language are generated through a sequence of applications of the rules, beginning with a special nonterminal of the grammar called the start symbol. This sequence of rule applications is called a derivation. In a grammar for a complete programming language, the start symbol represents a complete program and is often named `<program>`. The simple grammar shown in Example 3.1 is used to illustrate derivations.

A derivation of a program in this language follows:
- `<program>` => `begin <stmt_list> end`
- `=> begin <stmt> ; <stmt_list> end`
- `=> begin <var> = <expression> ; <stmt_list> end`
- `=> begin A = <expression> ; <stmt_list> end`
- `=> begin A = <var> + <var> ; <stmt_list> end`
- `=> begin A = B + <var> ; <stmt_list> end`
- `=> begin A = B + C ; <stmt_list> end`
- `=> begin A = B + ; <stmt> end`
- `=> begin A = B + C ; <var> = <expression> end`
- `=> begin A = B + C ; B = <expression> end`
- `=> begin A = B + C ; B = <var> end`
- `=> begin A = B + C ; B = C end`

This derivation, like all derivations, begins with the start symbol, in this case `<program>`. Each successive string in the sequence is derived from the previous string by replacing one of the nonterminals with one of that nonterminal’s definitions. Each of the strings in the derivation, including `<program>`, is called a sentential form.

### 3.3.1.7 Ambiguity

- **Definition of Ambiguity:** A grammar is considered ambiguous if it can generate a sentential form (a sequence of symbols) that can be parsed into two or more distinct parse trees.

- **Example of Ambiguity:** The text illustrates an example of ambiguity in this grammar. It presents a sentence, "A = B + C * A," and mentions that it can be parsed into two distinct parse trees. This ambiguity arises because the grammar allows growth of parse trees on both the left and the right sides.

- **Implications of Ambiguity:** Ambiguity in language structures poses challenges for compilers, as they often base the semantics (meaning) of these structures on their syntactic form. Compilers determine the code to be generated for a statement by examining its parse tree. If a language structure has more than one parse tree, its meaning cannot be uniquely determined.

- **Characteristics of Ambiguous Grammars:** The passage mentions other characteristics useful in determining whether a grammar is ambiguous. These include generating sentences with more than one leftmost derivation or more than one rightmost derivation.

- **Handling Ambiguity:** While ambiguous grammars present challenges, some parsing algorithms can handle them. These parsers use additional information provided by the designer to construct the correct parse tree when encountering ambiguous constructs. In many cases, ambiguous grammars can be rewritten to be unambiguous while still generating the desired language.

### 3.3.1.8 Operator Precedence

In expressions involving multiple operators, such as x + y * z, the order of evaluation can affect the result. Assigning precedence levels to operators resolves this issue. For instance, if * has higher precedence than +, multiplication will be performed first regardless of the operators' order.

- **Parsing Ambiguity and Precedence:** Parsing trees represent syntactic structures, and the position of operators in these trees determines their precedence. However, conflicting precedence information may arise, leading to ambiguity.
  
- **Unusual Precedence:** While a grammar may not be ambiguous, its operator precedence might not follow the standard order. In such cases, operators are positioned differently in the parse tree based on their roles in expressions.

- **Resolving Precedence:** To ensure unambiguous parsing and consistent operator precedence, separate nonterminal symbols are used to represent operands with different precedence levels. This approach allows the grammar to enforce precedence rules by structuring the parse tree accordingly.

- **Derivation and Parse Trees:** Each derivation in an unambiguous grammar corresponds to a unique parse tree. Different derivations may lead to the same parse tree, demonstrating the close relationship between parse trees and derivations.

- **Notes**
  - Every derivation with an unambiguous grammar has a unique parse tree, although that tree can be represented by different derivations  
  - Grammar:
    ````html
    <assign> → <id> = <expr>
    <id> → A | B | C
    <expr> → <expr> + <term>
    | <term>
    <term> → <term> * <factor>
    | <factor>
    <factor> → ( <expr>)
    | <id>
    ````
  - Left Side Derivation: (Start first step from the left)
    ````html
    <assign> => <id> = <expr>  
    => A = <expr>  
    => A = <expr> + <term>  
    => A = <term> + <term>  
    => A = <factor> + <term>  
    => A = <id> + <term>  
    => A = B + <term>  
    => A = B + <term> * <factor>  
    => A = B + <factor> * <factor>  
    => A = B + <id> * <factor>  
    => A = B + C * <factor>  
    => A = B + C * <id>  
    => A = B + C * A  
    ````
  - Right Side Derivation: (Start first step from the right)
    ````html
    <assign> => <id> = <expr>
    => <id> = <expr> + <term>
    => <id> = <expr> + <term> * <factor>
    => <id> = <expr> + <term> * <id>
    => <id> = <expr> + <term> * A
    => <id> = <expr> + <factor> * A
    => <id> = <expr> + <id> * A
    => <id> = <expr> + C * A
    => <id> = <term> + C * A
    => <id> = <factor> + C * A
    => <id> = <id> + C * A
    => <id> = B + C * A
    => A = B + C * A
    ```` 

### 3.3.1.9 Associativity of Operators

When expressions contain operators with the same precedence (e.g., * and /), a semantic rule, known as associativity, determines their order of evaluation. For example, in the expression A / B * C, associativity specifies whether the division or multiplication operation takes precedence.

- **Implicit Associativity:** Operator associativity can be implied by the structure of a grammar. 

- **Significance of Associativity:** In most cases, associativity for addition is assumed to be left associative, consistent with mathematical principles. However, in computer arithmetic, particularly with floating-point numbers, associativity may affect accuracy and precision.

- **Challenges with Left Recursion:** Left recursion in grammar rules implies left associativity. However, it poses limitations on certain syntax analysis algorithms. Consequently, grammars often need modifications to remove left recursion, compromising the explicit specification of left associativity.

- **Right Associativity and Exponentiation:** The exponentiation operator is typically right associative in languages. To denote right associativity, right recursion can be employed in grammar rules. For instance, using rules like <factor> → <exp> ** <factor> describes exponentiation as right associative.

- **Left vs Right Recursion Examples:**
  For left recursive: Ex: \<LHS> = \<LHS> \<RHS>, while for right recursive: Ex: \<LHS> = \<RHS> \<LHS>

### 3.3.1.10 An Unambiguous Grammar for if-else

The BNF rules for a Java if-else statement initially lack clarity due to ambiguity, especially when <stmt> → <if_stmt> is included. This ambiguity becomes apparent when dealing with nested if-else constructs.

- **Resolution Approach:** To address this ambiguity, an unambiguous grammar is developed. It distinguishes between matched and unmatched statements, considering that an else clause is matched with the nearest previous unmatched then clause.

- **Unambiguous Grammar:** The grammar introduces two nonterminals, <matched> and <unmatched>, to categorize statements based on their syntactic significance. <matched> represents statements with a matching else clause, while <unmatched> represents else-less if statements.

- **Example of Unambiguous Parsing:** The unambiguous grammar ensures clarity in parsing nested if-else constructs. There's only one possible parse tree for the sentential form if (<logic_expr>) if (<logic_expr>) <stmt> else <stmt>, providing unambiguous interpretation.

### 3.3.2 Extended BNF

EBNF, or Extended Backus-Naur Form, extends the traditional BNF notation to improve readability and writability. Three common extensions in EBNF include denoting optional parts using brackets, indicating repetition with braces, and specifying multiple-choice options using parentheses and the OR operator (|).

- **Optional Parts**
Optional parts of a production rule are denoted using brackets ([]). For example, in a C if-else statement, `<statement> [else <statement>]` indicates that the else part is optional.

- **Repetition**
Repetition is indicated by braces ({}), which denote that the enclosed part can be repeated indefinitely or left out altogether. For instance, `<identifier> {, <identifier>}` describes a list of identifiers separated by commas.

- **Multiple-Choice Options**
Parentheses and the OR operator (|) are used to specify multiple-choice options. For example, `<term> → <term> (* | / | %) <factor>` represents three options for the *, /, or % operators.

These extensions enhance the descriptive power of BNF without changing its underlying capabilities. However, it's important to note that they are not terminal symbols but notational tools used in the syntactic description. If these symbols are also terminal symbols in the language being described, they can be underlined or quoted.

Some variations on EBNF have emerged, such as using a colon instead of an arrow, placing alternative RHSs on separate lines, and using different notations for optional parts and multiple-choice options. Despite the existence of a standard for EBNF (ISO/IEC 14977:1996), it's rarely used in practice.

## 3.4 Attribute Grammars

### 3.4.1 Static Semantics

Static semantics involves characteristics of programming languages that are challenging to specify with BNF or impossible to define entirely. For example, type compatibility rules, like those in Java, require additional nonterminals and rules in BNF. Static semantics concerns the legal forms of programs, such as type constraints, and can be analyzed at compile time.

### 3.4.2 Basic Concepts

- **Attributes**: Associated with grammar symbols, attributes consist of synthesized and inherited sets used to pass semantic information.
- **Semantic Functions**: Associated with grammar rules, these functions compute attribute values.
- **Predicate Functions**: Define static semantic rules and evaluate to true or false.

### 3.4.3 Attribute Grammars Defined

An attribute grammar comprises a grammar with:
- Sets of synthesized and inherited attributes for each symbol.
- Semantic functions and predicate functions associated with grammar rules.

### 3.4.4 Intrinsic Attributes

Synthesized attributes of leaf nodes with values determined outside the parse tree, like variable types retrieved from a symbol table.

### 3.4.5 Examples of Attribute Grammars

Attribute grammars are illustrated through examples. They provide a formal approach to describe and validate static semantics rules.

### 3.4.6 Computing Attribute Values

Attribute values are computed through a process of decorating the parse tree. Evaluation can't proceed in a single direction due to a mix of synthesized and inherited attributes.

### 3.4.7 Evaluation

Attribute grammars are essential for checking the static semantic rules of a language. Despite their power, large and complex attribute grammars pose challenges in writing, reading, and evaluating attribute values on large parse trees. However, they remain a commonly used tool in compiler design.

## 3.5 Dynamic Semantics

**Dynamic semantics** refers to the meaning of expressions, statements, and program units during program execution. Three common approaches to dynamic semantics are operational semantics, denotational semantics, and axiomatic semantics.

**Operational Semantics:** This approach defines the meaning of a program by specifying how its execution proceeds step by step. It focuses on the operational behavior of programs, describing how program constructs are executed and how they interact with the computational environment.
- When a programmer runs a test program to test the functionality of a construct, this is an example of an operational semantic as they determined the meaning of the construct based on the effect that it had on the machine.
- At the lowest level this can be used to determine the meaning of a program based on the precise state changes that occur whenever the program is executed.
- There are several problems associated with using this approach for complete formal semantics descriptions. For example, individual steps in execution and resulting state changes can be too numerous to derive any meaningful insights.
- Machine language and real computers aren't used, instead intermediate languages and intepreters are used.
- Operational semantics depends on programming languages of lower levels, not mathamatics like the other two.

**Denotational Semantics:** Denotational semantics assigns mathematical objects, such as sets or functions, to program constructs, representing their meanings. This approach provides a mathematical model of program behavior, where the meaning of a program is represented by the mathematical properties of the objects assigned to its components. <mark>Parse trees with denotated objects, such as binary numbers or decimal numbers, are examples of denotational semantics in action.</mark>
- Grammar for the set N. 
    ````html
    <dec_num> → '0'|'1'|'2'|'3'|'4'|'5'|'6'|'7''8'|'9'
    |<dec_num> ('0'|'1'|'2'|'3'|'4'|'5'|'6'|'7'|'8'|'9')
    ````
- Denotational semantics is defined in terms of only the values of all of the program’s variables. So,denotational semantics uses the state of the program to describe meaning
  - This is different from Operational Semantics as <mark>Denotational Semantics uses the state of the program to describe meaning</mark> instead of the state of the machine
- The key difference between operational semantics
and denotational semantics is that state changes in operational semantics are
defined by coded algorithms, written in some programming language, whereas
in denotational semantics, state changes are defined by mathematical functions.
- Based on <mark>Recursive Function Theory</mark>

**Axiomatic Semantics:** Axiomatic semantics specifies the meaning of programs by defining logical properties that hold before and after their execution. It focuses on reasoning about program behavior in terms of preconditions and postconditions. Weakest precondition is a concept used in axiomatic semantics to determine the minimal condition under which a given statement or sequence of statements will achieve a desired effect.
- Most abstract approach to semantics specification compared to other two. It specifies what can be proven about the program. (Prove the correctness of programs?)
- There is no model of the state of machine or program, or model of state changes like the other two. Instead <mark>the meaning of the program is based on relationships among program variables and constants.</mark>
- Formal approach to specifying the meaning of mrograms by defining logical properties that hold before and after their execution.
-  A fundamental concept in axiomatic semantics is the Hoare triple, which is denoted as {P} S {Q}, where:  <br><br>
    ````
    P is the precondition,
    S is the program statement or command being executed, and
    Q is the postcondition.
    ````
    The Hoare triple asserts that if the precondition P holds true before executing the statement S, then the postcondition Q will hold true after executing S.

#### <mark>Review Weakest Precondition in Textbook (Pg170):</mark>
**Weakest Preconditions (WP):**
Single Statement: For a single statement, the weakest precondition is the condition that must hold true before executing the statement to ensure that the desired postcondition holds true after execution.
Multiple Statements (Sequential Steps): For a sequence of statements executed sequentially, the weakest precondition is the condition that must hold true before executing the first statement to guarantee that the desired postcondition holds true after executing all the statements in sequence.
- It is the least restrictive precondition that will guarentee the validity of the associated post condidtion. Ex:
  ````html
    sum = 2 * x + 1 {sum > 1}
    The weakest precondidtion would be {x > 0}
  ````

# Chapter 5: Names, Bindings, and Scopes

## 5.2 Names

### 5.2.1 Design Issues
The ftwo primary design issues for names include:
- Are they case sensitive?
- Are the special words of the language. Reserved words or keyboards

### 5.2.2 Name Forms

A name is a string of characters used to identify some entity in a program.

**Length Limitations**: Different programming languages have varying rules regarding the length of names. For example, C99 allows internal names to be of any length, but only the first 63 characters are significant. External names, which are handled by the linker, are restricted to 31 characters. Java and C# have no length limit on names.

**Character Restrictions**: Most programming languages allow names to consist of letters, digits, and underscore characters. The use of underscores to form names was popular in the past but has been replaced by camel notation in many C-based languages. In camel notation, all words in a multi-word name are capitalized except the first, as in myStack.

**Special Characters**: Some languages have special rules regarding the use of special characters in names. For example, in PHP, all variable names must begin with a dollar sign. In Perl, the special characters $, @, or % at the beginning of a variable name indicate its type. In Ruby, @ or @@ at the beginning of a variable name indicates that it is an instance or class variable, respectively.

**Case Sensitivity**: In many programming languages, including C-based languages like C++, uppercase and lowercase letters in names are distinct, making names case-sensitive. This means that rose, ROSE, and Rose would be considered different names. While some people find case sensitivity detrimental to readability, others argue that it allows for distinct names to coexist.

**Writability vs. Readability**: Case sensitivity can affect both the writability (ease of writing code) and readability (ease of understanding code) of programs. In languages like Java and C#, where predefined names include both uppercase and lowercase letters, programmers need to remember specific case usage, which can make writing correct programs more challenging.

## 5.3 Variables

**Name**: A variable's name is a symbolic identifier used to refer to a memory location. In programming languages, variables are commonly named to represent the data they hold. The name attribute of a variable is essential for readability and understanding of code.

**Address**: The address of a variable refers to the memory location where its value is stored. In many languages, a variable's address can change during program execution, particularly in the case of local variables within subprograms. The address of a variable is sometimes referred to as its l-value, especially when used on the left side of an assignment operation.

**Type**: The type of a variable defines the range of values it can store and the operations that can be performed on those values. For example, an int type variable in Java can store integer values within a specific range and supports arithmetic operations like addition, subtraction, etc.

**Value**: The value of a variable represents the actual data stored in its memory location. It is the contents of the memory cell(s) associated with the variable. The value of a variable can be thought of as its r-value, especially when used on the right side of an assignment operation. Determining the r-value often involves accessing the l-value first, which can be complicated by scoping rules and other factors.

The passage also discusses the concept of aliases, which are multiple variable names that refer to the same memory location. Aliasing can occur through various mechanisms such as union types, pointer variables, reference variables, or subprogram parameters. Aliases can introduce readability issues and make program verification more challenging.

## 5.4 Binding

**Binding and Binding Times:**

- **Binding:** It refers to the association between an attribute and an entity, such as a variable and its type or value, or an operation and a symbol.
- **Binding Time:** This is the time at which a binding takes place. Bindings can occur at various stages: language design time, language implementation time, compile time, load time, link time, or run time.
  
**Type Bindings:**

- **Static Type Binding:** The type of a variable is specified explicitly through declaration statements. This binding occurs at compile time and remains fixed throughout the program's execution.
- **Dynamic Type Binding:** The type of a variable is not specified by declaration statements but is determined at runtime. Variables can be bound to different types during program execution, providing more flexibility.
  
**Storage Bindings and Lifetime:**

- **Static Variables: **Bound to memory cells before program execution begins and remain bound to the same memory cells until program termination. Efficient but less flexible.
- **Stack-Dynamic Variables:** Bound to memory cells when their declaration statements are executed during runtime. Suitable for recursive subprograms and dynamic local storage needs.
- **Explicit Heap-Dynamic Variables:** Nameless memory cells allocated and deallocated explicitly by the programmer at runtime. Accessed through pointer or reference variables. Used for dynamic structures like linked lists and trees.
- **Implicit Heap-Dynamic Variables:** Bound to heap storage only when assigned values. Highest flexibility but incurs runtime overhead and may lead to loss of some error detection by the compiler.
  
Understanding these concepts is crucial for designing efficient and reliable programs, as they determine how variables are bound to memory, what types they can hold, and how long they persist during program execution.

## 5.5 Scope

**Static Scope:**
Static scoping, also known as lexical scoping, is a method of binding names to nonlocal variables. It allows the scope of a variable to be determined statically, meaning it can be determined before execution, which simplifies program reading and compilation. In languages with nested subprograms, static scopes are created by these subprograms. When a reference is made to a variable, the program searches for its declaration starting from the current subprogram and moving up through its static ancestors until a declaration is found. This method ensures that the correct variable is referenced even in nested subprograms.

**Dynamic Scope:**
Dynamic scoping, on the other hand, determines the scope of a variable based on the calling sequence of subprograms during runtime. In dynamic scoping, the scope cannot be determined statically, and a reference to a nonlocal variable may refer to different variables during different executions of the subprogram. This can lead to less reliable programs and makes it difficult for human readers to understand the code, as they need to know the calling sequence of subprograms to determine the meaning of variable references.

**Comparison:**
Static scoping is preferred over dynamic scoping in most cases because it leads to easier-to-read, more reliable, and faster-executing programs. Dynamic scoping has some advantages, such as the implicit visibility of parameters passed from one subprogram to another, but its drawbacks often outweigh these advantages.

In summary, <mark>static scoping determines variable scope statically before execution, while dynamic scoping determines scope based on the calling sequence of subprograms during runtime. Static scoping is generally preferred for its reliability and readability, while dynamic scoping can lead to more complex and error-prone code.</mark>

## 5.6 Scope and Lifetime

In Java, when a variable is declared within a method and there are no method calls within that method, the scope of the variable is limited to the method itself. The lifetime of the variable begins when the method is entered and ends when the method execution terminates. This relationship between scope and lifetime seems straightforward and intuitive.

However, in languages like C and C++, the relationship between scope and lifetime can be more complex. For example, when a variable is declared within a function using the static keyword, its scope is limited to the function, but its lifetime extends over the entire execution of the program. This means that the variable remains allocated in memory throughout the entire execution of the program, even though its scope is local to the function.

Another scenario discussed involves subprogram calls. In the provided example of C++, the compute() function contains a variable sum, and within compute(), the printheader() function is called. While the scope of sum is limited to the compute() function and does not extend to printheader(), its lifetime continues throughout the execution of both compute() and printheader() functions. This means that the memory allocated for sum persists even while printheader() is executing.

Overall, while there may be an apparent relationship between the scope and lifetime of variables in some situations, particularly in simple cases like Java methods, this relationship can become more complex in languages like C and C++, where variables may have different storage durations and lifetimes based on their declarations and usage within the program

## 5.7 Referencing Environments

In a static-scoped language, the referencing environment of a statement consists of the variables declared within its local scope and the variables from ancestor scopes that are visible. When compiling a statement in such a language, the referencing environment is crucial for creating code and data structures that allow references to variables from other scopes during runtime. Techniques for implementing references to nonlocal variables in both static- and dynamic-scoped languages are discussed further in Chapter 10.

In Python, scopes are created by function definitions. The referencing environment of a statement includes the local variables and all variables declared in the functions in which the statement is nested, excluding variables in nonlocal scopes that are hidden by declarations in nearer functions. Each function definition creates a new scope and thus a new environment.

The provided Python skeletal program demonstrates this concept:

````python
g = 3  # A global

def sub1():
    a = 5  # Creates a local
    b = 7  # Creates another local
    # Point 1

    def sub2():
        global g  # Global g is now assignable here
        c = 9  # Creates a new local
        # Point 2

        def sub3():
            nonlocal c  # Makes nonlocal c visible here
            g = 11  # Creates a new local
            # Point 3
````
The referencing environments of the indicated program points are as follows:

- Point 1: local variables a and b (of sub1), global g for reference, but not for assignment
- Point 2: local variable c (of sub2), global g for both reference and assignment
- Point 3: nonlocal variable c (of sub2), local g (of sub3)

The referencing environment ensures that variables are accessible within the appropriate scope and context during program execution, aiding in the proper handling of variable access and manipulation.

## 5.8 Named Constraints

A named constant is a variable that is assigned a value only once and remains constant throughout the program's execution. It's used to improve readability by providing meaningful names instead of hard-coded values like numbers or strings. For example, using the name pi instead of the constant ````3.14159265```` makes the code more understandable.

Named constants are also valuable for parameterizing a program, especially when dealing with fixed values that are used in multiple places throughout the code. Instead of hard-coding the value at multiple locations, a named constant can be defined and used throughout the program. This improves reliability because if the value needs to be changed, it only needs to be updated in one place.

In languages like C++ and Java, named constants can be dynamically bound to values, allowing expressions containing variables to be assigned to constants during declaration. This flexibility enables the use of variables to define the value of a constant, as long as those variables' values are visible at the time of assignment.

C# offers two kinds of named constants: const and readonly. const constants are statically bound to values and can only be assigned literal values or other const members. In contrast, readonly constants are dynamically bound and can be assigned either during declaration or in a static constructor. The choice between const and readonly depends on whether the constant's value needs to be determined at compile time or can vary between program executions.

The discussion also touches on initialization, which is the process of binding a value to a variable either statically or dynamically. In statically bound variables, initialization occurs before runtime and requires specifying the initial value as a literal or an expression involving named constants. In dynamically bound variables, initialization can occur at runtime and allows for more flexibility in choosing initial values. Most programming languages allow initialization to be specified at the variable's declaration.

Overall, named constants and initialization play important roles in enhancing the readability, reliability, and modifiability of programs by providing meaningful names, parameterizing values, and specifying initial values for variables.

# Chapter 15: Functional Programming Languages

## 15.2 Mathematical Functions

### Named Constants:

A named constant is a variable whose value cannot be changed once it has been assigned. These constants are used to represent values that are fixed throughout the execution of a program. Here are some key aspects of named constants:

1. **Readability and Maintainability:** Using named constants instead of hard-coded values improves the readability and maintainability of code. For example, using `const int MAX_SIZE = 100;` is more expressive than scattering the value `100` throughout the code.

2. **Parameterization:** Named constants are particularly useful for parameterizing a program. Instead of using literal values, constants can be used to represent values that may need to be changed in the future. This makes it easier to modify the program without having to hunt down and change every occurrence of the value.

3. **Dynamic Binding:** Some programming languages allow named constants to be dynamically bound, meaning their values can be determined at runtime. This adds flexibility, as constants can be assigned values based on expressions involving other variables.

### Initialization:

Initialization is the process of associating an initial value with a variable when it is created. This can occur either statically (before runtime) or dynamically (at runtime). Here's a deeper look at initialization:

1. **Static Initialization:** In statically bound variables, initialization occurs before the program starts executing. This initialization is typically done using literal values or expressions involving named constants that have already been defined. Static initialization is common in languages like C++ and Java.

2. **Dynamic Initialization:** In dynamically bound variables, initialization occurs during runtime. This allows for more flexibility, as variables can be assigned values based on conditions or user input. Dynamic initialization is common in languages like Python.

3. **Role in Program Execution:** Initialization is crucial for ensuring that variables have meaningful values before they are used in the program. It sets the stage for correct program behavior and prevents errors that may arise from using uninitialized variables.

4. **Types of Initialization:** Initialization can involve simple literal values (e.g., `int x = 10;`), expressions (e.g., `int y = x * 2;`), or more complex initialization routines depending on the programming language and the nature of the variable.

### Example:

Consider a scenario where a program needs to calculate the area of a circle. Using named constants, we can define the value of pi as `const double PI = 3.14159;`. Then, during initialization, we can use this constant in the calculation: `double area = PI * radius * radius;`.

By employing named constants and proper initialization techniques, the code becomes more readable, maintainable, and reliable. Additionally, it allows for easier modification and parameterization of the program, making it adaptable to changing requirements.

## 15.3 Fundamentals of Functional Programming Languages

### Functional Programming Paradigm:
- **Objective**: Functional programming languages aim to closely resemble mathematical functions, leading to a different approach to problem-solving compared to imperative languages.
- **Memory Management**: Unlike imperative languages, where expressions are evaluated and results are stored in memory locations represented by variables, functional languages eliminate the need for variables and assignment statements. This simplifies the programming methodology by removing concerns related to program state and memory management.
- **Iterative Constructs**: Without variables, iterative constructs are not feasible in functional languages. Instead, repetition is achieved through recursion rather than iteration.
- **Referential Transparency**: Functional programming languages exhibit referential transparency, meaning that the result of executing a function remains the same given the same parameters. This simplifies testing and reasoning about code.

### Features of Functional Languages:
- **Primitive Functions**: Functional languages provide a set of primitive functions, along with functional forms to construct complex functions from these primitives.
- **Data Representation**: Functional languages utilize structures to represent data, parameters, and values computed by functions.
- **Minimalistic Design**: Well-designed functional languages require only a small number of primitive functions, emphasizing simplicity and elegance in design.

### Evolution of Functional Languages:
- **Historical Context**: Early functional languages like Lisp introduced a unique syntax for both data and code, distinct from imperative languages.
- **Hybridization**: While some languages, like Haskell, remain purely functional, many others incorporate imperative features such as mutable variables and assignment statements.
- **Cross-Pollination**: Concepts and constructs originating from functional languages, such as lazy evaluation and anonymous subprograms, have influenced imperative languages.
- **Compilation**: While early functional languages were often interpreted, modern functional languages are frequently compiled, enhancing their performance and adoption.

Overall, functional programming languages offer a distinct paradigm focused on simplicity, expressiveness, and mathematical purity, albeit often incorporating features from imperative languages to improve versatility and practicality.

## 15.5 An introduction to Scheme

### 15.5.1 and 15.5.2 Origins and Interpreter

**Origins of Scheme:** Scheme was developed at MIT in the mid-1970s as a dialect of Lisp. It is known for its simplicity, exclusive use of static scoping, and treating functions as first-class entities. Early versions of Lisp did not have all the capabilities that Scheme introduced.

**Features of Scheme:** Scheme is characterized by its simplicity, small size, and its treatment of functions as first-class entities. Functions in Scheme can be used as values of expressions, elements of lists, passed as parameters, and returned from other functions. Scheme's simplicity and typelessness make it suitable for educational purposes, such as teaching functional programming and as a general introduction to programming.

**Scheme Interpreter:** A Scheme interpreter operates in an interactive mode known as REPL (Read-Evaluate-Print Loop). It continuously reads expressions typed by the user, evaluates them, and displays the resulting value. This type of interpreter is also used by other languages like Ruby and Python. Expressions in Scheme are interpreted using the EVAL function. Literals evaluate to themselves (e.g., typing a number displays the number). Expressions that are calls to primitive functions are evaluated by first evaluating each parameter expression and then applying the primitive function to the parameter values.

**Loading and Interpreting Scheme Programs:** Scheme programs stored in files can be loaded and interpreted.

**Comments in Scheme:** Comments in Scheme are any text following a semicolon on any line.

### 15.5.3 Primitive Numeric Functions

Scheme includes primitive functions for basic arithmetic operations such as addition, subtraction, multiplication, and division. Here's how they work:

**Examples:**
```scheme
(+ 3 4) ; Addition: returns 7
(- 10 5) ; Subtraction: returns 5
(* 3 7) ; Multiplication: returns 21
(/ 10 2) ; Division: returns 5
```
In Scheme, these functions can take multiple parameters and perform the corresponding arithmetic operation.

### 15.5.4 Defining Functions

Defining functions in Scheme is crucial for programming. Let's explore how to define functions using named and nameless approaches:

**Named Function Example:**
```scheme
(define (square number) (* number number)) ; Defining a function to square a number

(square 5) ; Calling the square function with argument 5: returns 25
```

**Nameless Function (Lambda Expression) Example:**
```scheme
((lambda (x) (* x x)) 7) ; Applying a nameless function to square a number: returns 49
```
In this example, `lambda` defines an anonymous function that squares its argument `x`, which is then applied to the argument `7`.

### 15.5.5 Output Functions

Scheme includes simple output functions, but output in an interactive interpreter primarily displays results directly. Explicit input/output is not typically part of the pure functional programming model.

### 15.5.6 Numeric Predicate Functions

Predicate functions in Scheme return Boolean values. Scheme provides various numeric predicate functions:

**Examples**:
```scheme
(= 5 5) ; Equal: returns #t (true)
(> 10 5) ; Greater than: returns #t
(< 3 2) ; Less than: returns #f (false)
(even? 6) ; Is it even?: returns #t
(odd? 3) ; Is it odd?: returns #t
(zero? 0) ; Is it zero?: returns #t
```
These functions return `#t` for true and `#f` for false.

### 15.5.7 Control Flow

Scheme offers control flow constructs similar to imperative languages, including `if`, `cond`, and recursion for repetition. Here's how they work:

**`if` Example:**
```scheme
(define (factorial n)
  (if (<= n 1)
      1
      (* n (factorial (- n 1)))))
```
This `factorial` function computes the factorial of a number using recursion and the `if` construct for conditionals.

**`cond` Example:**
```scheme
(define (leap? year)
  (cond
    ((zero? (modulo year 400)) #t)
    ((zero? (modulo year 100)) #f)
    (else (zero? (modulo year 4)))))
```
This `leap?` function determines if a given year is a leap year using the `cond` construct.

### 15.5.8 List Functions in Scheme

Scheme, a dialect of Lisp, is known for its powerful list processing capabilities. Let's explore some of the key list functions and their implementation in Scheme.

### 15.5.9 QUOTE Function

The `QUOTE` function is fundamental in Scheme as it allows you to treat data as literal expressions without evaluating them. Here's how it works:

**Examples:**
- `(QUOTE A)` returns `A`
- `(QUOTE (A B C))` returns `(A B C)`

You can use an apostrophe `'` as shorthand for `QUOTE`, so `(QUOTE (A B))` can be written as `'(A B)`.

### 15.5.10 CAR, CDR, and CONS Functions

In Scheme, `CAR` and `CDR` are used to extract the first element and the rest of the elements from a list, respectively. `CONS` is used to construct a new list from two given list parts.

**Examples:**
- `(CAR '(A B C))` returns `A`
- `(CDR '(A B C))` returns `(B C)`
- `(CONS 'A '(B C))` returns `(A B C)`

### 15.5.11 Predicate Functions: EQ?, NULL?, and LIST?

Predicate functions in Scheme are used to test conditions. `EQ?` checks for equality, `NULL?` checks for an empty list, and `LIST?` checks if an object is a list.

**Examples:**
- `(EQ? 'A 'A)` returns `#T`
- `(NULL? '())` returns `#T`
- `(LIST? '(X Y))` returns `#T`

### 15.5.12 Example Scheme Functions

Let's look at examples of functions in Scheme that solve list-processing problems:

**Member Function**
The `member` function checks if a given atom is present in a given list.

```scheme
(DEFINE (member atm a_list)
 (COND
   ((NULL? a_list) #F)
   ((EQ? atm (CAR a_list)) #T)
   (ELSE (member atm (CDR a_list)))
 ))
```

**Equal Function**
The `equal` function checks if two lists are equal.

```scheme
(DEFINE (equal list1 list2)
 (COND
   ((NOT (LIST? list1)) (EQ? list1 list2))
   ((NOT (LIST? list2)) #F)
   ((NULL? list1) (NULL? list2))
   ((NULL? list2) #F)
   ((equal (CAR list1) (CAR list2))
    (equal (CDR list1) (CDR list2)))
   (ELSE #F)
 ))
```

### 15.5.13 LET Function

The `LET` function creates a local scope where names are bound to values of expressions temporarily.

**Example:**
```scheme
(DEFINE (quadratic_roots a b c)
 (LET (
   (root_part_over_2a (/ (SQRT (- (* b b) (* 4 a c))) (* 2 a)))
   (minus_b_over_2a (/ (- 0 b) (* 2 a)))
   )
 (LIST (+ minus_b_over_2a root_part_over_2a)
       (- minus_b_over_2a root_part_over_2a))
 ))
```

### 15.5.14 Tail Recursion in Scheme

Tail recursion is a technique used in Scheme to optimize recursive functions where the recursive call is the last operation.

**Example: Member Function (Tail Recursive)**

```scheme
(DEFINE (member atm a_list)
 (COND
   ((NULL? a_list) #F)
   ((EQ? atm (CAR a_list)) #T)
   (ELSE (member atm (CDR a_list)))
 ))
```

### 15.5.15 Functional Forms

Scheme provides powerful functional forms like composition and apply-to-all.

**Functional Composition**

Functional composition creates a new function by combining two functions.

```scheme
(DEFINE (compose f g) (LAMBDA (x)(f (g x))))
```

**Apply-to-All Function**

The `map` function applies a given function to each element of a list and returns a list of results.

**Example:**
```scheme
(DEFINE (map fun a_list)
 (COND
   ((NULL? a_list) '())
   (ELSE (CONS (fun (CAR a_list)) (map fun (CDR a_list))))
 ))
```

### 15.5.16 Functions That Build Code

Scheme allows functions to create and evaluate code dynamically using the `EVAL` function.

**Example: Adder Function**

The `adder` function dynamically constructs a call to `+` with the proper parameters and evaluates it.

```scheme
(DEFINE (adder a_list)
 (COND
   ((NULL? a_list) 0)
   (ELSE (EVAL (CONS '+ a_list)))
 ))
``` 

These functions and forms demonstrate the flexibility and power of Scheme in list processing and functional programming.