# Fundamental of Computer - Active Tag Questions (172-250)

## Searching Algorithms (172)

**Q172: Explain searching algorithms (linear, binary).**

**Answer:**
- **Linear Search**: Sequentially checks each element in a list until the target is found or the end is reached. Time complexity: O(n)
- **Binary Search**: Works on sorted arrays by repeatedly dividing the search interval in half. Time complexity: O(log n)

---

## Heap Data Structure (173)

**Q173: What is a heap?**

**Answer:**
A heap is a specialized tree-based data structure that satisfies the heap property:
- **Max Heap**: Parent nodes are always greater than or equal to child nodes
- **Min Heap**: Parent nodes are always less than or equal to child nodes
- Used for priority queues and heap sort algorithm

---

## Priority Queue (174)

**Q174: Define priority queue.**

**Answer:**
A priority queue is an abstract data type where each element has a priority associated with it:
- Elements with higher priority are dequeued before elements with lower priority
- Can be implemented using heaps, arrays, or linked lists
- Common operations: insert, delete, peek

---

## Trie Data Structure (175)

**Q175: What is a trie?**

**Answer:**
A trie (prefix tree) is a tree-like data structure used to store strings:
- Each node represents a character
- Paths from root to leaf nodes represent complete strings
- Efficient for prefix-based searches and autocomplete functionality
- Space complexity: O(ALPHABET_SIZE × N × M) where N is number of strings, M is average length

---

## Computer Security (176)

**Q176: What is computer security?**

**Answer:**
Computer security is the protection of computer systems and networks from:
- Information theft
- Damage to hardware/software
- Disruption of services
- Unauthorized access
- Involves confidentiality, integrity, and availability (CIA triad)

---

## Malware Types (177)

**Q177: Define malware, virus, worm, and Trojan.**

**Answer:**
- **Malware**: Malicious software designed to harm systems
- **Virus**: Self-replicating code that attaches to legitimate programs
- **Worm**: Self-replicating malware that spreads across networks
- **Trojan**: Malicious software disguised as legitimate software

---

## Phishing (178)

**Q178: What is phishing?**

**Answer:**
Phishing is a cyber attack where attackers impersonate legitimate entities to:
- Steal sensitive information (passwords, credit card details)
- Install malware
- Gain unauthorized access
- Methods include fake emails, websites, and social engineering

---

## Social Engineering (179)

**Q179: Explain social engineering.**

**Answer:**
Social engineering manipulates people into:
- Revealing confidential information
- Performing actions that compromise security
- Bypassing security measures
- Techniques include pretexting, baiting, quid pro quo, and tailgating

---

## SSL/TLS Encryption (180)

**Q180: What is SSL/TLS encryption?**

**Answer:**
- **SSL (Secure Sockets Layer)**: Protocol for secure communication over networks
- **TLS (Transport Layer Security)**: Successor to SSL, more secure
- Provides encryption, authentication, and integrity
- Used for HTTPS, secure email, and VPN connections

---

## Firewall and IDS/IPS (181)

**Q181: Define firewall and IDS/IPS.**

**Answer:**
- **Firewall**: Network security device that monitors and controls incoming/outgoing traffic
- **IDS (Intrusion Detection System)**: Monitors network traffic for suspicious activity
- **IPS (Intrusion Prevention System)**: Actively blocks detected threats

---

## Access Control Lists (182)

**Q182: What are access control lists (ACL)?**

**Answer:**
ACLs are security policies that:
- Define which users or processes can access specific resources
- Specify permissions (read, write, execute)
- Control access to files, directories, networks, and databases
- Can be implemented at file system, network, or application level

---

## Authentication vs Authorization (183)

**Q183: Explain user authentication vs authorization.**

**Answer:**
- **Authentication**: Verifies user identity (who you are)
  - Methods: passwords, biometrics, tokens, certificates
- **Authorization**: Determines user permissions (what you can do)
  - Based on user roles, groups, or individual permissions

---

## Two-Factor Authentication (184)

**Q184: What is two-factor authentication?**

