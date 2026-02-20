# Marykerin Naughton

## About Me

Recent graduate with a Higher Diploma in Computer Science (Software Development), bringing a distinctive blend of technical programming skills and creative production experience. My career in film and theatre production as a Production Designer, Art Director, Prop Designer, and Master Scenic Artist has equipped me with exceptional problem-solving abilities, meticulous attention to detail, and the capacity to thrive in high-pressure, deadline-driven environments.

This unique background allows me to approach software development with both analytical precision and creative thinking. I understand the importance of user experience from years of creating immersive environments for audiences, and I apply this same dedication to building functional, well-designed applications. Whether working independently or collaborating within a team, I bring strong communication skills, adaptability, and a commitment to delivering quality work on schedule.

I'm passionate about building practical applications that solve real-world problems, and I'm eager to contribute my skills to a development team while continuing to grow and learn in the software engineering field.

## 🛠️ Technical Skills

### Programming Languages & Markup
- **Java** - Object-oriented programming, algorithm implementation, concurrent programming with virtual threads, exception handling, test-driven development
- **JavaScript (ES6+)** - Client-side scripting, DOM manipulation, event handling, asynchronous programming, localStorage API, JSON data handling
- **SQL** - Complex queries with JOINs and subqueries, database design and normalization, stored procedures, aggregate functions, parameterized queries for security
- **HTML5** - Semantic markup, form validation, accessibility best practices, responsive structure
- **CSS3** - Responsive design, flexbox layouts, custom styling, Bootstrap framework integration, mobile-first approach

### Frameworks, Libraries & Tools
- **Node.js** - Server-side JavaScript runtime, asynchronous I/O operations, event-driven architecture
- **Express.js** - Web application framework, RESTful API routing, middleware implementation, session management, static file serving
- **EJS (Embedded JavaScript)** - Server-side templating engine, dynamic content rendering, data injection into HTML templates
- **Bootstrap 5** - Responsive grid system, component library, carousel implementation, utility classes, mobile-first design
- **JUnit 5** - Unit testing framework, test lifecycle management, parameterized testing, assertions, test suites

### Databases & Data Management
- **MySQL** - Relational database design, normalization techniques, foreign key constraints, indexing for optimization, role-based access control (GRANT permissions), database security best practices
- **Database Design Principles** - Entity-relationship modeling, normalization (1NF, 2NF, 3NF), referential integrity, transaction management

### Development Practices & Methodologies
- **MVC Architecture** - Separation of concerns, modular code organization, maintainable application structure
- **RESTful API Design** - HTTP methods (GET, POST, PUT, DELETE), stateless communication, resource-based URLs
- **Version Control** - Git fundamentals, repository management, commit best practices
- **Security Implementation** - SQL injection prevention through parameterized queries, input validation (client and server-side), error handling without exposing system details
- **Concurrent Programming** - Virtual threads, thread-safe data structures (ConcurrentHashMap), executor services, asynchronous task execution
- **Test-Driven Development** - Writing tests before implementation, red-green-refactor cycle, regression testing

### Software Development Competencies
- **Algorithm Implementation** - Sørensen-Dice similarity algorithm, prefix-suffix text parsing, search and comparison algorithms
- **File I/O Operations** - BufferedReader, FileWriter, Files API (NIO), stream processing, progress tracking
- **Error Handling** - Try-catch blocks, exception hierarchy, graceful degradation, user-friendly error messages
- **Code Refactoring** - Eliminating code smells, applying SOLID principles, improving code maintainability
- **Performance Optimization** - Efficient data structures, concurrent processing, database query optimization

## 💼 Portfolio Projects

