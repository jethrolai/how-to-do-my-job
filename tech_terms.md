# Software Engineering Jargons and Definitions


## 1NF First Normal Form
    - No column has dividable/atomic data. (City: NYC,SF) violates the 1NF. 
    - Technically, city1, city2 columns do not violate 1NF but conceptually, the rule is violated. 
## 2NF Second Normal Form
    - Must be in 1NF
    - In the case of composite primary key, a non-attribute depends only on the partial primary key. 
## 3NF Third Normal Form
    - Must be in 2NF
    - No transitive dependency. e.g. bank_id (non primary key), bank_name (another non primary key). The bank name should be moved to a bank table with id and name. 
## 3.5NF BCNF ????
## [Agile Software Development Manifesto](http://agilemanifesto.org/)
#### Goals
    - Individuals and interactions              >>>> processes and tools    
    - Working software                          >>>> comprehensive documentation
    - Customer collaboration                    >>>> contract negotiation
    - Responding to change                      >>>> following a plan
#### [Principles](http://agilemanifesto.org/principles.html)
    - Customer satisfaction
    - Welcome changing requirements
    - Frequent cycles of delivery
    - Stakeholder collaboration
    - Culture of trust, support & motivation
    - Fact-to-face communication
    - Working software is the metric
    - Sustainable development
    - Technical excellence
    - Simplicity
    - Self organizatng teams
    - Team reflection
## atoi
    - A function in C. It means ASCII to integer.
## Backtracking
    - An algorithmic technique. Solving segments where the final result is combination of the solved segments. 
## Bloom Filter
    - space optimized alternative to hash table
    - false positive rate
        - when negative, true negative
        - when positive, probably positive but not guarantee. 
    - multiple hash functions to define a set of positions for storing the flags (bits). 
    - when all flgas are true, the value exists. 
## CAP Theorem
    - a.k.a **Brewer's theorem**
    - Consistency, Availability, Partition Torlerance
    - It's only possible to fulfill at most two of them. 
## Constrained programming
    - In nested blocks/loops, more restrictions are added each level to reduce the iterations. 
## COP 
    - Component Oriented Programming
## CSRF
    - Cross-Site Request Forgery
## CTE
    - Common Table Expression in SQL. Basically, temp table as a result of a sub query 
    - https://www.essentialsql.com/introduction-common-table-expressions-ctes/
## Dutch National Flag Program
    - Sorting algorithm: 3 way partitions
## Elixir
    - A dynamic functional programming language running on Erlang VM
## External sorting
    - sorting when the input cannot fit in the memory. 
## Go
    - Golang, a programming language
## Julia
    - A programming language
## JWT
    - JSON Web Token
    - Storing authentication information in the frontend environment. Commonly in local or session storage but cookies can works too. 
## Kadane’s Algorithm
    - linear algorithm for finding the max sum of a subarray of an array. 
    - https://www.geeksforgeeks.org/largest-sum-contiguous-subarray/
## ML
    - Machine Learning
## MMF
    - Minimum Marketable Feature
## MMP
    - Minimum Marketable Product
## Morris Traversal
    - https://www.educative.io/edpresso/what-is-morris-traversal
    - Space O(0) traversal algorithm
## MVP
    - Minimum Viable Product
    - Not to get confused with MMP or MMF.
## NLP
    - Natural Language Processing
## OOP
    - Object oriented programming
## Rust
    - A programming language
## Side effect
    - When a function does something else other than its original intention or something the name does not imply. 
## Strobogrammatic Number
    - A strobogrammatic number is a number that looks the same when rotated 180 degrees (looked at upside down).
## Structural programming
    - Control structure —> like what it reads, the code structure that controls the program/executions. 
        - Sequence —> just one instruction to another
        - Selection —> if/else/switch
        - Iteration/repetition —> while/for
        - Branching —> goto. Should not be used. This is an uncontrolled structure. 
    - Edsger Dijkstra’s rules of structured programming
        - Every function and every block should have one entry and one exit. 
        - Only one return in one function. 
        - No break or continue statements in a loop. 
        - Never, ever any goto statements. 
## Temporal coupling
    - when code is dependent on time in some way
## Floyd's Tortoise and Hare
    - using two pointers moving in two different speeds to detect cycle. 

[ Unsorted ] 
## Message Broker
    - A message broker (also known as an integration broker or interface engine[1]) is an intermediary computer program module that translates a message from the formal messaging protocol of the sender to the formal messaging protocol of the receiver. 
  - RabbitMQ, Kafka (designed by LinkedIn, now under Apache), ActiveMQ, Kestrel
## Thyemleaf
    - a modern server-side Java template engine for both web and standalone environments. Sort of like JSP (JavaServer Page)
## Synchronization primitives
    - [_mutex_ and _semaphore_](https://www.geeksforgeeks.org/mutex-vs-semaphore/#_=_)
## Atomicity
    - unbreakability
## Critical section
    - a critical section is group of instructions/statements or region of code that need to be executed atomically. Common solution: acquire lock, process critical section, release lock
## RSocket
    - Application protocol providing Reactive Streams semantics
## CSRF
    - Cross-site Request Forgery
## ES6
    - ECMAScript6, ECMA Script 2015, JavaScript6
## IIFE
    - Immediately Invoked Function Expression a.k.a Self-Executing Anonymous Function in JavaScript. Basically an anonymous function that runs immediately after it's defined. 
    - https://flaviocopes.com/javascript-iife/
## HOC
    - or HoC, Higher-Order Componenet. React technique. Kind of like interface with defaults in Java. 
## Protocol Buffers
    - a.k.a. protobuffa. A language and platform neutral mechanism for serialization and deserialization of structured data, which is proclaimed by Google, its creator, to be much faster, smaller and simpler than other types of payloads, such as XML and JSON, say, binary-based message payload.