**Answer:**
Two-factor authentication (2FA) requires two different verification methods:
- **Something you know**: Password, PIN
- **Something you have**: Phone, hardware token, smart card
- **Something you are**: Biometric (fingerprint, face recognition)
- Significantly improves security by adding an extra layer

---

## Digital Signature (185)

**Q185: Define digital signature.**

**Answer:**
A digital signature is a mathematical scheme that:
- Verifies the authenticity of digital messages or documents
- Ensures message integrity (no tampering)
- Provides non-repudiation (sender cannot deny sending)
- Uses public key cryptography (private key to sign, public key to verify)

---

## Public Key Infrastructure (186)

**Q186: What is public key infrastructure (PKI)?**

**Answer:**
PKI is a framework that manages digital certificates and public key encryption:
- **Certificate Authority (CA)**: Issues and validates digital certificates
- **Registration Authority (RA)**: Verifies certificate requests
- **Certificate Repository**: Stores and distributes certificates
- **Certificate Revocation List (CRL)**: Lists revoked certificates

---

## Ethical Hacking (187)

**Q187: Explain ethical hacking.**

**Answer:**
Ethical hacking involves authorized security testing to:
- Identify vulnerabilities in systems
- Assess security posture
- Improve security measures
- Follow responsible disclosure practices
- Requires proper authorization and documentation

---

## Vulnerability Assessment vs Penetration Testing (188)

**Q188: What is vulnerability assessment vs penetration testing?**

**Answer:**
- **Vulnerability Assessment**: 
  - Identifies and quantifies security vulnerabilities
  - Non-intrusive scanning and analysis
  - Provides risk ratings and remediation recommendations
  
- **Penetration Testing**:
  - Actively exploits vulnerabilities to prove they exist
  - Simulates real-world attacks
  - Provides detailed attack scenarios and impact assessment

---

## Patch Management (189)

**Q189: Define patch management.**

**Answer:**
Patch management is the process of:
- Identifying available software updates and security patches
- Testing patches in controlled environments
- Deploying patches to production systems
- Monitoring for patch success and rollback if needed
- Maintaining an inventory of patched systems

---

## GDPR (190)

**Q190: What is GDPR?**

**Answer:**
GDPR (General Data Protection Regulation) is a European Union regulation that:
- Protects personal data and privacy of EU citizens
- Gives individuals control over their personal data
- Requires organizations to implement data protection measures
- Imposes penalties for non-compliance
- Applies to any organization processing EU citizen data

---

## Data Privacy vs Data Protection (191)

**Q191: Explain data privacy vs data protection.**

**Answer:**
- **Data Privacy**: 
  - Focuses on individual rights and control over personal data
  - Includes consent, purpose limitation, and data minimization
  
- **Data Protection**:
  - Focuses on technical and organizational security measures
  - Includes encryption, access controls, and breach prevention

---

## Cyber Law (192)

**Q192: What is cyber law?**

**Answer:**
Cyber law encompasses legal frameworks that:
- Govern digital activities and electronic communications
- Address cybercrime, data protection, and intellectual property
- Define rights and responsibilities in cyberspace
- Varies by jurisdiction and evolves with technology

---

## Intellectual Property in Software (193)

**Q193: Define intellectual property in software.**

**Answer:**
Software intellectual property includes:
- **Copyright**: Protects source code and creative expression
- **Patents**: Protects novel and non-obvious software inventions
- **Trade Secrets**: Protects confidential algorithms and processes
- **Trademarks**: Protects software names and logos

---

## Software Licenses (194)

**Q194: What are software licenses (GPL, MIT, Apache)?**

**Answer:**
- **GPL (GNU General Public License)**: 
  - Copyleft license requiring derivative works to also be open source
  - Ensures software freedom and sharing
  
- **MIT License**: 
  - Permissive license allowing commercial use with minimal restrictions
  
- **Apache License**: 
  - Permissive license with patent protection and contributor agreements

---

## Acceptable Use Policy (195)

**Q195: Explain acceptable use policy (AUP).**

**Answer:**
An AUP defines:
- Acceptable and unacceptable use of IT resources
- User responsibilities and prohibited activities
- Consequences of policy violations
- Security requirements and best practices
- Applies to employees, contractors, and system users

