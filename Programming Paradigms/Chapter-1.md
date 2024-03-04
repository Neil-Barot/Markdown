# Table of Contents
- [Table of Contents](#table-of-contents)
- [Chapter 1: Preliminaries](#chapter-1-preliminaries)
  - [1.1: Reasons for Studying Concepts of Programming Languages](#11-reasons-for-studying-concepts-of-programming-languages)
    - [Increased Capacity to express ideas:](#increased-capacity-to-express-ideas)
    - [Improved Background for choosing appropriate languages](#improved-background-for-choosing-appropriate-languages)
    - [Increased Ability to learn a new language](#increased-ability-to-learn-a-new-language)
    - [Better use of languages that are already known](#better-use-of-languages-that-are-already-known)
    - [Overall advancement of computing](#overall-advancement-of-computing)
  - [1.2 Programming Domains](#12-programming-domains)
    - [**Might have talked about these in class:**](#might-have-talked-about-these-in-class)
    - [**In the textbook *know these!!!***:](#in-the-textbook-know-these)
  - [1.3 Language Evaluation Criteria](#13-language-evaluation-criteria)
    - [Criteria Definitions](#criteria-definitions)
  - [1.4 Influences on Language Design](#14-influences-on-language-design)
    - [Computer Architecture](#computer-architecture)
    - [Programming Design Methodologies](#programming-design-methodologies)

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
1. **Scientific Applications:** Utilizing programming to solve scientific problems, such as mathematical modeling, simulations, and data analysis in fields like physics, biology, and chemistry.

2. **Business Applications:** Developing software to support business processes and operations, including enterprise resource planning (ERP), customer relationship management (CRM), and inventory management systems.

3. **Artificial Intelligence:** Creating intelligent systems and algorithms that can mimic human intelligence, including machine learning, natural language processing, computer vision, and robotics.

4. **Systems Programming:** Writing low-level software to manage hardware resources and interact with the operating system, often used in areas like operating systems development, device drivers, and embedded systems.

5. **Web Software:** Building applications and services for the web, including websites, web applications, e-commerce platforms, and content management systems (CMS).

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

## 1.4 Influences on Language Design

### Computer Architecture
The design of programming languages is heavily influenced by factors such as computer architecture and programming methodologies. The von Neumann architecture, which has been prevalent in computers since the 1940s, plays a significant role in shaping imperative languages. These languages emphasize variables, assignment statements, and iterative forms of repetition, reflecting the pipelining operation between memory and the CPU in von Neumann computers.

The fetch-execute cycle is a fundamental process in von Neumann architecture, where instructions are fetched from memory and executed in the CPU. Imperative languages are well-suited for this architecture due to their efficient handling of variables and iterative operations.

Functional languages, on the other hand, prioritize the application of functions to parameters and often lack variables, assignment statements, and iteration. While functional languages like Scheme offer benefits, they may not displace imperative languages until non-von Neumann computers are developed to efficiently execute functional programs.

Despite the structural alignment of imperative languages with machine architecture, some argue for the naturalness of imperative languages over functional ones. They believe that even if functional programs were as efficient, imperative languages would still dominate due to perceived ease of use.

Overall, the design of programming languages is intricately linked to the underlying computer architecture and the preferences of language users.

### Programming Design Methodologies

During the late 1960s and early 1970s, the structured-programming movement spurred an in-depth analysis of software development processes and programming language design. This shift was driven by the increasing prominence of software development costs as hardware costs decreased, and as computers tackled larger and more complex tasks.

New methodologies emerged, such as top-down design and stepwise refinement, aimed at improving programmer productivity and tackling complex problems more effectively. In this era, concerns were raised about deficiencies in programming languages, particularly regarding type checking and control statements.

By the late 1970s, there was a shift towards data-oriented program design methodologies, which emphasized data design and abstract data types. Data abstraction became a key aspect of software system design, supported by languages like SIMULA 67, albeit in a limited capacity initially. However, the benefits of data abstraction became more widely recognized in the early 1970s, leading to its adoption in most languages designed thereafter.

The evolution continued into the early 1980s with the emergence of object-oriented design, which builds upon data abstraction by incorporating concepts like inheritance and dynamic method binding. Object-oriented programming languages like Smalltalk introduced these concepts, which have since become integral parts of popular imperative languages such as Java, C++, and C#. Object-oriented concepts have also influenced other paradigms, including functional and logic programming.

Despite the dominance of data-oriented methods, procedure-oriented programming has not been abandoned. Recent research has focused on concurrency, leading to the development of language features to support concurrent programming units, as seen in languages like Java and C#.

Overall, these evolutionary steps in software development methodologies have led to the introduction of new language constructs to support them, reflecting the continuous evolution of programming languages.