### 🕯️ Candle Shop E-Commerce Web Application
**[View Repository]( https://github.com/MKNaughton/E-Commerce-Web-Application-Candle-Shop)** | 
**Technologies:**
 Node.js, Express.js 5.1.0, MySQL 8.0, EJS 3.1.10, Bootstrap 5.3.0, JavaScript ES6, HTML5, CSS3

A full-stack e-commerce web application designed for browsing and purchasing handcrafted candles online. This project demonstrates comprehensive understanding of web development from database design through to responsive frontend implementation, showcasing the complete software development lifecycle.

#### Technical Implementation Highlights:

**Backend Architecture:**
- Built Express.js server with organized routing structure separating authentication, product display, and form handling
- Created custom authentication module (`auth.js`) using Node.js `module.exports` pattern for code reusability and separation of concerns
- Implemented dual-layer authentication: client-side validation using regex patterns for email format verification and server-side credential checking
- Designed RESTful API routes supporting both GET (product retrieval via query parameters) and POST (login authentication, form submissions) methods
- Configured middleware stack including `express.urlencoded()` for parsing POST request bodies and `express.static()` for efficient static asset delivery

**Database Integration:**
- Structured MySQL database containing product catalog with 6 candle products including names, manufacturers, batch information, pricing, and image references
- Implemented parameterized SQL queries using placeholder values (`?`) to prevent SQL injection attacks, following OWASP security guidelines
- Created efficient database queries targeting specific products by ID, reducing data transfer and improving response times
- Designed normalized database schema eliminating data redundancy

**Frontend Development:**
- Developed server-side rendering using EJS templating engine, injecting dynamic product data from MySQL into HTML templates using `<%= %>` syntax
- Built responsive user interface with Bootstrap 5 framework featuring mobile-first design principles
- Implemented interactive carousel component with JavaScript randomization using `Math.random()` to display different starting images on each page load, enhancing user engagement
- Created custom CSS styling maintaining consistent design language across all pages with navy (#0a192f) and blue (#1e88e5) color scheme
- Applied "Great Vibes" typography for elegant heading presentation while maintaining readability with sans-serif body text

**Shopping Cart Functionality:**
- Engineered client-side cart management system using browser localStorage API for persistent data storage across page navigation
- Implemented JavaScript functions for adding products to cart, validating quantity selections, creating JSON objects with price and quantity data using `JSON.stringify()`
- Developed checkout page that iterates through localStorage, parses JSON data with `JSON.parse()`, calculates individual item costs and running totals
- Added visual confirmation messages with auto-dismiss functionality using `setTimeout()` for improved user feedback

**Form Handling & Validation:**
- Created comprehensive checkout form collecting customer information (name, email, address) with HTML5 validation attributes
- Implemented client-side JavaScript validation checking for empty fields, valid email formats using regex patterns, and proper data formatting
- Designed payment method selection dropdown offering multiple options (credit card, PayPal, Stripe)
- Applied CSS error states with red borders and error messages providing immediate visual feedback on validation failures

**Key Learning Outcomes:**
- Understanding of full-stack development workflow from database design to frontend implementation
- Practical application of MVC architectural pattern separating data, business logic, and presentation
- Experience with asynchronous JavaScript operations and callback functions
- Implementation of security best practices including parameterized queries and input validation
- Development of responsive, mobile-friendly user interfaces

---

### 📝 Text Similarity Comparison Java Application
**[View Repository](https://github.com/MKNaughton/Text-Similarity-Comparison-Java-Application)** | 
**Technologies:** 
Java 21, Virtual Threads, ConcurrentHashMap, Executors Framework, NIO Files API, Lambda Expressions

A console-based Java application implementing the Sørensen-Dice similarity algorithm for comparing text documents and calculating similarity percentages. This project demonstrates advanced Java concurrency patterns using Java 21's modern virtual threads feature, thread-safe programming, and algorithm implementation.

#### Technical Implementation Highlights:

**Concurrent Architecture:**
- Utilized Java 21's virtual threads via `Executors.newVirtualThreadPerTaskExecutor()` enabling lightweight concurrent processing of multiple files simultaneously
- Designed inner `Parser` class implementing `Callable<Set<String>>` interface for asynchronous file parsing tasks returning results via `Future` objects
- Implemented concurrent processing pattern where query files and subject files parse simultaneously rather than sequentially, significantly improving performance for batch operations
- Applied try-with-resources pattern ensuring automatic executor service cleanup and proper resource management

**Thread-Safe Data Structures:**
- Employed `ConcurrentHashMap.newKeySet()` for thread-safe token storage, preventing race conditions when multiple virtual threads access shared collections
- Designed architecture ensuring thread safety without explicit synchronization blocks, leveraging Java's concurrent collections framework
- Implemented immutable data patterns where appropriate to eliminate potential concurrency issues

**Algorithm Implementation:**
- Coded Sørensen-Dice coefficient calculation: `2 * |A ∩ B| / (|A| + |B|)` where A and B represent word token sets from compared documents
- Created intersection logic identifying common words between document sets
- Calculated similarity scores returning values between 0.0 (no similarity) and 1.0 (identical documents)

**File Processing:**
- Leveraged Java NIO `Files.lines()` API for efficient line-by-line file reading with automatic resource management
- Implemented tokenization splitting text on whitespace using regex patterns, converting to lowercase for case-insensitive comparison
- Applied lambda expressions and `forEach` operations for functional stream processing of text data
- Added empty string filtering to eliminate noise from whitespace-only tokens

**Batch Processing & Results Management:**
- Developed functionality supporting comma-separated file paths enabling comparison of multiple query files against multiple subject files in single execution
- Implemented `List<ResultsOutput>` structure storing all comparison results for batch export operations
- Created `FileWriter` with append mode preventing overwriting of previous results, allowing cumulative result logging
- Designed progress tracking displaying real-time feedback during longer batch comparison operations

**User Interface & Input Handling:**
- Built menu-driven console interface with seven options providing complete workflow control
- Implemented input validation using `trim()` method handling extra whitespace in user-provided file paths
- Created configuration viewer displaying current settings and loaded word counts
- Added error handling for invalid file paths, missing files, and malformed input preventing application crashes

**Code Organization:**
- Structured application across six classes following separation of concerns principle:
  - `Runner` - Application entry point
  - `Menu` - User interaction and input validation
  - `CompareText` - Comparison engine with inner Parser class
  - `FileParser` - Text file parsing into token sets
  - `DiceSimilarity` - Similarity calculation implementation
  - `ResultsOutput` - Results formatting and file export

**Key Learning Outcomes:**
- Mastery of modern Java concurrency with virtual threads
- Understanding of thread-safe programming and concurrent collections
- Algorithm implementation and mathematical computation
- Functional programming with lambda expressions and streams
- Clean code architecture with proper separation of concerns

---

### 🔤 Text Encode-Decode Java Application
**[View Repository](https://github.com/MKNaughton/Text-Encode-Decode-Java-Application)** 
| **Technologies:** 
Java, BufferedReader, FileWriter, Array Data Structures, CSV Processing

A console-based Java application performing bidirectional encoding and decoding of text files using a comprehensive 9,999-entry word-to-code mapping dictionary loaded from CSV format. This project showcases algorithm design, file I/O operations, custom data structure implementation, and complex string manipulation.

#### Technical Implementation Highlights:

**Encoding Algorithm Design:**
- Developed word-based encoding system processing text word-by-word rather than character-by-character, utilizing whitespace splitting with `String.split("\\s+")` regex pattern
- Engineered intelligent prefix-suffix splitting algorithm for handling dictionary misses:
  - Iterates through split points from index 1 to word length
  - Creates prefix using `word.substring(0, splitPoint)` and suffix using `word.substring(splitPoint)`
  - Appends "@@" notation to suffixes aligning with CSV format conventions
  - Searches arrays for both components, returning `[prefixCode,suffixCode]` format for split words
- Implemented normalization method converting text to lowercase and stripping non-alphanumeric characters using `replaceAll("[^a-z0-9]", "")` improving encoding success rates
- Applied fallback strategy returning code `0` for completely unmatched words

**Decoding Algorithm Design:**
- Created reverse lookup functionality searching code arrays to retrieve original words
- Implemented bracket detection parsing encoded text to identify single codes versus double codes (prefix-suffix pairs)
- Developed string parsing splitting double codes on comma delimiter
- Applied "@@" prefix stripping from decoded suffix entries restoring original word structure
- Concatenated prefix and suffix components reconstructing split words
- Returned `[???]` placeholder for unrecognized codes maintaining output structure integrity

**Data Structure Management:**
- Designed parallel array architecture: `String[] words` storing dictionary words and `int[] codes` storing corresponding numeric codes
- Implemented array-based lookup requiring linear search O(n) complexity, understanding tradeoff between simplicity and performance
- Passed arrays by reference between `FileProcessor` and `TextEncodingDecoding` classes avoiding expensive data copying and improving memory efficiency
- Managed array indices carefully preventing `ArrayIndexOutOfBoundsException` errors

**Custom StringBuilder Implementation:**
- Built custom `StringBuilder` class from scratch using char arrays rather than String concatenation
- Implemented dynamic capacity resizing starting with 4 character capacity and doubling when full (exponential growth strategy)
- Created method overloading supporting `append(String)`, `append(char)`, and `append(int)` for flexible string construction
- Provided `toString()` conversion method creating final String from accumulated characters
- Demonstrated understanding of memory management and performance optimization (avoiding String immutability overhead)

**File I/O Operations:**
- Utilized `BufferedReader` for efficient line-by-line file reading reducing disk I/O operations
- Implemented CSV parsing extracting word-code pairs from comma-delimited format
- Applied `FileWriter` for output file creation with proper resource management using try-with-resources
- Developed two-pass file reading: first pass counting total lines for accurate progress calculation, second pass processing content

**Progress Tracking & User Feedback:**
- Engineered visual progress indicator displaying percentage completion with bracket notation `[####----] 45%`
- Calculated progress at 2% intervals (50 total updates) balancing feedback frequency with console output performance
- Implemented first-line debug output (limited to 3 lines) for verification without excessive console spam
- Maintained output structure integrity handling empty lines appropriately

**Error Handling:**
- Implemented comprehensive exception catching:
  - `FileNotFoundException` validating file paths before processing preventing crashes
  - `IOException` handling corrupted or inaccessible files gracefully
  - `NullPointerException` checks across all array operations ensuring data integrity
  - `NumberFormatException` catching invalid menu selections providing user-friendly error messages
- Designed graceful degradation allowing application continuation after recoverable errors

**Menu System & Configuration:**
- Created 7-option menu interface providing complete workflow control including:
  - Mapping file specification (default: `./encodings-10000.csv`)
  - Input file configuration
  - Output file configuration (default: `./output.txt`)
  - Settings viewer displaying current configuration
  - Encode operation execution
  - Decode operation execution
  - Application exit
- Implemented default value system with override capability balancing convenience and flexibility

**Key Learning Outcomes:**
- Algorithm design for complex text processing challenges
- Array manipulation and data structure selection
- Custom class implementation (StringBuilder) understanding underlying mechanics
- File I/O operations and resource management
- User interface design for command-line applications
- Error handling strategies and defensive programming

---

### 🧪 Banking Test Suite with JUnit 5 - Java
**[View Repository](https://github.com/MKNaughton/Junit-Agile-Java-Project)** | 
**Technologies:** 
Java, JUnit 5.13.4, Test-Driven Development, Object-Oriented Design

A comprehensive testing suite validating banking account management functionality using JUnit 5 framework. This project demonstrates test-driven development practices, code refactoring following SOLID principles, and mastery of various JUnit testing patterns including parameterized tests, exception testing, and test lifecycle management.

#### Technical Implementation Highlights:

**Code Refactoring & Architecture:**
- Refactored original monolithic design extracting `Account` from private nested class within `BankingApp` to separate public class in `ie.atu.dip` package
- Applied Single Responsibility Principle: `Account` class manages individual account operations while `BankingApp` manages multiple accounts and bank-level operations
- Eliminated code smell improving testability, maintainability, and following object-oriented design best practices
- Designed clear separation of concerns enabling independent testing of account behavior versus bank management logic

**Test Organization & Structure:**
- Created four distinct test classes each focusing on specific testing aspects:
  - `AccountTest` - Individual account behavior testing
  - `BankingAppTest` - Bank management and multi-account operations
  - `AccountParameterizedTest` - Account operations with multiple input datasets
  - `BankingAppParameterizedTest` - Bank operations with varied test data
- Implemented `AllTestSuite` using `@Suite` and `@SelectClasses` annotations combining `AccountTest` and `BankingAppTest` for batch test execution
- Applied class-level `@Timeout(value = 300, unit = TimeUnit.MILLISECONDS)` on `AccountTest` enforcing performance constraints

**Test Lifecycle Management:**
- Utilized `@BeforeEach` annotation creating fresh test data before each test method ensuring test independence and isolation
- Implemented test fixture setup initializing `BankingApp` instance and populating with Alice (€1000) and Bob (€500) test accounts
- Applied `@BeforeAll` for one-time setup operations and `@AfterAll` for cleanup when needed
- Used `@AfterEach` for per-test cleanup maintaining clean test state

**Parameterized Testing Patterns:**
- Implemented `@ValueSource` for testing single parameters with multiple values:
  ```java
  @ValueSource(doubles = {100.0, 250.0, 500.0, 1000.0})
  ```
  Testing deposit operations with various amounts reducing test code duplication
- Applied `@CsvSource` for testing multiple parameters as comma-separated values:
  ```java
  @CsvSource({
      "200, true, 800",    // amount, expected success, expected balance
      "1000, true, 0",
      "1500, false, 1000"
  })
  ```
  Testing withdrawal scenarios covering success cases, boundary conditions, and failure scenarios

**Assertion Techniques:**
- Used `assertEquals()` for value comparisons validating expected versus actual results
- Applied `assertTrue()` and `assertFalse()` for boolean operation verification
- Implemented precise floating-point comparisons for monetary calculations
- Created meaningful assertion messages improving test failure diagnostics

**Exception Testing:**
- Implemented `assertThrows()` for exception validation:
  ```java
  assertThrows(NullPointerException.class, () -> {
      Account nullAccount = null;
      nullAccount.getBalance();
  });
  ```
- Tested `ArithmeticException` for division by zero scenarios
- Validated proper exception handling across banking operations
- Ensured application fails gracefully with appropriate error messages

**Banking Business Logic Testing:**
- Validated account creation with initial deposits updating both account balance and bank total deposits
- Tested deposit operations confirming balance increases and bank deposit tracking
- Verified withdrawal operations with insufficient funds checking preventing overdrafts
- Tested loan approval mechanism limited by total bank deposits (loans cannot exceed available deposits)
- Validated loan repayment functionality with overpayment prevention
- Confirmed `hasAccount()` lookup functionality for account existence checking
- Tested `findAccount()` helper method encapsulating account search logic

**Test Coverage:**
- Achieved comprehensive coverage of all banking operations: create, deposit, withdraw, approve loan, repay loan
- Tested boundary conditions: zero amounts, exact balance matches, maximum values
- Validated edge cases: insufficient funds, loan amount exceeding deposits, non-existent accounts
- Confirmed error conditions: null accounts, negative values, invalid operations

**TDD Practices Demonstrated:**
- Red-Green-Refactor workflow: write failing test, implement code to pass, refactor for quality
- Test-first development writing tests before implementation code
- Regression testing after refactoring ensuring functionality preservation during code improvements
- Hardcoded expected values in tests (you control setup, verify implementation correctness)

**Key Learning Outcomes:**
- Mastery of JUnit 5 testing framework and annotations
- Understanding of test-driven development methodology
- Code refactoring techniques following SOLID principles
- Parameterized testing reducing code duplication
- Exception testing and error condition validation
- Test organization and suite management

---

### 🏥 Veterinary Clinic Management Database System
**[View Repository](https://github.com/MKNaughton/MySQL-Database-Veterinary-Clinic-Database)** 
| **Technologies:**
 MySQL 8.0, Complex SQL Queries, Database Design, Security Implementation

A comprehensive relational database system designed for managing complete veterinary clinic operations including clinical services, financial management, inventory control, retail sales, and staff administration. This project demonstrates advanced database design principles, normalization techniques, security implementation, and business intelligence reporting.

#### Technical Implementation Highlights:

**Database Architecture & Schema Design:**
- Architected 13 interconnected tables organized across four business domains:
  - **Clinical Operations:** Staff, Customer, Animal, Appointment, MedicalRecord
  - **Financial Management:** Billing, Payment
  - **Inventory & Retail:** Supplier, Inventory, SupplyOrder, OrderItem, ProductSale, SaleItem
- Applied database normalization (1NF, 2NF, 3NF) eliminating data redundancy and ensuring data integrity
- Designed primary key strategy using auto-incrementing integers for efficient indexing
- Implemented foreign key constraints establishing referential integrity across related tables
- Created composite keys where appropriate (e.g., OrderItem linking SupplyOrder and Inventory)

**Entity Relationships & Data Modeling:**
- Established one-to-many relationships: Customer to Animal, Animal to Appointment, Appointment to MedicalRecord
- Implemented many-to-many relationships through junction tables: SupplyOrder to Inventory via OrderItem, ProductSale to Inventory via SaleItem
- Designed self-referential relationship in Staff table for manager-employee hierarchy
- Applied appropriate cardinality constraints ensuring business rule enforcement at database level

**Complex SQL Query Implementation:**
- Developed multi-table JOIN queries combining data from Clinical, Financial, and Inventory domains
- Created subqueries for nested data retrieval and complex filtering conditions
- Implemented aggregate functions (SUM, COUNT, AVG, MAX, MIN) for business calculations
- Applied GROUP BY clauses for categorical data aggregation and reporting
- Utilized HAVING clauses for filtering aggregated results
- Constructed CASE statements for conditional logic within queries

**View Creation for Business Intelligence:**
- **vw_FinancialOverview:** Calculates total revenue from billing against total expenses from supply orders showing overall profitability for manager/owner review
- **vw_StaffDirectory:** Provides staff contact and role information excluding sensitive salary data, accessible to all staff members
- **vw_TodaysAppointments:** Filters appointment table to current date for receptionists managing daily workflow and scheduling
- **vw_ReorderAlert:** Identifies inventory items below reorder threshold alerting supplies administrator for timely restocking
- **vw_OutstandingBills:** Shows unpaid bills with amounts owing including partial payment tracking for installment agreements, supporting billing administration

**Security Implementation:**
- Designed role-based access control (RBAC) using GRANT statements:
  - Veterinary administrators: Full access (SELECT, INSERT, UPDATE) to MedicalRecord
  - Veterinarians: Read-only access (SELECT) to MedicalRecord for consultation
  - Reception staff: Management access to Customer, Animal, Appointment, ProductSale tables
  - Billing administrators: Full access to Billing and Payment tables
  - Supplies administrators: Management access to Inventory, SupplyOrder, OrderItem tables
- Protected sensitive salary information through vw_StaffDirectory view excluding compensation data
- Restricted financial overview (vw_FinancialOverview) to manager/business owner preventing unauthorized access to profitability data
- Applied principle of least privilege granting minimum necessary permissions for each role

**Index Optimization:**
- Created indexes on frequently queried columns improving SELECT performance:
  - Customer name and contact information for quick lookup
  - Animal species and customer_id for filtered searches
  - Appointment date and veterinarian assignment for scheduling queries
  - Billing payment status and customer for accounts receivable reporting
- Balanced index creation considering query performance improvement versus INSERT/UPDATE overhead
- Applied compound indexes for multi-column filtering scenarios

**Business Logic Implementation:**
- **Billing with Installments:** Designed Billing table with total amount and Payment table tracking individual payments enabling installment arrangement support
- **Farm Animal Handling:** Stored farm animals alongside domestic pets in unified Animal table using species column for differentiation and industry-standard identification codes
- **Dual-Purpose Inventory:** Implemented single Inventory table with forSale boolean flag separating clinical supplies from retail products
- **Supplier Management:** Linked inventory items to suppliers tracking payment terms and contact information for procurement operations

**Data Integrity & Constraints:**
- Applied NOT NULL constraints on required fields preventing incomplete records
- Implemented CHECK constraints validating data ranges (e.g., prices > 0, quantities > 0)
- Designed UNIQUE constraints preventing duplicate customer emails and employee usernames
- Applied DEFAULT values for fields like appointment status ('Scheduled') and inventory forSale flag (FALSE)
- Utilized ON DELETE and ON UPDATE cascade rules maintaining referential integrity during data modifications

**Scalability Considerations:**
- Designed schema supporting multiple clinic locations through potential location_id foreign key
- Architected inventory system accommodating both small clinic and large practice scale
- Created flexible appointment system supporting various appointment types and durations
- Implemented medical records structure supporting comprehensive patient history tracking

**Key Learning Outcomes:**
- Comprehensive understanding of relational database design principles
- Proficiency in complex SQL query construction with multiple JOINs
- Implementation of database security through role-based access control
- View creation for operational reporting and business intelligence
- Index optimization balancing query performance and data modification overhead
- Real-world application of normalization theory preventing data anomalies

---

## 🎯 Transferable Skills from Creative Production

### Problem-Solving & Critical Thinking
- **Scenic Design Challenges:** Developed creative solutions working within physical, budgetary, and time constraints - similar to software development tradeoffs between functionality, performance, and delivery deadlines
- **Prop Fabrication:** Engineered practical solutions bringing abstract concepts to physical reality, paralleling the process of translating requirements into working code.
- **Production Troubleshooting:** Diagnosed and resolved technical issues during live productions under pressure, comparable to debugging and fixing critical software issues in production environments.
- **Resource Optimization:** Maximized limited budgets and materials in theatre production, similar to optimizing code performance and memory usage in software applications.

### Project Management & Delivery
- **Deadline Management:** Consistently delivered theatre productions on strict opening night deadlines with no room for delay - demonstrating ability to deliver software projects on schedule
- **Multi-Project Coordination:** Managed overlapping production schedules as freelancer balancing multiple concurrent projects, applicable to managing multiple development tasks or features
- **Milestone Tracking:** Broke down large productions into manageable phases (concept, design, build, install, opening), mirroring agile sprint planning and software development lifecycle stages
- **Quality Assurance:** Maintained high production standards under time pressure ensuring finished work met artistic and safety requirements before public viewing

### Collaboration & Communication
- **Cross-Functional Teamwork:** Collaborated effectively with directors (product owners), producers (project managers), technical crew (developers), and actors (users/stakeholders) requiring clear communication across diverse skill sets
- **Technical Communication:** Translated artistic vision into technical specifications for carpenters, painters, and electricians, comparable to translating business requirements into technical documentation
- **Stakeholder Management:** Presented design concepts to directors and producers incorporating feedback while maintaining artistic integrity and technical feasibility
- **Conflict Resolution:** Navigated creative differences and production challenges diplomatically maintaining positive team dynamics under stress

### Attention to Detail & Quality
- **Master Scenic Artist Precision:** Executed detailed paintwork requiring extreme accuracy and consistency - directly applicable to writing clean, precise code and catching bugs
- **Design Documentation:** Created comprehensive technical drawings, material specifications, and build schedules ensuring accurate execution by production teams
- **Continuity Management:** Maintained visual consistency across scenes and performances tracking minute details over extended production runs
- **Safety Compliance:** Ensured all scenic elements met safety regulations and building codes demonstrating understanding of compliance and standards adherence

### Adaptability & Learning
- **Rapid Skill Acquisition:** Continuously learned new techniques, materials, and technologies in evolving theatre industry paralleling need for ongoing learning in fast-changing tech sector
- **Technology Adoption:** Integrated new tools and software (CAD programs, projection mapping, automated systems) into traditional scenic design workflow
- **Problem Pivoting:** Adapted designs mid-production when confronted with unexpected constraints (budget cuts, space limitations, safety concerns) similar to adjusting software requirements during development
- **Multi-Disciplinary Knowledge:** Bridged artistic creativity with technical engineering understanding both aesthetic and structural requirements

### Independent Work & Initiative
- **Freelance Career Management:** Successfully operated as independent contractor managing client relationships, project pipelines, invoicing, and quality standards
- **Self-Motivation:** Drove projects forward autonomously from concept through completion without constant supervision
- **Time Management:** Balanced multiple concurrent projects allocating time effectively across different production phases and client needs
- **Continuous Improvement:** Actively sought feedback and refined techniques improving craft over time demonstrating growth mindset

### User-Centered Thinking
- **Audience Experience:** Designed environments considering audience perspective, sightlines, and emotional impact - paralleling user experience (UX) design in software
- **Accessibility Considerations:** Ensured productions accommodated diverse audience needs including visibility, mobility, and sensory considerations
- **Immersive Design:** Created cohesive environments where all elements supported unified experience similar to creating consistent, intuitive user interfaces
- **Iterative Refinement:** Conducted technical rehearsals gathering feedback and making adjustments before public opening, comparable to user testing and iteration in software development

---

## 📚 Education

### Higher Diploma in Computer Science (Software Development)
**Atlantic Technological University (ATU)**  
Expected Graduation: 2025

**Core Modules Completed:**
- Object-Oriented Programming (Java)
- Web Application Development (Node.js, Express, HTML/CSS/JavaScript)
- Database Management Systems (MySQL, SQL)
- Data Structures & Algorithms
- Operating Systems
- Software Testing & Quality Assurance
- Computer Networks
- Project Engineering & Management

**Key Projects:** Full-stack e-commerce application, concurrent text processing system, database design, automated testing suite

**Academic Strengths:**
- Consistent performance across theoretical and practical modules
- Strong grasp of both object-oriented and functional programming paradigms
- Ability to connect abstract concepts to practical implementation
- Effective at independent learning and problem-solving

---

### BA (Honours) Fine Art
**[University Name]**  
Graduation: [2013]

**Focus Areas:**
- Multi Media
- Spatial design and environmental aesthetics
- Technical drawing and architectural rendering
- Material studies and fabrication techniques
- Project development from concept through execution
- Critical analysis and presentation skills

**Relevance to Software Development:**
- Developed strong visual design sense applicable to UI/UX
- Learned systematic approach to complex projects
- Built foundation in creative problem-solving
- Cultivated attention to detail and quality standards

---

## 💡 What I Bring to a Development Team

### Technical Foundation
- **Solid Programming Skills:** Proficiency in Java and JavaScript with understanding of object-oriented principles, data structures, and algorithms
- **Full-Stack Capability:** Experience across entire web development stack from database design through backend logic to responsive frontend implementation
- **Security Awareness:** Understanding of common vulnerabilities (SQL injection) and implementation of security best practices
- **Testing Knowledge:** Familiarity with test-driven development and automated testing frameworks
- **Database Expertise:** Ability to design normalized database schemas and write efficient SQL queries

### Professional Attributes
- **Fast Learner:** Successfully transitioned from arts to technical field mastering programming languages, frameworks, and development tools
- **Work Ethic:** Proven track record of delivering quality work on deadline from years in demanding production environments
- **Communication Skills:** Ability to explain technical concepts clearly and collaborate effectively with team members
- **Adaptability:** Comfortable working in fast-paced environments with changing requirements and shifting priorities
- **Problem-Solving Approach:** Creative yet analytical thinking combining artistic innovation with logical debugging
- **Team Player:** Experience collaborating across disciplines respecting different perspectives and skill sets

### Unique Perspective
- **User Empathy:** Understanding of end-user experience from creating audience-facing theatre productions
- **Design Sensibility:** Appreciation for aesthetics and usability in interface design
- **Attention to Detail:** Meticulous approach to work ensuring quality and catching errors
- **Creative Solutions:** Ability to think outside standard patterns when approaching technical challenges
- **Resilience:** Comfortable with critique and iteration, viewing feedback as opportunity for improvement

---

## 📫 Open to Opportunities

I'm actively seeking **entry-level developer positions**, **software development internships**, or **graduate programmes** where I can contribute my technical skills, creative problem-solving abilities, and strong work ethic while continuing to learn and grow as a software developer.

My unique combination of technical programming capabilities and creative production experience allows me to approach software development with both analytical precision and innovative thinking. I'm particularly drawn to opportunities where I can:

- Work on full-stack web applications building both frontend and backend components
- Collaborate with experienced developers learning best practices and industry standards
- Contribute to meaningful projects that solve real user problems
- Continue developing my technical skills in modern frameworks and technologies
- Apply my attention to detail and quality focus to writing clean, maintainable code

### Areas of Interest

**Web Development:**
- Full-stack application development
- Backend API development with Node.js/Express
- Frontend development with modern frameworks
- Responsive design and mobile-first development
- Database design and optimization

**Software Engineering:**
- Object-oriented programming and design patterns
- Algorithm implementation and optimization
- Concurrent and asynchronous programming
- Software testing and quality assurance
- Version control and collaborative development

**Emerging Interests:**
- UI/UX design and user experience optimization
- Cloud technologies and deployment
- DevOps practices and continuous integration
- Mobile application development
- Data visualization and analytics

### What I'm Looking For

**In a Role:**
- Opportunities to work on diverse projects building varied skill set
- Mentorship from experienced developers accelerating learning
- Collaborative team environment valuing communication and knowledge sharing
- Exposure to modern development tools, frameworks, and methodologies
- Clear path for professional growth and skill development

**In a Company:**
- Supportive culture that values continuous learning
- Commitment to best practices and code quality
- Diverse team bringing different perspectives
- Investment in junior developer growth and training
- Work-life balance supporting long-term career sustainability

---

## 🔗 Let's Connect

💻 **Browse my repositories below** to see detailed code, documentation, and implementation

📧 **[naughtonmarykerin@gmail.com]** - Feel free to reach out about opportunities or to discuss my projects

🌟 **Open to:** Entry-level developer roles, internships, graduate programmes, contract positions, remote work

---

*Thank you for taking the time to review my profile. I'm excited about transitioning into software development and contributing to meaningful projects while continuing to grow my technical skills.*