---

## Digital Rights Management (196)

**Q196: What is digital rights management (DRM)?**

**Answer:**
DRM is technology that:
- Controls access to digital content and media
- Prevents unauthorized copying and distribution
- Manages licensing and usage rights
- Protects intellectual property of content creators
- Examples: streaming services, e-books, software licensing

---

## Insider Threat (197)

**Q197: Define insider threat.**

**Answer:**
Insider threats come from:
- Current or former employees
- Contractors or business partners
- Individuals with authorized access to systems
- May be malicious (intentional) or accidental (negligence)
- Often more dangerous than external threats due to access privileges

---

## Ransomware (198)

**Q198: What is ransomware?**

**Answer:**
Ransomware is malicious software that:
- Encrypts victim's files or entire system
- Demands payment (ransom) for decryption key
- Spreads through phishing, malicious downloads, or vulnerabilities
- Can cause significant business disruption and data loss
- Prevention includes backups, updates, and user training

---

## Backup Encryption (199)

**Q199: Explain backup encryption.**

**Answer:**
Backup encryption protects backup data by:
- Converting data into unreadable format using encryption algorithms
- Requiring decryption keys to restore data
- Protecting against unauthorized access to backup files
- Ensuring data confidentiality even if backups are compromised
- Essential for compliance and data protection regulations

---

## Security Audit (200)

**Q200: What is security audit?**

**Answer:**
A security audit is a systematic evaluation that:
- Reviews security policies and procedures
- Identifies security vulnerabilities and risks
- Assesses compliance with security standards
- Provides recommendations for improvement
- May be internal, external, or third-party conducted

---

## Procedural Programming (201)

**Q201: What is procedural programming?**

**Answer:**
Procedural programming is a programming paradigm that:
- Organizes code into procedures or functions
- Follows a top-down approach
- Emphasizes procedure calls and data flow
- Uses structured programming constructs
- Examples: C, Pascal, FORTRAN

---

## Object-Oriented Programming (202)

**Q202: Define object-oriented programming.**

**Answer:**
Object-oriented programming (OOP) is a paradigm that:
- Organizes code into objects containing data and methods
- Emphasizes encapsulation, inheritance, and polymorphism
- Models real-world entities and relationships
- Promotes code reusability and maintainability
- Examples: Java, C++, Python, C#

---

## Encapsulation (203)

**Q203: What is encapsulation?**

**Answer:**
Encapsulation is an OOP principle that:
- Bundles data and methods that operate on that data within a single unit (class)
- Hides internal implementation details from external code
- Provides controlled access through public interfaces
- Protects data integrity and prevents unauthorized access
- Achieved through access modifiers (public, private, protected)

---

## Inheritance (204)

**Q204: Explain inheritance.**

**Answer:**
Inheritance allows a class to:
- Inherit properties and methods from a parent/superclass
- Create a hierarchy of related classes
- Promote code reuse and establish "is-a" relationships
- Override or extend parent class functionality
- Support single and multiple inheritance (depending on language)

---

## Polymorphism (205)

**Q205: What is polymorphism?**

**Answer:**
Polymorphism allows objects to:
- Take multiple forms or behave differently based on context
- Implement the same interface in different ways
- Support method overriding and overloading
- Enable flexible and extensible code design
- Types: compile-time (overloading) and runtime (overriding)

---

## Abstraction (206)

**Q206: Define abstraction.**

**Answer:**
Abstraction is the process of:
- Hiding complex implementation details
- Showing only essential features to users
- Creating simplified models of complex systems
- Reducing complexity and improving maintainability
- Examples: abstract classes, interfaces, and method signatures

---

## Class vs Object (207)

**Q207: What is a class vs object?**

**Answer:**
- **Class**: 
  - Blueprint or template that defines structure and behavior
  - Contains attributes (data) and methods (functions)
  - Exists at design time
  
- **Object**: 
  - Instance of a class created at runtime
  - Contains actual data values
  - Can interact with other objects

---

## Function vs Method (208)

**Q208: Explain function vs method.**

