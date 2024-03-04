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
   - Compilation involves translating the entire source code of a program into machine code or bytecode before execution. This process typically involves several stages, including lexical analysis, parsing, optimization, and code generation. The resulting compiled code is then executed directly by the computer's hardware.

2. **Pure Interpretation:**
   - In pure interpretation, the source code of a program is executed line-by-line or statement-by-statement by an interpreter. The interpreter reads each instruction, translates it into machine code or intermediate code, and executes it immediately. This approach does not produce an intermediate compiled form, resulting in slower execution compared to compilation.

3. **Hybrid:**
   -  Hybrid implementation methods combine elements of both compilation and interpretation. Typically, the source code is initially compiled into an intermediate representation or bytecode. This bytecode is then executed by a virtual machine or interpreter. This approach offers a balance between the performance benefits of compilation and the flexibility of interpretation.

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