**Answer:**
- **Function**: 
  - Standalone code block that performs a specific task
  - Not associated with any object or class
  - Can be called independently
  
- **Method**: 
  - Function that belongs to a class or object
  - Can access object's data and other methods
  - Called on specific object instances

---

## Variables and Data Types (209)

**Q209: What are variables and data types?**

**Answer:**
- **Variables**: Named storage locations that hold data values
- **Data Types**: Define the kind of data a variable can store
  - **Primitive**: int, float, boolean, char
  - **Reference**: objects, arrays, strings
  - **User-defined**: custom classes and structures

---

## Control Flow (210)

**Q210: What is control flow?**

**Answer:**
Control flow determines the order in which:
- Program statements are executed
- Decisions are made (conditional statements)
- Loops are repeated
- Functions are called
- Programs respond to different conditions and inputs

---

## Conditional Statements (211)

**Q211: Define conditional statements.**

**Answer:**
Conditional statements allow programs to:
- Make decisions based on conditions
- Execute different code blocks based on true/false evaluations
- Use if, if-else, if-else-if, and switch statements
- Control program execution flow
- Support nested conditions and logical operators

---

## Loops (212)

**Q212: Explain loops (for, while, do-while).**

**Answer:**
- **For Loop**: 
  - Executes code block a specific number of times
  - Uses initialization, condition, and increment/decrement
  
- **While Loop**: 
  - Repeats code block while condition is true
  - Condition checked before execution
  
- **Do-While Loop**: 
  - Executes code block at least once
  - Condition checked after execution

---

## Exception Handling (213)

**Q213: What is exception handling?**

**Answer:**
Exception handling manages runtime errors by:
- Catching and responding to unexpected program conditions
- Using try-catch blocks to handle errors gracefully
- Providing fallback behavior or error recovery
- Preventing program crashes and improving reliability
- Supporting custom exception types and error logging

---

## Compilation vs Interpretation (214)

**Q214: Define compilation vs interpretation.**

**Answer:**
- **Compilation**: 
  - Converts entire source code to machine code before execution
  - Faster execution, but slower development cycle
  - Examples: C, C++, Java
  
- **Interpretation**: 
  - Translates and executes code line by line at runtime
  - Slower execution, but faster development cycle
  - Examples: Python, JavaScript, PHP

---

## Library vs Framework (215)

**Q215: What is a library vs framework?**

**Answer:**
- **Library**: 
  - Collection of reusable functions and classes
  - Developer calls library functions as needed
  - Provides specific functionality without controlling program flow
  
- **Framework**: 
  - Provides structure and architecture for applications
  - Controls program flow and calls developer code
  - Implements inversion of control principle

---

## RESTful API (216)

**Q216: Explain RESTful API.**

**Answer:**
RESTful API (Representational State Transfer) is an architectural style that:
- Uses HTTP methods (GET, POST, PUT, DELETE)
- Treats resources as URLs
- Is stateless and cacheable
- Provides uniform interface
- Supports multiple data formats (JSON, XML)
- Follows REST principles for web services

---

## Event-Driven Programming (217)

**Q217: What is event-driven programming?**

**Answer:**
Event-driven programming is a paradigm where:
- Program flow is determined by events (user actions, sensor outputs, messages)
- Code responds to events through event handlers or callbacks
- Supports asynchronous and non-blocking operations
- Common in GUI applications, web development, and IoT systems
- Examples: JavaScript, Node.js, event-driven frameworks

---

## Callback and Promise (218)

**Q218: Define callback and promise (in JavaScript).**

**Answer:**
- **Callback**: 
  - Function passed as argument to another function
  - Executed when specific event occurs
  - Can lead to callback hell in complex scenarios
  
- **Promise**: 
  - Object representing eventual completion of asynchronous operation
  - Has three states: pending, fulfilled, rejected
  - Provides better error handling and chaining than callbacks

---

## Concurrency vs Parallelism (219)

**Q219: What is concurrency vs parallelism?**

**Answer:**
- **Concurrency**: 
  - Multiple tasks making progress over time
  - Tasks may not run simultaneously
  - Achieved through time-sharing and context switching
  
- **Parallelism**: 
  - Multiple tasks executing simultaneously
  - Requires multiple processors or cores
  - Achieves true simultaneous execution

---

## Deadlock in Concurrent Programs (220)

**Q220: Explain deadlock in concurrent programs.**

**Answer:**
Deadlock occurs when two or more processes:
- Wait indefinitely for resources held by other processes
- Create circular dependency for resource allocation
- Require all four conditions: mutual exclusion, hold and wait, no preemption, circular wait
- Can be prevented through resource ordering, timeouts, or deadlock detection

---

## Memoization (221)

**Q221: What is memoization?**

**Answer:**
Memoization is an optimization technique that:
- Caches results of expensive function calls
- Returns cached results for repeated inputs
- Improves performance by avoiding redundant calculations
- Trades memory for computation time
- Commonly used in dynamic programming and recursive algorithms

---

## Dynamic Programming (222)

**Q222: Define dynamic programming.**

**Answer:**
Dynamic programming is an optimization method that:
- Breaks complex problems into simpler subproblems
- Stores solutions to subproblems to avoid recomputation
- Builds optimal solutions from bottom up
- Applies to problems with overlapping subproblems and optimal substructure
- Examples: Fibonacci sequence, shortest path, knapsack problem

---

## Greedy Algorithm (223)

**Q223: What is greedy algorithm?**

**Answer:**
A greedy algorithm:
- Makes locally optimal choice at each step
- Assumes local optimal choices lead to global optimal solution
- Is simple and efficient but may not always find optimal solution
- Works well for problems with greedy choice property
- Examples: Huffman coding, Dijkstra's algorithm, activity selection

---

## Backtracking (224)

**Q224: Explain backtracking.**

**Answer:**
Backtracking is an algorithmic technique that:
- Builds solutions incrementally
- Abandons partial solutions that cannot lead to valid solution
- Uses depth-first search with pruning
- Is useful for constraint satisfaction problems
- Examples: N-queens problem, Sudoku solver, maze traversal

---

## Divide and Conquer (225)

**Q225: What is divide and conquer?**

**Answer:**
Divide and conquer is an algorithmic paradigm that:
- Breaks problem into smaller, similar subproblems
- Recursively solves subproblems
- Combines solutions to solve original problem
- Often leads to efficient algorithms
- Examples: merge sort, quick sort, binary search, fast Fourier transform

---

## Artificial Intelligence (226)

**Q226: What is artificial intelligence?**

**Answer:**
Artificial Intelligence (AI) is technology that:
- Enables machines to simulate human intelligence
- Includes learning, reasoning, problem-solving, and perception
- Can be narrow (specific tasks) or general (human-like intelligence)
- Applications: speech recognition, image processing, decision making
- Uses machine learning, neural networks, and expert systems

---

## Machine Learning vs Deep Learning (227)

**Q227: Define machine learning vs deep learning.**

**Answer:**
- **Machine Learning**: 
  - Subset of AI that enables systems to learn from data
  - Improves performance without explicit programming
  - Uses algorithms to identify patterns and make predictions
  
- **Deep Learning**: 
  - Subset of machine learning using neural networks
  - Automatically learns hierarchical representations
  - Requires large amounts of data and computational power

---

## Internet of Things (228)

**Q228: What is Internet of Things (IoT)?**

**Answer:**
IoT is a network of:
- Physical devices embedded with sensors and connectivity
- Objects that can collect and exchange data
- Smart devices that can be monitored and controlled remotely
- Applications: smart homes, industrial automation, healthcare monitoring
- Enables automation and data-driven decision making

---

## Blockchain (229)

**Q229: Explain blockchain.**

**Answer:**
Blockchain is a distributed ledger technology that:
- Records transactions in blocks linked by cryptography
- Provides transparency, immutability, and decentralization
- Eliminates need for trusted intermediaries
- Uses consensus mechanisms for validation
- Applications: cryptocurrencies, supply chain, voting systems

---

## Edge Computing (230)

**Q230: What is edge computing?**

**Answer:**
Edge computing is a distributed computing paradigm that:
- Processes data closer to data source (edge of network)
- Reduces latency and bandwidth usage
- Improves real-time processing capabilities
- Supports IoT devices and mobile applications
- Complements cloud computing for distributed workloads

---

## Quantum Computing (231)

**Q231: Define quantum computing.**

**Answer:**
Quantum computing uses quantum mechanical phenomena to:
- Process information using quantum bits (qubits)
- Perform calculations exponentially faster than classical computers
- Solve complex problems in cryptography, optimization, and simulation
- Face challenges in error correction and qubit stability
- Still in early development stages

---

## Augmented Reality vs Virtual Reality (232)

**Q232: What is augmented reality vs virtual reality?**

**Answer:**
- **Augmented Reality (AR)**: 
  - Overlays digital information on real-world environment
  - Enhances real-world experience with computer-generated content
  - Examples: Pokemon Go, AR navigation, industrial training
  
- **Virtual Reality (VR)**: 
  - Creates completely immersive digital environment
  - Replaces real-world experience entirely
  - Examples: gaming, training simulations, virtual tours

---

## 5G Technology (233)

**Q233: Explain 5G technology.**

**Answer:**
5G is the fifth generation of mobile networks that provides:
- Higher data rates (up to 10 Gbps)
- Lower latency (1-10 milliseconds)
- Increased device density and network capacity
- Support for IoT, autonomous vehicles, and smart cities
- Uses millimeter wave frequencies and advanced antenna technologies

---

## Big Data (234)

**Q234: What is big data?**

**Answer:**
Big data refers to extremely large datasets that:
- Exceed traditional database processing capabilities
- Are characterized by volume, velocity, and variety
- Require specialized tools and techniques for analysis
- Provide insights for business intelligence and decision making
- Examples: social media data, sensor data, transaction logs

---

## Data Analytics vs Data Science (235)

**Q235: Define data analytics vs data science.**

**Answer:**
- **Data Analytics**: 
  - Focuses on analyzing data to find patterns and insights
  - Uses statistical methods and visualization tools
  - Aims to answer specific business questions
  
- **Data Science**: 
  - Broader field combining statistics, programming, and domain expertise
  - Develops predictive models and algorithms
  - Creates new methods for data analysis

---

## Natural Language Processing (236)

**Q236: What is natural language processing (NLP)?**

**Answer:**
NLP is a branch of AI that enables computers to:
- Understand, interpret, and generate human language
- Process text and speech data
- Perform tasks like translation, sentiment analysis, and chatbots
- Use machine learning and linguistic rules
- Applications: virtual assistants, search engines, language translation

---

## Robotics (237)

**Q237: Explain robotics.**

**Answer:**
Robotics combines mechanical engineering, electronics, and computer science to:
- Design, build, and operate robots
- Automate physical tasks and processes
- Create machines that can sense, think, and act
- Applications: manufacturing, healthcare, exploration, household assistance
- Integrates AI, sensors, and actuators for autonomous operation

---

## Serverless Computing (238)

**Q238: What is serverless computing?**

**Answer:**
Serverless computing is a cloud computing model where:
- Cloud provider manages server infrastructure
- Developers focus on code without server management
- Functions are executed on-demand
- Pay only for actual compute time used
- Examples: AWS Lambda, Azure Functions, Google Cloud Functions

---

## Microservices Architecture (239)

**Q239: Define microservices architecture.**

**Answer:**
Microservices architecture is a design pattern where:
- Applications are built as collection of small, independent services
- Each service runs in its own process and communicates via APIs
- Services can be developed, deployed, and scaled independently
- Improves maintainability, scalability, and fault isolation
- Challenges include distributed system complexity and data consistency

---

## Container Orchestration (240)

**Q240: What is container orchestration (e.g., Kubernetes)?**

**Answer:**
Container orchestration automates:
- Deployment, scaling, and management of containerized applications
- Load balancing and service discovery
- Health monitoring and failure recovery
- Resource allocation and scheduling
- Kubernetes is the most popular container orchestration platform

---

## Cloud Computing Models (241)

**Q241: Explain cloud computing models (IaaS, PaaS, SaaS).**

**Answer:**
- **IaaS (Infrastructure as a Service)**: 
  - Provides virtualized computing resources (servers, storage, networking)
  - User manages OS, applications, and data
  
- **PaaS (Platform as a Service)**: 
  - Provides platform for developing and deploying applications
  - User manages applications and data
  
- **SaaS (Software as a Service)**: 
  - Provides complete software applications
  - User only manages data and user access

---

## DevOps (242)

**Q242: What is DevOps?**

**Answer:**
DevOps is a set of practices that:
- Combines software development (Dev) and IT operations (Ops)
- Automates software delivery and infrastructure changes
- Promotes collaboration and communication between teams
- Emphasizes continuous integration, delivery, and deployment
- Aims to reduce development cycles and improve reliability

---

## CI/CD Pipeline (243)

**Q243: Define CI/CD pipeline.**

**Answer:**
CI/CD pipeline is an automated process that:
- **CI (Continuous Integration)**: Automatically builds and tests code changes
- **CD (Continuous Delivery/Deployment)**: Automatically deploys code to production
- Reduces manual errors and speeds up software delivery
- Includes automated testing, security scanning, and deployment
- Tools: Jenkins, GitLab CI, GitHub Actions, CircleCI

---

## Infrastructure as Code (244)

**Q244: What is infrastructure as code (IaC)?**

**Answer:**
Infrastructure as Code is the practice of:
- Managing and provisioning infrastructure through code and configuration files
- Treating infrastructure like software with version control
- Automating infrastructure deployment and configuration
- Ensuring consistency and reducing manual errors
- Tools: Terraform, AWS CloudFormation, Ansible, Chef

---

## Virtualization vs Containerization (245)

**Q245: Explain virtualization vs containerization.**

**Answer:**
- **Virtualization**: 
  - Creates complete virtual machines with OS
  - Higher resource overhead and isolation
  - Examples: VMware, Hyper-V, VirtualBox
  
- **Containerization**: 
  - Shares host OS kernel, packages application and dependencies
  - Lower resource overhead and faster startup
  - Examples: Docker, Kubernetes, LXC

---

## Green Computing (246)

**Q246: What is green computing?**

**Answer:**
Green computing focuses on:
- Environmentally responsible use of computing resources
- Energy-efficient hardware and software design
- Sustainable manufacturing and disposal practices
- Reducing carbon footprint of IT operations
- Practices: power management, virtualization, cloud computing, recycling

---

## Digital Twin (247)

**Q247: Define digital twin.**

**Answer:**
A digital twin is a virtual representation that:
- Mirrors physical objects, processes, or systems in real-time
- Uses sensors and IoT data for continuous updates
- Enables simulation, monitoring, and optimization
- Applications: manufacturing, smart cities, healthcare, aerospace
- Supports predictive maintenance and decision making

---

## 3D Printing (248)

**Q248: What is 3D printing?**

**Answer:**
3D printing (additive manufacturing) is a process that:
- Creates three-dimensional objects by depositing materials layer by layer
- Builds objects from digital 3D models
- Supports various materials: plastics, metals, ceramics, biological materials
- Applications: prototyping, manufacturing, healthcare, construction
- Enables rapid prototyping and customized production

---

## Wearable Technology (249)

**Q249: Explain wearable technology.**

**Answer:**
Wearable technology includes electronic devices that:
- Are worn on the body or integrated into clothing
- Monitor health metrics, track fitness, and provide notifications
- Connect to smartphones and cloud services
- Examples: smartwatches, fitness trackers, smart glasses, health monitors
- Uses sensors, wireless connectivity, and mobile apps

---

## Ethical Considerations in Emerging Tech (250)

**Q250: What are ethical considerations in emerging tech?**

**Answer:**
Ethical considerations in emerging technologies include:
- **Privacy**: Data collection and surveillance concerns
- **Bias**: Algorithmic discrimination and fairness
- **Autonomy**: Human control over AI systems
- **Accountability**: Responsibility for AI decisions and actions
- **Transparency**: Explainable AI and decision-making processes
- **Job Displacement**: Economic impact of automation
- **Security**: Vulnerabilities and misuse of technology
- **Environmental Impact**: Sustainability and resource consumption
