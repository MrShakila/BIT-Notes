# Introduction to Software Testing: Software Quality Assurance

## Understanding Software, Quality, and Assurance

### Defining Software

- Software is a set of machine-readable instructions for a computer's processor.

- IEEE (1991) defines software as computer programs, procedures, and associated documentation and data for computer system operation.

- ISO (1997) defines software as computer programs, procedures, documentation, and data necessary for operating the software system.  All four components are essential for assuring software development quality.

### Defining Software Quality

- IEEE (1991) offers two definitions:  the degree to which software meets specified requirements, and the degree to which it meets customer needs or expectations.

- The first definition focuses on meeting a written specification.

- The second definition prioritizes customer satisfaction and fulfilling real needs.

### Quality Assurance vs. Testing

- Quality assurance (QA) is not the same as testing.

- QA is part of quality management, encompassing software development, human resources, and delivery processes.  It ensures standard procedures are followed correctly.

- Testing is a quality control activity.

- Testing is essential but insufficient alone; it should be integrated into a comprehensive, team-wide quality assurance process.

- QA supports good testing.

### Software Quality Assurance

- IEEE Glossary (1991) defines software quality assurance (SQA) as a planned, systematic pattern of actions to ensure a product meets requirements, and as activities to evaluate the development process.

- SQA involves planning and integrating actions across all development stages.

- SQA extends beyond development to encompass service and delivery.

- SQA includes non-technical aspects like scheduling and budget.

- A broader definition includes systematic, planned actions to ensure the software development or maintenance process conforms to functional and managerial requirements, including schedule and budget.

### Quality Assurance vs. Quality Control

- Quality control evaluates the quality of a finished product, withholding anything that doesn't meet standards.

- Quality assurance detects and prevents errors early, aiming to reduce the cost of ensuring quality.

- Quality control is a subset of quality assurance activities.

## Objectives of Software Quality Assurance and Testing

### Objectives in Development

- Ensure software meets functional and technical requirements.

- Ensure software meets managerial scheduling and budgetary requirements.

- Initiate and manage activities to improve the software development process and SQA activities.

### Objectives in Maintenance

- Ensure software maintenance activities meet functional and technical requirements.

- Ensure maintenance activities meet managerial scheduling and budgetary requirements.

- Initiate and manage activities to improve the efficiency of software maintenance and SQA activities.

### Objectives of Testing

- Verify that all specified requirements are met.

- Find failures and defects (a primary focus).

- Provide information to stakeholders for informed decisions on quality.

- Reduce the risk of inadequate software quality.

- Ensure compliance with contractual, legal, or regulatory requirements and standards.

## Testing and Debugging

### Testing vs. Debugging

- Testing and debugging are different concepts.

- Debugging is a software development activity where a developer identifies, analyzes, and removes a defect.

- Testing detects system defects and resulting failures.

- Further testing is needed after debugging to ensure functionality.

- Testers may conduct initial and final confirmation tests while developers debug.

- In Agile, testers may participate in debugging.

### Testing in Different Software Development Stages

- Requirement reviews and user story refinement: Detects defects early, reducing risks of incorrect or untestable software.

- System design: Improves stakeholder understanding and reduces design defect risks.

- Coding: Increases understanding of the code and reduces defect risks.

- Before release: Detects failures and ensures the software meets stakeholder requirements.

## Software Errors, Faults, and Failures

### Defining Errors, Faults, and Failures

- Software engineering involves human error (grammatical or logical).

- Errors can become software faults (defects), causing improper functioning.

- Not all faults become failures; a failure occurs when a fault causes unexpected behavior during execution.

- Only some errors become faults, and only some faults become failures.

### Root Causes of Defects

- A root cause is a source of defects; removing it reduces or eliminates the defect type.

- Root causes are the earliest actions or conditions causing defects.

- Root cause analysis should be conducted to prevent similar defects.

- Root causes are often organizational issues.

### Causes of Software Errors

- Identifying causes is crucial for avoiding poor-quality software.

- Errors can occur in any phase and be caused by any stakeholder.

- Causes include time pressure, human error, inexperienced personnel, code complexity, miscommunication, misunderstandings, and unfamiliar technologies.

- Errors can be code, procedure, documentation, or data errors.

- Galin [2] classifies errors into nine categories based on development stage: faulty requirements, communication failures, deliberate deviations, logical design errors, coding errors, non-compliance with documentation, testing shortcomings, procedure errors, and documentation errors.

### Specific Error Causes

- Faulty requirements: erroneous, incomplete, or unnecessary requirements.

- Communication failures: misunderstandings of instructions, changes, responses, or lack of attention.

- Deliberate deviations: reusing modules without analysis, omitting functionalities, or introducing improvements without approval.

- Logical design errors: erroneous algorithms, process definitions, or omitted system states.

- Coding errors: misunderstandings in design, linguistic errors, errors in using tools, or data selection errors.

- Non-compliance: ignoring documentation and coding standards.

- Testing shortcomings: incomplete plans, poor error reporting, or failure to correct errors.

- Procedure errors: misinterpreting system requirements due to procedural errors.

- Documentation errors: errors in design documents or user manuals.

## Manual vs. Automation Testing

### Manual vs. Automation Testing

- Manual testing involves human execution without scripts.

- Automation testing uses tools and scripts to automate testing tasks.

- Automation improves efficiency, reduces costs, and shortens testing time.

- Automated tests include code auditing, coverage monitoring, functional tests, load tests, and test management.

### Advantages and Disadvantages of Automation Testing

- Advantages: accuracy and completeness of performance, higher accuracy in documentation, comprehensive information, less manpower, and shorter testing periods.

- Disadvantages: high investment in purchasing and training, high development costs, high manpower for test preparation, and some testing areas may be left uncovered.

## Seven Testing Principles

### Testing shows the presence, not absence, of defects.

### Exhaustive testing is impossible.

### Early testing saves time and money.

### Defects cluster together.

### Beware of the pesticide paradox (repeating the same tests loses effectiveness).

### Testing is context-dependent.

### Absence of errors is a fallacy.

## Software Quality Assurance Models and Standards

### ISO 9000-3

- ISO 9000-3 guidelines from the International Organization for Standardization address software development and maintenance.

- It emphasizes eight quality management principles: customer focus, leadership, involvement of people, process approach, system approach to management, continual improvement, factual approach to decision making, and mutually supportive supplier relationships.

- Certification requires developing an SQA system (quality manuals and procedures, staff training), implementing it, and undergoing certification audits.

### Capability Maturity Models (CMM and CMMI)

- CMM focuses on improving an organization's software development process.

- CMMI integrates agile principles into CMM to improve development processes, configuration management, and quality management.

### Bootstrap Model

- The Bootstrap methodology measures organizational and project maturity based on 31 quality attributes categorized into process, organization, and technology.

### Benefits of Using Software Quality Assurance Standards

- Using sophisticated methodologies and procedures.

- Better understanding and cooperation among stakeholders.

- Obtaining SQA certifications through independent audits.

## Summary

### Software quality assurance is a planned, systematic approach to ensure products meet requirements and to evaluate the development process.

### Quality control focuses on withholding unqualified products.

### Debugging and testing are distinct; debugging fixes defects, while testing detects them.

### Software errors, faults, and failures are different concepts.

### Galin [2] categorizes software errors based on development stages.

### SQA standards promote the use of sophisticated methodologies and better understanding among stakeholders.


# Software Testing Process: A Comprehensive Overview

## The Software Testing Process

### Defining the Software Testing Process

- Effective and efficient testing involves proper planning and execution of tests designed to cover all necessary system areas.

- Results should be reviewed regularly.

- This is a process with identifiable tasks and activities.

- There's no one-size-fits-all approach; the right process achieves objectives efficiently.

- The best process for one project may not be suitable for another.

### Factors Influencing the Testing Process

- Software development life cycle models and project methodologies significantly impact the testing process.  An agile mobile app project will have a different process than a medical device project.

- Test levels and types influence the process. A large, complex project with various integration tests will require a more complex process.

- Product and project risks affect process formality; lower risk allows for less formal processes.

- Business domain, operational constraints (budgets, resources, timescales, complexity), organizational policies and practices, and required internal and external standards all play a role.

## Test Activities and Tasks

### Main Groups of Test Activities

- Test planning involves defining testing objectives and the approach to meet them within project constraints.  This includes deciding on techniques, tasks, and schedules.

- Test monitoring and control involves checking the status of testing activities, identifying variances from plans, and reporting to stakeholders.  Stopping testing or the project may be necessary if serious problems arise. Exit criteria, or "definition of done" in Agile, helps monitor progress.

- Test analysis identifies test conditions by analyzing the test basis (requirements, design, implementation, risk analysis).  It transforms general objectives into tangible test conditions and identifies defects like ambiguities or inconsistencies.

- Test design derives and specifies test cases from test conditions, addressing "how to test" by defining inputs and data needed for each test condition.  It refines general things to test into specifics for the component or system.

### Detailed Breakdown of Test Activities

- Test planning includes deciding on suitable test techniques, identifying tasks, and formulating a test schedule.

- Test monitoring and control uses exit criteria to track progress and involves corrective actions (test control) to address deviations from the plan.

- Test analysis involves analyzing the test basis for the appropriate test level, evaluating for defects, identifying features and sets of features to test, and prioritizing test conditions.  It also helps validate whether requirements capture stakeholder needs.

- Test design includes designing and prioritizing test cases, identifying necessary test data, designing the test environment, and capturing bi-directional traceability between test basis, conditions, cases, and procedures.

### Test Implementation and Execution

- Test implementation prepares the testware (work products for planning, designing, executing, evaluating, and reporting) needed for test execution.  It specifies test procedures and sets up the test environment.

- Test execution involves running tests and producing actual results.  Test suites (sets of test cases or procedures) are run according to the test execution schedule.

- Test execution includes recording item identities and versions, executing tests manually or automatically, comparing actual and expected results, analyzing anomalies (differences between actual and expected results), and reporting defects.

- Test completion makes test assets available for later use, leaves the test environment in good condition, and communicates results to stakeholders.  It involves closing defect reports, creating a test summary report, and archiving test assets for reuse.

### Test Work Products

- Work products are documentation, informal communication, or artifacts used in testing.  There is significant variation in types, organization, and naming.

- Examples include test plans, test reports, test conditions, test cases, test procedures, test suites, test execution schedules, defect reports, and test summary reports.

## Traceability Between Test Basis and Test Work Products

### Traceability and Bi-directional Traceability

- Traceability is the degree to which relationships can be established between work products.

- Bi-directional traceability exists between all test work products, allowing for analysis of change impacts, auditing, and measurement of coverage.

### Benefits of Good Traceability

- Analyzing the impact of changes.

- Making testing auditable and measurable.

- Meeting IT governance criteria.

- Improving the coherence of test progress reports.

- Relating technical aspects of testing to stakeholders in understandable terms.

- Providing information to assess product quality, process capability, and project progress.

## Software Development and Software Testing

### The Relationship Between Software Development and Testing

- The software development life cycle model significantly impacts testing.

- Testing organization must fit the development life cycle to deliver benefits.

- For every development activity, there's a corresponding test activity.

- Each test level has specific objectives.

- Test analysis and design should begin during the corresponding development activity.

- Testers should participate in discussions to define and refine requirements and design, reviewing work products as drafts become available.

### Sequential Development Models (Waterfall and V-Model)

- The Waterfall model has testing at the end, making late defect detection a problem. Feedback is difficult, and iterations are challenging.

- The V-model pairs each development phase with a corresponding testing phase, allowing for early testing and demonstrating that testing is not just execution-based.  A common V-model uses four test levels: component/unit, integration, system, and acceptance.

### Iterative and Incremental Development Models

- Most test tasks from sequential models are present in iterative and incremental models, but timing and extent may vary.

- Tasks may not be sequential.

- Fewer entry and exit criteria exist between activities compared to sequential models.

- Common issues include more regression testing, defects outside iteration scope, and less thorough testing.  Examples of iterative and incremental models include RUP, Scrum, Kanban, Spiral, Agile, and XP.

### Agile Development and Testing

- Scrum and XP emphasize testing throughout the process.

- Each iteration culminates in a short testing period, often with independent and business representatives.

- Developers write and run tests, using tools to automate and measure coverage.

- Agile offers benefits (focus on working software, simpler design, test-driven development) and challenges (constant time pressure, increased regression testing importance, less formal test design).  Testers often act as coaches.

### Choosing a Development Model

- Selecting a suitable development model is crucial based on the specific situation or context.

- The context determines test levels and activities.

## Software Testing Methodologies

### White-Box Testing

- Also known as structural, glass-box, or clear-box testing.

- Based on analysis of internal structure (code, data structures, design).

- Code is visible to testers.

- Involves testing for internal security holes, broken code paths, input flow, expected output, conditional loops, and individual statements, objects, and functions.

### White-Box Testing Techniques

- Statement coverage: traversing all statements at least once.

- Decision coverage: reporting true/false outcomes of Boolean expressions.

- Branch coverage: traversing each branch from decision points.

- Condition coverage: covering all individual conditions.

- Multiple condition coverage: testing all possible combinations of condition outcomes.

- Finite state machine coverage: checking visited and transited states and sequences.

- Path coverage: testing all possible paths, covering statements and branches.

### Black-Box Testing

- Also known as behavioral testing.

- Tests functionalities without knowledge of internal structure.

- Focuses on input and output, based on requirements and specifications.

### Types of Black-Box Testing

- Functional testing: related to functional requirements.

- Non-functional testing: related to non-functional requirements (performance, scalability, usability).

- Regression testing: done after code changes to ensure no new defects are introduced.

### Grey-Box Testing

- Tests with partial knowledge of internal structure.

- Identifies defects due to improper code structure or application use.

## Functional, Non-Functional, and Change-Related Testing

### Functional Testing

- Evaluates compliance with functional requirements.

- Tests are based on functions described in documents or understood by testers.

- Performed at all test levels.

- Can focus on suitability, interoperability, security, accuracy, and compliance.

- Two perspectives: requirement-based (using specifications) and business process-based (using knowledge of business processes and use cases).

- Thoroughness is measured by coverage of functions.

- Specialized skills may be needed for specific application domains.

### Non-Functional Testing

- Tests quality characteristics (non-functional attributes).

- Performed at all test levels.

- Includes performance testing (speed, response time, stability, reliability, scalability, resource usage) and load testing (system loading capacity).

- Also includes stress testing (stability and reliability under heavy load), usability testing (ease of use), portability testing (ease of moving between environments), and security testing (vulnerability identification and prevention of attacks).

- Thoroughness is measured by coverage of non-functional elements.

- Specialized skills may be needed (performance or security testing).

### Change-Related Testing

- Addresses changes to software function and/or structure.

- Considers the change itself and its other effects.

- Confirmation testing (re-testing) confirms that defects are fixed and don't cause new failures.

- Regression testing ensures that changes haven't introduced new defects or uncovered existing ones in unchanged areas.

- Both are done at all test levels.

## Test Types and Test Levels

### Test Levels

- Groups of test activities organized and managed together.

- Each level has specific objectives, a test basis, a test object, typical defects, approaches, responsibilities, and a test environment.

### Test Levels and Their Characteristics

- Component testing (module or unit testing): tests individual components.

- Integration testing: tests interfaces and interactions between components or systems.

- System testing: verifies that the whole system meets requirements.

- Acceptance testing: validates the system against user needs, requirements, and business processes.

### Different Forms of Acceptance Testing

- User acceptance testing (UAT): conducted in a real or simulated environment by intended users.

- Operational acceptance testing (OAT): performed in an operational environment by operations staff.

- Contractual acceptance testing: verifies compliance with contractual requirements.

- Regulatory acceptance testing: verifies compliance with laws and regulations.

- Alpha testing: simulated or actual testing in the developer's environment by external roles.

- Beta testing: simulated or actual testing at an external site by external roles.

### Test Level Characteristics Summary

- Objectives, test basis, test objects, and typical defects and failures are summarized for each test level (component, integration, system, acceptance).

### Test Types and Levels

- Each test type (functional, non-functional, white-box) is applicable at every test level.  An example using a banking application illustrates this.

## Static vs Dynamic Testing

### Static Testing

- Tests software without code execution.

- Reviews code, requirements, and design documents to find errors.

- Improves quality by finding early errors.

- Techniques include informal reviews, technical reviews, walkthroughs, inspections, and static code reviews.

### Dynamic Testing

- Executes code.

- Checks functional behavior, memory/CPU usage, and performance.

- Confirms that the software works according to requirements.

- Techniques include unit testing, integration testing, and system testing.

### Key Differences Between Static and Dynamic Testing

- Static testing is done without execution; dynamic testing involves execution.

- Static testing focuses on defect prevention; dynamic testing focuses on finding and fixing defects.

- Static testing performs verification; dynamic testing performs validation.

- Static testing happens before compilation; dynamic testing happens after compilation.

- Static testing techniques are structural and statement coverage-based; dynamic testing techniques include boundary value analysis and equivalence partitioning.

## Summary

### There is no single "one size fits all" testing process.

### Test activities may overlap or occur concurrently.

### Different testing methodologies exist (white-box, black-box, grey-box, functional, non-functional).

# Software Testing Techniques and Their Characteristics

## Black-Box Test Techniques

### Overview of Black-Box Testing

- Black-box testing involves testing software without knowledge of its internal workings.

- It treats the software as a "black box" with inputs and outputs, ignoring internal structure.

- This technique is suitable for all testing levels where a specification exists.

### Characteristics of Black-Box Testing

- Test conditions, cases, and data are derived from a test basis (requirements, specifications, use cases, user stories).

- Test cases can reveal gaps between requirements and implementation, or deviations from requirements.

- Coverage is measured based on items tested within the test basis.

### Black-Box Testing Techniques

- Equivalence Partitioning: Divides test conditions into groups considered the same, testing only one condition per group.

- Boundary Value Analysis: Tests values at the boundaries between partitions, including valid and invalid boundaries.

- Decision Table Testing: Systematically states complex business rules, aiding test case selection and revealing specification issues.

- State Transition Testing: Used when system aspects can be described as a finite state machine, often visualized with state diagrams.

- Use Case Testing: Identifies test cases that exercise the entire system on a transaction-by-transaction basis.

## White-Box Test Techniques

### Overview of White-Box Testing

- White-box testing uses the software's internal structure to derive test cases.

- It's also known as "glass-box" testing, requiring knowledge of the software's implementation.

- Applicable to all testing levels.

### Characteristics of White-Box Testing

- Test conditions, cases, and data are derived from a test basis (code, software architecture, design, etc.).

- Coverage is measured based on items tested within a selected structure (code or interfaces).

- Specifications are used to determine expected test case outcomes.

### White-Box Testing Techniques

- Statement Testing and Coverage: Tests each program statement at least once; also known as line or segment coverage.

- Decision Testing and Coverage: Exercises decisions in the code, testing code executed based on decision outcomes.  This ensures both true and false outcomes of decisions are tested.

## Experience-Based Test Techniques

### Overview of Experience-Based Testing

- Test cases are derived from the tester's skill, intuition, and experience with similar applications.

- Useful for identifying tests missed by more systematic techniques.

- Coverage and effectiveness vary greatly depending on the tester's approach and experience.

### Experience-Based Testing Techniques

- Error Guessing: Anticipates errors based on the tester's knowledge; success depends heavily on tester skill.

- Exploratory Testing: A hands-on approach with minimal planning and maximum execution, focusing on learning about the software.

- Checklist-Based Testing: Uses checklists to guide testing; provides consistency but may lack repeatability due to high-level nature of checklists.

# Static Testing Techniques in Software Quality Assurance

## Static Methods in Software Testing

### Definition and Objective of Static Testing

- Static testing examines software work products manually or with tools without execution.

- It analyzes various documents including source code, design documents, requirement specifications, test plans, and user manuals.

- The primary goal is to improve software quality by helping engineers identify and fix defects early in the development process.

- It begins early in the software development life cycle.

### Types of Defects Easily Found Through Static Testing

- Deviation from standards

- Missing requirements

- Design defects

- Non-maintainable code

- Inconsistent interface specifications

### Documents Testable Through Static Testing

- Business Requirements Document (BRD)

- Functional or system requirements

- Unit use cases

- Prototype and prototype specification documents

- Test data

- Database field dictionary spreadsheets

- Documentation, training guides, and user manuals

- Test cases/test plan strategy documents

- Traceability matrix documents

- Performance test scripts/automation

### Types of Static Methods

- Static testing encompasses two main categories: review and static analysis.

- Review methods include formal and informal approaches.

- Static analysis utilizes tools to assess code quality against standards, identifying defects like unused variables, dead code, infinite loops, variables with undefined values, and syntax errors.

## Benefits of Static Testing

### Cost and Time Savings

- Lowered costs in the initial development phase due to reduced rework for error correction.

- Reduced development time.

- Early feedback improves overall functionality, leading to fewer errors in later testing phases.

- Improved software code maintainability.

- Better understanding of software quality issues for developers.

### Process Improvement

- Automated tools expedite code and document review.

- Enhanced communication between teams.

## Types of Reviews

### Informal Reviews (Buddy Check, Pairing, Pair Review)

- Characterized by detecting potential defects; may also generate ideas or solutions.

- Not based on a formal documented process; may not involve a meeting.

- Can be performed by a colleague (buddy check) or multiple people.

- Results may or may not be documented; usefulness varies depending on the reviewer.

- Checklist use is optional; commonly used in Agile development.

- A simple example is one person asking a colleague for a quick look at their work.

- Other forms include pair programming, where one person continually reviews the other's work as it's being typed.

### Walkthroughs

- Aims to find defects, improve the software product, consider alternative implementations, and evaluate conformance to standards.

- May also exchange ideas, train participants, and achieve consensus.

- Individual preparation is optional; the review meeting is typically led by the author.

- A scribe is mandatory; checklists are optional.

- May use scenarios, dry runs, or simulations; defect logs and review reports may be produced.

- The author does most of the preparation.

- Participants from different departments are not required to study the work product beforehand.

- Useful for higher-level work products like requirement specifications and architectural documents.

- Often used to transfer knowledge and educate a wider audience.

### Technical Reviews

- Aims to gain consensus and detect potential defects.

- May also evaluate quality, build confidence, generate new ideas, motivate authors, and consider alternative implementations.

- Reviewers should be technical peers or experts.

- Individual preparation is required; the review meeting is optional, ideally led by a trained moderator (not the author).

- A scribe is mandatory (ideally not the author); checklists are optional.

- Defect logs and review reports are typically produced.

- Often focuses on achieving consensus on technical content after participants have studied the work product.

- Defects are found by experts focusing on the work product's content.

- Experts may include architects, chief designers, and key users.

- An independent facilitator is useful, especially with conflicting opinions.

- Less formal than inspections but generally more formal than walkthroughs; formality can vary.

### Inspections

- Aims to detect potential defects, evaluate quality and build confidence, and prevent future defects through author learning and root cause analysis.

- May also motivate authors and improve future work products and the development process; achieves consensus.

- Follows a defined process with formal documented outputs, using rules and checklists.

- Clearly defined roles are mandatory, including a dedicated reader who reads/paraphrases the work product aloud.

- Individual preparation is required.

- The most formal review type.

- Work products are thoroughly prepared and checked by reviewers before the meeting using rules and checklists.

- Defects are logged in the meeting; discussion is postponed until later.

- Inspections can balance multiple goals (e.g., time to market and efficiency).

- When done well, inspections identify defects and improve processes, benefiting both authors and reviewers.

## Summary of Static Testing

### In static testing, software products and source code are examined without execution to identify issues.

### Static testing starts early in the software development life cycle.

### The static testing techniques discussed are informal review, walkthrough, technical review, and inspection.

# Software Quality Assurance: 5 Levels of Testing

## Functional Testing

### Overview of Functional Testing

- Functional testing validates software against functional requirements and specifications.

- Its main purpose is to test each function by providing input and verifying the output against functional requirements.

- It can be done manually or using automation, checking aspects like user interface, APIs, databases, and security.

### Component/Unit Testing

- Also known as "unit" or "module" testing, it searches for defects and verifies the functioning of separately testable software items.

- Goals include reducing risk, identifying defects, validating performance, developing confidence in quality, and preventing defects from escaping to higher levels.

- It may be done in isolation using "mock objects," "stubs," and "drivers" to simulate interfaces.  A stub is called from the component, while a driver calls the component.

### Integration Testing

- Integrates software modules and tests them as a group.

- Aims to find issues in how modules interact when combined.

- Includes component integration testing (focusing on interactions between components, performed after component testing, often automated, and the responsibility of developers) and system integration testing (focusing on interactions between systems, packages, and microservices; may involve external organizations; often the responsibility of testers).

### System Testing

- Concerned with the behavior of the whole system/product.

- May include tests based on risks, requirement specifications, business processes, and use cases.

- Objectives include reducing risk, verifying compliance with requirements, validating completeness, building confidence in overall quality, finding defects, and preventing defects from escaping to later testing or production.

### User Acceptance Testing

- Conducted in a real or simulated operational environment by intended users.

- Aims to build confidence that the system enables users to perform tasks efficiently.

- Includes types like Contract Acceptance Testing (CAT), Regulations Acceptance Testing (RAT), Operational Acceptance Testing (OAT), and Alpha and Beta testing.

## Non-Functional Testing

### Overview of Non-Functional Testing

- Evaluates compliance of a component or system with non-functional requirements.

- Characteristics include measurability (no subjective characterization), correct identification of quality attributes, and prioritization of requirements.

- Parameters include interoperability, performance, scalability, security, loading capacity, stability, and reliability.

### Interoperability Testing

- Ensures software interacts with other components and systems.

- Proves end-to-end functionality between communicating systems as specified by requirements.

- Includes data type, semantic, physical, protocol, and data format interoperability testing.  It is particularly significant for systems based on the Internet of Things (IoT), web services, systems of systems, and commercial off-the-shelf (COTS) software.

### Performance Testing

- Determines the actual system performance compared to expectations.

- Metrics vary by application, testing speed, response time, stability, reliability, scalability, and resource usage.

- Aims to identify and eliminate performance bottlenecks.

### Stress Testing

- Evaluates behavior under extremely heavy load.

- Ensures acceptable performance under worst-case conditions; recovery mechanisms should be invoked if limits are exceeded.

- Targets problems like memory leaks and buffer allocation/memory carving.  Testing from different locations (inside and outside the system) is recommended.

### Regression Testing

- Verifies that no defects are introduced into unchanged portions of a system due to changes elsewhere.

- Addresses scenarios where a reported defect is fixed, not fixed, fixed but something else fails, or not fixed and something else fails.

- Since testing every case for every version is expensive, a subset of test cases is carefully selected to maximize defect uncovering and reduce costs.

## Documentation Testing

### Documentation Testing Overview

- Verifies technical accuracy and readability of user manuals, tutorials, and online help.

- Levels include read tests (reviewing for clarity, organization, and accuracy without execution), hands-on tests (exercising online help and verifying error messages), and functional tests (following instructions to verify system functionality).

- Concrete tests include verifying grammar, terminology, graphics, glossary standards, indexes, internal consistency, and the equivalence of online and printed versions.  It also includes verifying troubleshooting guides, installation procedures, and configuration sections.

# Software Testing Life Cycle (STLC)

## Requirements Analysis/Design

### High-Level Requirement Analysis

- This phase begins when the Software Requirements Document is ready and shared with stakeholders.

- The testing team identifies testing requirements, including scope, verification and validation key points, and time estimations.

- It's crucial to identify the expected timeframe for each functionality.

### Scope Definition

- Defines the scope of testing at a high level, breaking it down into several functional modules.

- Identifies the needed types of testing.

- Analyzes and identifies prerequisites and testing environment details.

### Requirement Traceability Matrix (RTM) Preparation

- Requirement tracing documents the links between requirements and work products developed to implement and verify those requirements.

- The RTM maps and traces user requirements with test cases.

- This ensures traceability and helps in managing requirements throughout the testing process.

### Automation Analysis

- Analyzes the scope of automation for regression testing.

- Plans the automation tool, functionalities to be automated, timeframe, and resource allocation.

- This helps in identifying areas where automation can improve efficiency and reduce testing time.

## Entry and Exit Criteria

### Entry Criteria

- Conditions or documents needed to start a specific STLC phase.

- Tasks are only performed if these conditions are met.

- Defining a timeframe for entry criteria is ideal.

### Common Entry Criteria

- Requirements are defined and approved.

- Complete or partially testable code is available.

- Test data and test cases are available.

- The testing environment is completely set up.

### Common Entry Criteria for Unit Testing

- The planning phase is completed.

- System design, technical design, and other relevant documents are reviewed and approved.

- Business and functional requirements are defined and approved.

- Testable codes or units are available.

- The test environment is available.

### Exit Criteria

- Items, documents, actions, or tasks that must be completed before concluding an STLC phase and moving to the next.

- A set of expectations for a particular phase.

- Defining a timeframe for exit criteria is ideal.

### Common Exit Criteria

- Deadlines are met.

- All test cases are executed.

- Sufficient coverage of requirements and functionalities is achieved.

- All identified defects are corrected and closed.

- No critical bugs are left unresolved.

### Common Exit Criteria for Unit Testing

- Unit tests are successfully executed.

- All identified bugs are fixed and closed.

- The project code is completed.

## Test Planning

### Defining Test Specifications

- Defines test specifications to meet project requirements.

- The main objective is to prepare a Test Plan document.

- This document outlines the testing strategy, resources, environment, limitations, and schedule.

### Test Plan Document

- Usually prepared by the Quality Assurance Team Lead or Manager.

- Focuses on data and information related to the application.

- Answers key questions like "What is to be tested?" and "What resources are required?".

### Entry and Exit Criteria for Test Planning

- Entry criteria include providing requirements documents along with the RTM and an automation feasibility report (if automation is in scope).

- Exit criteria include completing the Test Plan Document and Test Effort Estimation document.

- Major aspects include scope of deliverables, effort estimation, and resource planning.

## Test Case Design and Development

### Test Case Preparation

- The main objective is to prepare test cases for individual units.

- Test cases cover functionality, verification, and validation points mentioned in the Test Plan.

- They are written by the QA team and signed off by a Business Analyst after review.

### Entry Criteria for Test Case Development

- Activities in Test Planning are finished.

- The Test Plan is ready.

### Exit Criteria for Test Case Development

- Test cases are signed off.

- Test data is ready.

- Test scripts are prepared if automation is in scope.

### Activities in Test Case Development

- Test Scenarios Identification:  Simplifies testing and evaluation of complex systems. Strategies include enumerating possible users and their actions, evaluating users with a hacker's mindset, listing system events and how the system handles them, and studying similar systems and their behavior.

- Test Cases Writing: A test case includes test data, preconditions, expected results, and post-conditions.  It verifies compliance against specific requirements and serves as the starting point for test execution. Good test cases are simple, transparent, have 100% coverage, are identifiable, align with client expectations, and are regularly revised and updated.

- Test Data Preparation: Used to execute tests on the test platform. Data should be precise and exhaustive to uncover defects. It can be created manually or using automation methods and should have high coverage and be regularly updated.

## Test Environment Setup

### Test Environment

- Contains elements supporting test execution, including software, hardware, and network configurations.

- It's a combination of hardware and software environments for executing tests.

- This phase includes hardware configuration, operating system settings, software configuration, test terminals, and other support.

### Activities in Test Environment Setup

- Design Test Environment: Checks if archiving is needed for backups, verifies network configuration, identifies required server operating systems, databases, and other components, and identifies the number of licenses needed.

- Environment Set Up: Analyzes setup requirements, prepares software and hardware requirements, and gets official confirmation for the test environment setup.

- Smoke Testing: Validates the test environment's stability and prevents wasting time and resources on deeper tests with a broken product.

## Defect Life Cycle

### States of a Defect Life Cycle

- New: A potential defect raised but not yet validated.

- Assigned: Assigned to a development team for checking.

- Active: The defect is being addressed by the developer. Possible outcomes are deferred or rejected.

- Test/Fixed/Ready for Retest: The defect is fixed and ready for retesting.

- Verified: The defect is retested and verified by QA.

- Closed: The final state; closed after QA retesting or if it's a duplicate or not a defect.

- Reopened: An unfixed defect reactivated or reopened by QA.

- Deferred: A defect that cannot be addressed in the current cycle and is deferred to a future release.

- Rejected: A defect rejected because it's a duplicate, not a defect, or non-reproducible.

## Defects Classification

### Priority and Severity

- QA team perspective: Priority (order of resolving defects).

- Development perspective: Severity (complexity of fixing the code).

- QA sets priority and timeframe based on end-user requirements.

### Priority Categories

- Low: Defects fixed after critical defects.

- Medium: Defects resolved in subsequent builds.

- High: Defects solved immediately due to considerable impact on application functionality.

- Urgent: Defects resolved immediately due to severe impact, rendering the product unusable.

### Severity Categories

- Severity is the impact of the defect on the application and the complexity of fixing it from a development perspective.

- It's determined by how crucial the defect is to the system.

- Severity status indicates the deviation in functionality due to the defect.

### Severity Listings

- Critical/Severity 1: Impacts crucial functionality; QA cannot continue validation without fixing it (e.g., frequent app crashes).

- Major/Severity 2: Impacts a functional module; QA can continue validating other modules (e.g., flight reservation not working).

- Medium/Severity 3: Issue with a single screen or function; system still functions (e.g., ticket number format incorrect).

- Low/Severity 4: Does not impact functionality; cosmetic defect or UI inconsistency (e.g., mismatched button colors).

## Test Execution

### Objectives

- Ensure no bugs or issues exist in the application; it's "fit for purpose".

- Unit and integration testing are performed, comparing expected and actual results.

- Identified defects are corrected until all tests pass.

### Activities in Test Execution

- Testers execute tests, log defects, and communicate progress to the test manager.

- Test status is communicated to management; the development team resolves defects and produces new releases.

- The testing team retests failed test blocks and performs regression testing to confirm main functionality is maintained.

### Entry Criteria for Test Execution

- Test Plan is complete.

- Test Cases Development Phase is complete.

- Test data is available.

### Exit Criteria for Test Execution

- All test cases are successfully validated.

- Defects are deferred.

- Test case execution is complete.

- A Defect Summary Report is available.

### Main Activities in Test Execution

- System Integration Testing (SIT): A black box testing technique evaluating system compliance against requirements/test cases. Usually performed on a subset of the system.  Can be performed with minimal testing tools; interactions and data field behavior are investigated. After integration, data flow is checked in the integration, database, and application layers.

- Defect Reporting: A process of finding defects by testing or recording feedback; new versions fix defects based on client feedback. Managing, evaluating, and prioritizing defects is challenging.

- Defect Mapping: Once a defect is reported and logged, it's mapped with failed/blocked test cases and corresponding requirements in the RTM. This helps create proper defect reports and analyze impact. Stakeholders decide whether to fix or defer based on priority and severity.

- Re-testing: Executing a previously failed test after a defect is fixed to check if the problem is resolved.

- Regression Testing: Re-executing tests impacted by code changes. Types include final regression tests (validating unchanged builds) and regression tests (verifying that code changes haven't broken other parts of the application).

## Test Closure

### Final Phase

- The final phase of the STLC.

- Completeness is ensured by checking against test exit criteria and product quality measurement against test completion criteria.

### Entry Criteria for Test Closure

- Test case execution is complete.

- Test results are available.

- Defects report is available.

### Exit Criteria for Test Closure

- Test closure reports are provided.

- Matrices are prepared (to be signed by clients).

### Main Activities in Test Closure

- Test Completion Reporting: Summarizes test metrics to update stakeholders, enabling informed decisions. The report includes the test summary report identifier, summary, variances, summary results, evaluation, planned vs. actual efforts, and sign-off.

- Test Completion Matrix Reporting: Upon completion, various matrices are collected to prepare test reports.

- Availability of Test Results: Articulates test results (screenshots, database query results, recordings, log files).  These are saved during test case execution, re-testing, and regression testing, and included in test closure documents.

# Software Quality Assurance: Quality Control, Metrics, and Test Reporting

## Test Monitoring and Control

### Objectives of Test Monitoring and Control

- Monitor the test plan and schedule to stay on track.

- Monitor key project parameters.

- Conduct progress and milestone reviews to determine the actual status and replan as needed.

- Monitor risks and take appropriate action.

- Analyze issues and change requests, taking appropriate action.

- Track corrective actions to closure.

- Monitor resources and manage resource issues.

- Report the test status to management.

### Responsibilities in Test Monitoring and Control

- The test manager is responsible for monitoring and control, ensuring appropriate corrective action is taken to address risks and issues.

- Regular status reports communicate testing progress to stakeholders.

- Test monitoring and control provide feedback and visibility on test operations, including corrective action when performance deviates from expectations.

### Sample Process Map for Test Monitoring and Control

- The process involves monitoring progress against the plan, identifying risks/issues, managing corrective actions, and ensuring all actions are closed.  This is a cyclical process.

## Metrics Used in Testing

### Defining Metrics in Testing

- Metrics provide quantitative answers to specific questions, offering an objective view of goal attainment.

- A variety of test and business metrics provide visibility into key areas and demonstrate how metrics facilitate improvement.

### Customer Satisfaction Metrics

- Monthly quality or operational reviews reveal improvement patterns in metrics over time.

- Sample metrics include customer satisfaction, project management of testing, execution of testing, customer care, and cost of quality.

- Charts illustrate customer satisfaction surveys, showing arrival rates and satisfaction levels across different customers and various aspects of the software (quality, timeliness, ease of use, etc.).  Numerical interpretations are provided to clarify the meaning of the scores.

### Project Management Metrics for Testing

- Metrics provide visibility into the test manager's effectiveness in completing testing on time, within budget, and with the right quality.

- Charts show schedule accuracy (planned vs. actual) and effort estimation accuracy (planned vs. actual) across different projects.

- Timeliness metrics are lagging indicators, showing on-time delivery after the testing is complete.  Careful tracking of activities is necessary to address slippage or delays.  Effort estimation is a key component in calculating cost and scheduling.

### Test Execution Metrics

- Metrics provide visibility into the testing process.

- Charts illustrate the number of defects and change requests, their severities, and their status (open, closed).

- Charts also show the age of open defects, problem arrival rates, and phase containment effectiveness.  The goal is to minimize defects found after acceptance testing and product release.  Cumulative arrival rate curves indicate product stability.  Charts also show the arrival and closure rates of problems, indicating project stability and effectiveness in resolving defects.  Another chart shows the status of problems (raised, open, closed) but not their severity.

## Customer Care Metrics

### Goals and Metrics for Customer Care

- Customer care aims to respond efficiently and effectively to customer problems, ensure high service standards, and ensure reliable product function at customer sites.

- Metrics track effectiveness in resolving customer queries, the number of queries raised, system availability at customer sites, and the age of open queries.

- A customer query may lead to a defect report if a software problem is identified.

### Customer Care Charts and Analysis

- Charts show the arrival and closure rates of customer queries, highlighting potential backlogs.

- Charts also present outage information, showing the customers impacted and the duration of outages.  Post-mortems are conducted to prevent recurrence.

- Metrics track system availability and outage time per month.

## Cost of Quality

### CMMI Maturity and Cost of Poor Quality

- Metrics apply to various organizational areas, including CMMI maturity and the cost of poor quality (COPQ).

- A chart shows internal CMMI maturity, using a 1-10 scale to rate process areas. A score of 7 or higher indicates satisfaction.

- According to Crosby, the most meaningful quality measurement is the cost of poor quality (COPQ).  Improvement activities should focus on reducing COPQ.

### Components of Cost of Quality

- COPQ includes the cost of external and internal failure, the cost of preventative infrastructure, and the cost of verification infrastructure.

- A chart shows the cost of quality over time, broken down into external, internal, prevention, appraisal, and total costs.

## Purposes, Contents, and Audiences for Test Reports

### Test Report Purpose and Frequency

- A test report summarizes all test activities and final results of a testing project.

- Reporting frequency is defined in the project test plan or communication plan; IEEE standard 829 provides guidance for test summary reports.

### Test Report Content and Audience

- Test reports advise management and stakeholders on testing status, including key project information (summary of activities and results, completed deliverables, new risks and issues, schedule/effort/budget status, key risks and issues, milestone status, and planned activities/deliverables).

- The test manager discusses the report with management, presenting the current status, key risks, and issues, and explaining how issues are being addressed and risks managed.

- Management considers the test manager's plans for dealing with risks and issues, providing support.

- The project manager presents a recovery plan (exception report) if the project deviates significantly from its defined tolerance.

## Summary of Testing Metrics and Reports

### Testing metrics estimate progress and quality in software testing.

### Various metrics measure software quality, considering key risks and issues.

### Metrics track quality, timeliness, cost, schedule, and effort.

### They provide an internal view of software quality; external behavior requires further examination.

### Test reports are crucial for determining software readiness for customer release.

# Software Quality Assurance: Test Automation

## Introduction to Test Automation

### What is Test Automation?

- Automation testing uses software tools to develop and execute tests.

- Tools input test data, compare expected and actual results, and generate reports.

### Why Automate Software Testing?

- Improves accuracy, quality, and test coverage.

- Makes test execution faster.

### When to Automate

- Regression testing:  Suitable when the software application is stable.

- Smoke testing: Provides a quick high-level assessment of software build quality.

- Static & Repetitive Tests: Automates unchanging, repetitive tasks.

- Data Driven Testing: Validates functions with numerous data sets.

- Load & Performance Testing: No viable manual alternative.

### Which Tests to Automate?

- Business critical test cases and critical flows.

- Smoke tests to determine software stability.

- Tests difficult to perform manually (complex calculations, tedious steps).

- Stable test cases or modules (avoid automating unstable components).

### Types of Automation Tests

- Functional Automated Tests: Verify software fulfills business requirements (Tools: Selenium, UFT, RFT, VSTS).

- Non-Functional Automated Tests: Test non-functional requirements (performance, security, compliance) (Tools: Jmeter, LoadRunner).

## Choosing the Right Test Automation Tool

### Key Factors in Tool Selection

- Compatibility with platforms and technologies (operating systems, application types, mobile platforms).

- User-friendliness and flexibility for testers of all skill levels (keyword testing vs. scripting).

- Features like record-and-playback and checkpoint verification.

- Ability to create maintainable and reusable tests adaptable to UI changes.

- Integration with existing ecosystem (CI/CD pipeline, test management, defect management, source control).

- Ability to test enterprise applications (SAP, Oracle, Salesforce, Workday).

### Steps for Choosing a Tool

- Step 1: Identify Requirements (project scope, testing needs, desired functionalities).

- Step 2: Evaluate Tools and Vendors (consider gathered information, create a shortlist).

- Step 3: Estimate Cost and Benefit (perform cost-benefit analysis for shortlisted tools).

- Step 4: Make the Final Decision (test the tool in a real-world setting, schedule meetings with the project team and consultants).

## Effective Use of Test Automation Tools

### Training the Testing Team

- Provide training on automation concepts, terminology, and the chosen tools.

- Familiarize external automation architects with the product, manual testing process, and organizational expectations.

- Allow time for experimentation and finding the most effective automation strategy.

- Provide training on existing organizational tools (bug tracking, requirements management).

- Ensure effective communication between manual testers, developers, and the automation team.

### Creating the Test Automation Framework

- The automation architect develops a long-term framework to support automated testing.

- The framework provides guidelines and strategies for creating easily maintainable test scripts.

- Different framework types exist: linear, modular, data-driven, keyword-driven, hybrid.

### Developing an Execution Plan

- Choose appropriate execution environments (operating system, browser, hardware).

- Write scripts to run on multiple browsers if necessary.

- Communicate environment details before scripting.

- Specify who will execute the scripts (automation team, developers, dedicated resource, unattended mode).

### Writing Test Scripts

- Write scripts in an orderly fashion, using proper naming conventions.

- Maintain source code in source control for version control and history.

- Follow best programming practices.

### Reporting

- Use the tool's reporting feature or develop custom reporting mechanisms (e.g., automated emails).

- Generate reports (charts, tables) as needed.

- Keep management informed about test case coverage (automated vs. remaining manual tests).

### Maintenance of Test Scripts

- Maintenance is usually easy with best practices and a good framework.

- Update scripts immediately if application changes occur.

- Poor frameworks and lack of best practices make maintenance difficult and can cause project failure.

- Automation architects are expensive due to their expertise in creating robust and maintainable frameworks.

## Test Automation Environments

### Test Automation Environments Explained

- A test environment (or test bed) combines software and hardware for testing.

- It may include test data.

- Establishing the right environment is crucial for success; mistakes lead to extra costs and work.

### Components of a Test Environment

- Systems and applications

- Test data

- Database servers

- Client operating systems

- Browsers

- Server operating systems

- Hardware

- Networks

- Necessary documentation (reference documents, configuration guides, installation guides, user manuals)

### Process of Software Test Environment Setup

- Tests are limited by what can and cannot be tested.

- Involved personnel: System admins, developers, testers, sometimes users or techies.

- Setup involves various distinct areas.

### Steps in Test Environment Setup

- Step 1: Test Server Setup (not all tests run on local machines; may need a test server).

- Step 2: Network Setup (internet, LAN/WiFi, private network to avoid impacting other teams).

- Step 3: Test PC Setup (configure PCs according to application needs; different OS and browsers).

- Step 4: Bug Reporting Tools (provide testers with bug reporting tools).

- Step 5: Creating Test Data (duplicate production data for testing, anonymize sensitive data).  Anonymization methods include blacklist and whitelist approaches.  Obtain data strategically using SQL scripts.

### Test Environment Management

- Involves managing and maintaining the test environment.

- Activities include: maintaining a central repository, managing environments based on team needs, establishing new environments, removing outdated ones, investigating issues, coordinating resolutions.

### Challenges in Test Environment Management

- Inadequate resource planning (negative impact, conflicts).

- Remote environments (geographic location issues, support team dependency).

- Elaborate setup time (complex setups for integration testing).

- Shared usage by teams (concurrent use can corrupt results).

- Complex test configurations (intricate configurations can be challenging).

### Best Practices for Test Environment Management

- Thoroughly understand and communicate test requirements.

- Verify connectivity before testing.

- Ensure necessary hardware, software, licenses, browsers, and versions are available.

- Plan scheduled use of the environment, automation tools, and configurations.

## Manual Testing vs. Test Automation

### This section compares manual and automation testing across several criteria: accuracy, testing at scale, turnaround time, cost efficiency, user experience, areas of specialization, and user skills.  A table summarizes the key differences.

## Benefits and Risks of Test Automation

### Advantages of Test Automation

- Speed (faster than manual testing).

- Reliability (consistent results).

- Repeatability (easy to repeat tests).

- Coverage (increased test coverage).

- Reusability (tests can be reused across application versions).

### When Test Automation is Beneficial

- Long-run projects (cost-effective for long-term maintenance).

- Many regression tests (reusability is valuable for constantly changing code).

- Time-consuming and complex manual tests (impractical to manually test all features).

- Fairly stable applications.

### Risks of Automation Testing

- Overly ambitious or impractical expectations.

- Overlooking the capabilities of human testers.

- Incorrectly estimating time and effort (tool selection, training, procedure adjustments, maintainability).

- Incompatibility of tools with the test environment.

- Project budget issues.

- Vendor issues (lack of support, unavailable updates, vendor liquidation, free tools becoming licensed).

## Test Tool Considerations

### This section lists licensed and open-source test automation tools (Appium, Tellurium, QTP, Test Complete, Win Runner, Rational Functional Tester, VSTS, Silk Test, Testim, Selenium, Jmeter, Open STA, SoapUI) and provides brief descriptions of some commonly used tools (Appium, QTP, Selenium, TestComplete, Testim).

# XML Based Test Automation in Selenium

## Introduction to XML Path in Selenium

### What is XPath?

- XPath is an XML path language used for navigating through the HTML structure of a webpage.

- It's a syntax for locating any element on a webpage using XML path expressions.

- It leverages the HTML DOM structure to find elements.  If standard locators (id, class, name) fail, XPath is used.

### XPath Syntax

- XPath contains the path of an element on a webpage.

- The basic format is:  Xpath=//tagname[@Attribute='Value']   where  tagname  represents the element type,  Attribute  is an attribute of the element, and  Value  is the attribute's value.

### XPath Locators in Selenium

- Selenium uses various locators to find elements.

- These include ID, Classname, Name, Link text, XPath, and CSS path.

- XPath is particularly useful for finding dynamic elements and traversing between elements.  CSS path is used for elements lacking name, class, or ID.

### Types of XPath

- Absolute XPath: The complete path to an element starting from the root node.

- Relative XPath: A shorter, more flexible path starting from an element within the DOM, not the root node.

## Absolute XPath

### Characteristics and Disadvantages

- Absolute XPath directly locates elements.

- It begins with a single forward slash ( / ), indicating selection from the root node.

- A major disadvantage is that it fails if the element's path changes.

### Identifying Absolute XPath in Chrome

- Right-click the element and select "Inspect."

- Right-click the highlighted HTML element and select "Copy XPath."

- Paste the copied XPath into the search bar and press Enter; the relevant element will be highlighted.

### Example of Absolute XPath

- An example of an absolute XPath is:  /html/body/div[1]/section/div[1]/div/div/div/div[1]/div/div/div/div/div[3]/div[1]/div/h4[1]/b 

## Relative XPath

### Characteristics and Advantages

- Relative XPath starts from the middle of the HTML DOM structure.

- It uses a double forward slash ( // ).

- It avoids lengthy paths by starting from a middle element.

- Elements are found by searching the relative XPath in the browser's inspect tool.

### Example of Relative XPath

- An example is:  //*[@class='featured-box']//*[text()='Testing'] 

## Finding Elements using Attributes with XPath

### Basic XPath Expressions

- XPath expressions select nodes based on attributes like ID, Name, and Classname.

- Examples include:  //input[@type='text'] ,  //label[@id='message23'] ,  //input[@value='RESET'] ,  //a[@href='http://demo.guru99.com/'] .

### Contains() Method

-  Contains()  is used when attribute values change dynamically (e.g., login information).

- It finds elements with partial text matches.  For example, if the 'name' attribute is 'btnLogin', using  contains(@name, 'btn')  will find it.

### Using OR and AND Expressions

- OR expressions find elements if any condition is true.  Example:  //*[@type='submit' or @name='btnReset'] 

- AND expressions require both conditions to be true. Example:  //input[@type='submit' AND @name='btnLogin'] 

### Starts-with() Function

-  Starts-with()  finds elements whose attribute values change dynamically on refresh or other operations.

- It matches the starting text of an attribute.  It can also find elements with static attribute values.

### Text() Function

-  Text()  is a built-in Selenium function to locate elements based on their text content.

- The text must be in string form.  Example:  //td[text()='UserID'] 

### XPath Axes

- XPath axes are methods to find dynamically changing elements.

- They search different nodes in an XML document from the current context node.

- Common axes include Child, Parent, Ancestor, Sibling, Preceding, Self, Following, Following-sibling, and Descendant.

### Following Axis

- Selects all elements in the document after the current node.

- Example:  //*[@type='text']//following::input 

### Ancestor Axis

- Selects all ancestor elements (grandparent, parent, etc.) of the current node.

- Example:  //*[text()='Enterprise Testing']//ancestor::div[1] 

### Child Axis

- Selects all children elements of the current node.

- Example:  //*[@id='java_technologies']//child::li[1] 

### Preceding Axis

- Selects all nodes that come before the current node.

- Example:  //*[@type='submit']//preceding::input[1] 

### Following-sibling Axis

- Selects the following siblings of the context node (at the same level).

- Example:  //*[@type='submit']//following-sibling::input 

### Parent Axis

- Selects the parent of the current node.

- Example:  //*[@id='rt-feature']//parent::div[1] 

### Self Axis

- Selects the current node itself.

- Example:  //*[@type='password']//self::input 

### Descendant Axis

- Selects all descendants of the current node.

- Example:  //*[@id='rt-feature']//descendant::a 

## Summary

### XML Path is used to find and operate on web page elements.

### XPath has absolute and relative types.

### XPath axes methods find dynamic elements, and XPath expressions select nodes based on attributes.

# Automated Testing Suites for Web Applications

## Introduction to Automated Testing Suites

### Defining Automated Testing

- Automated testing uses software tools to automatically run tests on software applications.

- It efficiently tests complex user interactions and business logic across multiple browsers and devices.

- It streamlines the testing process for complex web applications, reducing issues associated with manual testing.

- It caters to unique configurations of different browsers and devices.

- Automated testing suites are crucial for modern software development, especially for web applications.

### Popular Automated Testing Suites

- Many automated testing frameworks and tools exist, each with unique properties.

- Popular suites include Selenium, Cypress, TestCafe, and Puppeteer.

- Selenium is a widely used open-source suite supporting multiple programming languages (Java, Python, C#, JavaScript, Ruby).  It's used for functional, regression, and browser compatibility testing.

- Cypress is a JavaScript-based framework providing a complete end-to-end testing experience with real-time reloading, automatic waiting, and debugging tools.

- TestCafe is a JavaScript-based framework focusing on cross-browser testing and parallel test executions, handling complex user interactions and workflows.

- Puppeteer is a Node.js based framework for testing complex user interactions and workflows, including headless testing, network traffic interception, and PDF generation.

## Types of Automated Testing for Web Applications

### Unit Testing

- Focuses on individual units or components of an application in isolation.

- For web applications, this involves testing individual functions or methods within a module or component.

- Unit tests are executed as part of continuous integration or the build process to prevent bugs.

### Integration Testing

- Tests how different components or modules of an application work together.

- For web applications, this tests how the front-end interacts with the back-end server and database, and how microservices interact.

- Integration testing is executed as part of continuous integration or deployment to ensure the application functions correctly.

### End-to-End Testing

- Tests the entire application workflow from start to finish.

- For web applications, it simulates user interactions (clicking buttons, navigating pages).

- These tests are executed manually or using automated testing suites to ensure the application works as expected from the user's perspective.

## Introduction to Selenium

### Selenium Overview

- Selenium is a free and open-source test automation suite widely used in web applications.

- It supports test automation across different browsers, platforms, and programming languages.

- It simulates common end-user activities (entering text, selecting drop-down values, checking boxes, clicking links).

- It provides a common interface for major browser technologies.

### Selenium Suite Components

- Selenium WebDriver: Creates robust, browser-based regression automation suites and tests; scales and distributes scripts; provides language-specific bindings and drivers for different browsers.

- Selenium IDE: A Chrome, Firefox, and Edge add-on for simple record-and-playback of browser interactions; simplifies testing for users with limited programming experience.

- Selenium Grid: Enables distributed parallel running of Selenium tests across multiple remote machines; facilitates scaling and managing multiple environments from a central point.

- Selenium Remote Controller: (Currently unavailable) Previously used to inject JavaScript code into the browser for automation.

## Architectures and Layers of Automated Testing Suites

### Types of Architectures

- Record and Playback: Records user interactions and generates automated tests; simple but can be brittle with complex applications.

- Keyword-driven: Uses predefined keywords and commands to interact with the application and build test cases; more flexible than record and playback but requires more planning.

- Data-driven: Useful for applications requiring many input combinations; tests use input data to drive the testing process.

- Modular: Useful for complex web applications; tests are broken down into smaller, independently testable modules.

- Page Object Model: Tests web pages through objects representing page elements; simplifies writing and maintaining automated tests for complex web applications.

- The choice of architecture depends on the web application's needs and the testing team's preferences.  A well-designed architecture improves quality, reliability, and reduces testing time and resources.

### Layers in Automated Testing Suite Architectures

- Test Layer: Where actual test cases (end-to-end, unit, integration) are created; tests are written in a scripting or programming language.

- Automation Layer: Executes test cases; interacts with the web application mimicking user behavior; accesses the user interface and database through libraries and APIs.

- Framework Layer: Provides structure for planning and carrying out test operations; includes elements for test data management, configuration, and reporting; assists with test planning, ranking, and administration.

## Recorders in Automated Testing Suites

### Introduction to Recorders

- Recorders are essential tools for recording user interactions and automatically generating test scripts.

- They speed up testing, reduce errors, and ensure accurate results.

- They automate test script generation, saving time and effort.

- They produce more accurate test cases reflecting real user behavior.

- They reduce errors and inconsistencies in test scripts.

- Common recorders include Selenium IDE and Katalon Recorder.

### Selenium IDE

- A browser plugin offering a simple interface for recording and playing back test scripts.

- It's an easy-to-use browser extension recording user actions using Selenium commands.

- Available for Google Chrome, Mozilla Firefox, and Microsoft Edge.

### Katalon Recorder

- A Selenium-IDE compatible record and playback tool for browser automation testing.

- Used to record, debug, execute, and manage test cases.

- Exports test suites to multiple programming languages (C#, Java, Python, Ruby).

- Its user interface includes a main toolbar, Test Explorer, Test Case Detail View, and Log/Reference/Variable/Self-healing sections.

### Limitations of Recorders

- Recordings may not capture all aspects of user behavior; manual or code-based testing may be necessary.

- Some user interactions may not be captured, leading to incomplete or inaccurate test cases.

- Recorded scripts may require customization to fit specific web application needs.

### Best Practices for Using Recorders

- Use recorders as part of a comprehensive testing approach (manual and code-based testing).

- Regularly review and update recorded scripts to ensure accuracy and effectiveness.

- Customize recorded scripts to fit the specific needs of the web application being tested.

## Working with Selenium API

### Overview of Selenium API

- A suite of tools and libraries for automating web browsers.

- Provides a powerful and flexible framework for automating testing tasks.

- Reduces testing time and improves accuracy.

- Selenium WebDriver is its most widely used component.  Setting it up involves installing drivers, configuring the environment, and importing libraries.

### Selenium API: Locating Elements

- Locators find elements on a web page (buttons, form fields).

- Types of locators include ID, name, class name, tag name, link text, and partial link text.  Examples include  find_element_by_id ,  find_elements_by_class_name ,  find_element_by_xpath .

### Selenium API: Interacting with Elements

- Actions interact with elements (clicking buttons, filling forms, navigating links).

- The Action class handles keyboard and mouse events in Selenium WebDriver.

- Mouse actions include  doubleClick ,  clickAndHold ,  dragAndDrop ,  moveToElement ,  contextClick .

- Keyboard actions include  sendKeys ,  keyUp ,  keyDown .

### Selenium API: Handling Windows and Frames

- Web pages may contain multiple windows and frames, making automation challenging.

- Techniques include methods for switching between windows and frames, or interacting with elements within frames.

- A window handle uniquely identifies and holds the address of all windows.

### Selenium API: Executing JavaScript

- Selenium executes JavaScript within the browser for interacting with elements or manipulating the page.

-  JavaScriptExecutor  is an interface for executing JavaScript with Selenium.

-  executeScript  executes the test script in the context of the currently selected window or frame.

-  executeAsyncScript  executes asynchronous JavaScript.

- Getting started involves importing packages, creating a reference, and calling methods.  Examples are provided for clicking buttons, sending text, and interacting with checkboxes.

### Selenium API: Working with Wait Commands

- Wait commands ensure elements are loaded before interacting with them.

- When a page loads, elements load at different times; wait commands pause the script.

- Types of wait commands include implicit waits, explicit waits, and fluent waits.  Examples and code snippets are provided.

### Selenium API: Handling Alerts and Pop-ups

- Web pages may contain alerts or pop-ups requiring user interaction.

- Techniques include methods for accepting or dismissing alerts, or interacting with elements within pop-ups.

- Alert types include simple, prompt, and confirmation alerts.

- Popups are windows that display on the screen due to certain activity.  Selenium has designated methods for handling alerts and popups.

### Best Practices for Working with Selenium API

- Use a consistent coding style for readability and maintainability.

- Write modular code for flexibility and easier maintenance.

- Use debugging tools to identify and fix errors efficiently.

## Summary

### Automated testing suites are powerful tools for ensuring software quality, reducing testing time and effort, and increasing test coverage.

### Various types of automated testing exist (unit, integration, end-to-end).

### Different automated testing tools offer various features and capabilities.

### Popular suites include Selenium, TestCafe, and Cypress.

### Careful planning and execution of automated testing are crucial for effectiveness and efficiency.

### Automated testing is an essential component of modern software development, improving software quality and customer satisfaction.

# Continuous Integration (CI) and Continuous Delivery (CD) with Jenkins and Git

## Continuous Integration (CI) and Continuous Delivery (CD)

### Understanding CI and CD

- CI is a method of continuously verifying codebase condition through automated testing, best achieved with version control integration.

- CD is an approach to regularly deploying artifacts that successfully pass the CI phase for confident deployment.

- CI, CD, and continuous deployment share the goal of faster, more robust software development and release, differing mainly in automation scope.

### CI and CD Phases and Pipelines

- CI involves code pushes to a Version Control System (VCS), build server checks, developer feedback, and code storage in a repository.

- CD ensures reliable, quick, and frequent software releases, aiding automated deployment.

- CI/CD pipelines visually represent the process, from code in a Git repository through various testing stages to final deployment.

### Characteristics of Good CI/CD

- Good CI features decoupled stages (each step performs a specific task), repeatability (consistent and repeatable automation), and fast failure detection.

- Good CD involves system-focused design (covering application, infrastructure, configuration, and data), pipelines that increase confidence towards production, and globally unique versions for tracking system state.

- Developers, QAs, and system administrators should all understand CI/CD.  Many tools exist for CI/CD, including Jenkins, GitLab, Bamboo, and others.

## Setting up Jenkins

### Jenkins Overview and Functionality

- Jenkins is a widely used open-source tool for continuous integration and building software development projects.

- It allows manual, periodic, or automatic builds, and uses plugins for deployment and automation.

- It supports various languages and team sizes.

- It is programmed using Java.

### Jenkins Plugins and CI/CD Process

- Jenkins uses plugins for source code management (Git), build tools (Maven), code quality analysis (Sonar), and testing frameworks (JUnit).

- A typical CI/CD process using Jenkins involves developers committing code changes, the CI server pulling the code and triggering a build, building the application for testing, and finally deploying to production.  Concerned teams are notified throughout the process.

### Jenkins Master-Slave Architecture

- Jenkins uses a master-slave architecture to handle multiple machines and distribute the workload for testing on various browsers and operating systems.

- The master schedules jobs and monitors slaves, while slaves execute the build jobs.

### Jenkins Installation Prerequisites and Process

- Prerequisites include JDK 1.7 or above, 2GB RAM (recommended), sufficient disk space, and a supported operating system (Windows, various Linux distributions, macOS).

- Installation involves downloading the LTS release, running the jenkins.war file using Java, and optionally changing the port.

- The Git plugin should be installed and Jenkins restarted.

## Jenkins Pipeline Process

### Jenkins Pipeline Overview

- Jenkins Pipeline (or "Pipeline") is a suite of plugins for implementing and integrating continuous delivery pipelines.

- It uses a domain-specific language (DSL) for pipeline creation.

- Pipeline-as-code involves writing the pipeline definition in a Jenkinsfile, stored in the project's source control repository.

### Benefits of Using Jenkinsfile

- Automates Pipeline build processes for all branches and pull requests.

- Enables code review and iteration on the Pipeline.

- Provides an audit trail.

- Creates a single source of truth for the Pipeline.

### Declarative vs. Scripted Pipeline Syntax

- Jenkinsfiles can use Declarative or Scripted syntax.

- Declarative Pipeline is newer and easier to write and read.

- Declarative Pipeline offers richer syntactical features.

- While syntax differs, commonalities exist between Declarative and Scripted Pipelines.

### Jargon in Jenkins Pipeline

- Pipeline: The code encompassing the complete build process.  A pipeline block is essential in Declarative syntax.

- Node: A machine in the Jenkins environment capable of running a Pipeline. A node block is crucial in Scripted syntax.

- Stage: A logically distinct set of tasks (e.g., Build, Test, Deploy).  Plugins use this information for status display.

- Step: An individual action or command (e.g., using the 'sh' step to execute a shell command).  Plugins often introduce new steps.

### Setting up a Basic Jenkins Pipeline

- Requires Jenkins 2.x or later and the Pipeline plugin.

- Create a new Pipeline project in the Jenkins Classic UI.

- Choose the Pipeline script option and enter the Pipeline code.

- The 'agent' directive allocates an executor and workspace.

- The 'echo' step writes to the console.

- Save and run the Pipeline using the 'Build Now' option.  View the results in the Build History and Console Output.

### Creating a Jenkinsfile

- A Jenkinsfile defines a Jenkins Pipeline and is saved in a source control repository.

- A basic three-stage continuous delivery pipeline (Build, Test, Deploy) is a common starting point.

### Example Jenkinsfile and Pipeline Stages

- The example Jenkinsfile uses Declarative Pipeline syntax.

- The 'agent' directive assigns an executor and workspace.

- The 'stages' directive defines the pipeline stages.

- The 'steps' directive specifies the actions within each stage.

- The 'when' expression in the Deploy stage ensures it only runs after successful Build and Test stages.

## Introduction to Version Control Systems (VCS)

### Understanding VCS

- Version control (or source control) monitors and handles software code modifications.

- VCSs are software applications that oversee code alterations over time.

### Features of VCS

- Back-up methodology.

- Recording increments to track live versions.

- Maintaining change history.

- Allowing multiple developers (remotely) to work on the same codebase.

- Merging changes across files.

- Tracking who made changes.

- Point-in-time marking (tagging).

- Branching for parallel development and release version maintenance.

### Centralized vs. Distributed VCS

- Centralized VCSs have a single central repository.

- Distributed VCSs allow each developer to have a full copy of the repository.

### VCS Jargon

- Repository (repo): Database storing files.

- Server: Computer storing the repository.

- Client: Computer connecting to the repository.

- Working copy: Local directory of files.

- Trunk/Main: Master code location.

- Head: Latest revision.

### Actions Performed in VCS

- Add: Place a file under version control.

- Check in: Send local changes to the repo.

- Check out: Download from repo to working copy.

- Ignore: Exclude files from version control.

- Revert: Restore a previous revision.

- Update/Sync: Update working copy to the latest revision.

- Diff/Change: Specific modification.

- Branch: Duplicate copy for feature development.

- Merge: Integrate changes from branches.

- Conflict: Inability to reconcile changes.

- Resolve: Manually fix conflicted changes.

- Locking: Prevent other developers from making changes.

### Example VCSs

- Concurrent Versions System (CVS)

- Subversion (SVN)

- Git

- Bazaar

- Mercurial

- Monotone

- Visual Source Safe (VSS)

## Git

### Git Overview

- Git is a distributed revision control system developed by Linus Torvalds.

- It supports non-linear development.

- It's compatible with macOS, Linux, Windows, and various protocols (HTTP, FTP, SSH).

- It efficiently handles projects of all sizes.

### Git Project Sections

- Working directory: Local files.

- Staging area: Files prepared for commit.

- Git directory (repository): Stores project history.

### Installing Git

- On Linux (Fedora/CentOS):  sudo dnf install git-all 

- On Linux (Debian/Ubuntu):  sudo apt install git-all 

- On macOS: Install Xcode Command Line Tools or use a binary installer.

- On Windows: Download from the Git for Windows website or use Chocolatey.

### Initializing a Git Repository

-  git init  creates a new Git repository.

-  git add  stages files for tracking.

-  git commit  saves changes with a message.

### Viewing Commit History

-  git log  displays commit history.

### Creating and Merging Branches

-  git branch  creates a new branch.

-  git checkout  switches branches.

-  git merge  merges branches.

# Mobile Test Automation: A Comprehensive Guide

## Introduction to Mobile Applications and Architectures

### What are Mobile Applications?

- Mobile applications, also known as mobile apps, are software applications designed for smartphones and tablets.

- They enhance user experience and provide convenient solutions for various needs, facilitating communication and information access.

- They have become integral to daily life in the digital age.

### Examples of Mobile Applications

- Utility apps: Serve practical purposes (weather forecasts, note-taking, financial management).

- Social networking apps: Facilitate social interaction and news updates (Facebook, Instagram, Twitter).

- Entertainment apps: Provide access to multimedia content (streaming platforms, gaming apps).

- E-commerce apps: Enable online shopping and order tracking.

- Productivity apps: Help manage time, tasks, and projects (document editing, project management).

- Health and fitness apps: Support fitness tracking, nutrition planning, and meditation.

- Travel and navigation apps: Provide maps, directions, and transportation information.

### Mobile Application Architectures

- Mobile architecture defines rules and techniques for mobile application development.

- A proper architecture simplifies implementation, testing, and maintenance.

- Considerations include device types, application types, mobile platform, CPU load, and screen time.

- A good architecture adheres to software development principles, with independent layers for easy scaling and troubleshooting.  This often involves a three-layer architecture.

- The three-layer architecture includes a Presentation Layer (UI and UX), a Business Layer (logic and data exchange), and a Data Layer (data safety and maintenance).

## Types of Mobile Applications

### Introduction to Mobile Application Types

- Mobile applications are categorized into three main types: native, browser-based, and hybrid.

- This section details the characteristics and differences between these categories.

### Native Applications

- Native apps are developed for specific mobile platforms (Android, iOS, Windows).

- Android apps are typically written in Java, while iOS apps use Swift or AppCode.

- They are tied to their respective operating systems and cannot run on others.

- They function in both online and offline modes.

- Android architecture emphasizes independent layers, while iOS often uses the Model-View-Controller (MVC) architecture.

### Browser-based Applications

- These apps are accessed through mobile browsers (Safari, Chrome).

- They are implemented using technologies like HTML, CSS, and JavaScript.

- They require a network connection and are not stored offline.

- Responsive web design enhances user experience.

- They are easier to implement and maintain across platforms compared to native apps.

- However, they may lack access to native device features like GPS and cameras.

### Hybrid Applications

- Hybrid apps are developed using web technologies (HTML, CSS, JavaScript) but run within a native container.

- They offer a native app feel.

- Abstraction layers enable access to device-specific capabilities (GPS, camera).

- They allow for a single code base across multiple mobile operating systems.

- They are particularly useful when an existing web page can be easily wrapped into a hybrid app.

## Test Strategy for Mobile Applications

### Defining a Test Strategy

- Ideally, every line of code should be tested, but this is unrealistic due to low efficiency and high costs.

- An optimal testing strategy balances efficiency, reliability, and precision.

- A test environment similar to the real device improves testing performance.

- High-fidelity tests run on emulated or physical devices, while low-fidelity tests might run on a local workstation's JVM.

- Flaky tests are those that do not pass 100% of the time, even with correct design and implementation.

### Testable Architecture

- A proper testable architecture allows testing different application parts in isolation.

- This improves code readability, maintainability, reusability, and scalability.

- Untestable architectures lead to larger, slower, and more flaky tests.

- Larger tests make it difficult to test all scenarios and states of an application.

### The Decoupling Approach

- Decoupling involves extracting parts of functions, classes, or modules for easier testing.

- Common techniques include splitting the app into layers (presentation, domain, data) or modules.

- It's important to make dependencies easy to replace and avoid direct framework dependencies in business logic classes.

- Further details can be found in the provided Android developer documentation link.

## Mobile Application Testing Fundamentals

### Types of Tests in Android

- Android tests are classified by subject (functional, performance, accessibility, compatibility) and scope (unit, end-to-end, medium).

- They can also be classified as instrumented tests (executed on a physical device or emulator) or local tests (executed on the development machine or server).

### Types of Tests for iOS Applications

- iOS application testing is classified into different types.  Examples include:

	- Manual testing using the device (system, UI, security, field testing).

	- Manual testing using the emulator (unit, integration, UI testing).

	- iOS Automation Testing (regression, built verification, compatibility, performance testing).

## Mobile Testing Tools and Frameworks

### Mobile Testing Frameworks - Examples

- Several frameworks and tools are used for mobile application testing.  Examples include:

	- Appium

	- SmartBear TestComplete

	- Katalon

	- Ranorex

### Appium

- Appium is an open-source test automation project used across multiple platforms (iOS, Android, Tizen).

- It uses a single, unified API for UI automation code.

- It supports multiple programming languages (Java, JavaScript, PHP, Ruby, Python, C#).

- It allows reusing source code for Android and iOS, saving time and effort.

### SmartBear TestComplete

- TestComplete handles various test automation requirements for mobile applications.

- It offers scriptless record and replay and keyword-driven testing.

- It includes advanced features like object recognition, automated reporting, and data-driven testing.

### Katalon

- Katalon is a comprehensive quality management platform with easy and efficient testing capabilities.

- It supports native, mobile web, and hybrid apps on Android and iOS.

- It works on real devices and emulators, offering features like record and playback, cloud-based integration, and cross-environmental execution.

### Ranorex

- Ranorex Studio automates mobile and mobile web app testing on real devices and emulators.

- It supports Android and iOS.

- It offers features like record and playback, CI environment integration, device-specific parameter checks, and simulation of user interactions.

## Appium Architecture

### Appium Architecture - Introduction

- Appium is a web server written in Node.js.

- It uses a client-server architecture. The server receives connections from the client, executes commands, and returns status.

- Communication happens via JSON objects over HTTP.

- A session ID is created and maintained until the Appium server is running.

### Appium Architecture Diagram

- A diagram shows the interaction between the WebDriver script, Appium server, UIAutomator (Android) or XCUITest (iOS), and the device or emulator.

## Advantages of Using Appium

### Appium is open-source with an active community.

### It supports multiple programming languages.

### It doesn't require recompiling the app, allowing testing of the same version submitted to app stores.

### It allows cross-platform testing.

### It uses native frameworks (UIAutomator for Android, XCUITest for iOS) for communication with devices.

## Native Type Mobile Application Testing with Appium

### Appium in Android

- Appium proxies commands to a UIAutomator script on the Android device.

- UIAutomator is a native UI automation framework allowing direct execution of JUnit test cases.

- bootstrap.jar acts as a TCP server, sending commands to the device via UIAutomator.

### Appium in iOS

- Appium uses Apple's UIAutomation API to interact with UI elements.

- UIAutomation is a JavaScript library.

- Executed test scripts are sent to the Appium server as JSON via HTTP.

- The server sends commands to instruments, which execute commands within the bootstrap.js file in the iOS instruments environment.

### Prerequisites to Use Appium

- Install Java (JDK), Android Studio, Android SDK tools, Appium jar file, Appium Desktop Client, and Eclipse IDE for Java.

- Refer to the provided links for detailed installation instructions.

- Appium Doctor can verify Appium installation.

### Writing an Appium Test

- The official Appium documentation provides step-by-step guidance for writing tests in JavaScript, Python, Java, or Ruby.

- The documentation also details Appium drivers, plugins, server security, and session parameters (capabilities).  Further information can be found in the "Guides" section of the documentation.

## References

### A list of references is provided, including books and online resources related to mobile test automation with Appium and testing Android and iOS applications.

# Software Quality Assurance: Test Reporting

## Test Reporting Process

### Understanding Test Reports

- A test report summarizes all test activities and final results of a testing project.

- It evaluates the success of testing.

- Stakeholders use it to assess product quality and decide on software release.  They may postpone release if many defects remain.

- Test summary reports are ideally prepared after the testing cycle is complete, allowing sufficient time before product shipment.

- Daily status reports provide daily updates, while test summary reports offer a consolidated overview of the entire testing cycle.

### Content of a Test Summary Report

- Concise and relevant information is crucial.

- Report templates vary depending on the project.  A typical report includes:

	- Test objective: The purpose of testing.

	- Areas covered: Functionalities tested.

	- Areas not covered: Untested areas.

	- Testing approach: Methods and processes used.

	- Defect report: Defects identified and described.

	- Platform details: Testing environments and platforms.

	- Overall summary: Feedback on the application's status.

### Steps to Create a Test Summary Report

- Step 1: Define the document's purpose with a short description.

- Step 2: Provide an overview of the application tested.

- Step 3: Detail the testing scope, including in-scope, out-of-scope, and untested areas due to constraints or dependencies.

- Step 4: Capture metrics such as planned, executed, passed, and failed test cases.

- Step 5: Document the types of testing performed to ensure proper application testing, including details of multiple testing rounds.

- Step 6: Describe the test environment (application URL, database version, etc.) and tools used, including bug management tools.

- Step 7: Document critical issues encountered and solutions implemented.

- Step 8: Include recommendations or suggestions for stakeholders.

- Step 9: Define exit criteria (successful test case execution, closed critical issues, action plans for open issues).

- Step 10: Indicate testing team approval for live system deployment and exit criteria fulfillment.  Sharing reports within the team is also important.

## Test Reporting Frameworks

### What are Test Frameworks?

- A test framework provides guidelines for coding standards, test data handling, object repository testing, etc.

- These are guidelines, not mandatory rules.

- They create a consistent interface between code and tests.

### Benefits of Using Test Frameworks

- Improved test efficiency.

- Lower maintenance costs.

- Minimal manual intervention.

- Maximum test coverage.

- Code reuse.

- Easier handling of recovery scenarios.

- Easy reporting.

### Common Types of Test Frameworks

- Linear Scripting Framework: Tests are independent, often created by recording and replaying manual actions.

- Module Based Framework: The application is tested in smaller parts (functions, modules, sub-systems). Tests can be combined for system-level testing.

- Library Based Framework: Reusable libraries are created for better maintenance and scalability.

- Behavior Driven Framework: Tests are written descriptively for business stakeholder understanding, focusing on behaviors and user scenarios.

- Data Driven Framework: Tests use different input data from databases or spreadsheets, separating test scripts and input data to avoid hard-coding.

- Keyword Driven Framework: An extension of data-driven, using keywords to define test steps, mapped to objects and actions in a shared repository.  Promotes reuse.

- Hybrid Testing Framework: Combines multiple frameworks to leverage their strengths and mitigate weaknesses.

## Software Tools for Test Reporting

### What are Test Reporting Tools?

- Software providing reporting, decision-making, and business intelligence capabilities.

- They extract and present data in charts, tables, and other visualizations.  Examples include Katalon, SpiraTest, Testim, Allure, and more.

### Why are Test Reporting Tools Required?

- Early bug detection: Tools identify critical bugs early, avoiding manual code review.

- Easier analysis:  Provides insights into project status and alignment with business requirements.

- Progress tracking: Helps monitor product development progress.

### Criteria for Choosing Test Reporting Tools

- User interface: Clean and easy to use.

- Usability: Easy to learn and master.

- Flexibility: Compatibility with various automation tools.

- Functionality and features: Comprehensive and relevant reports.

- Value: Reasonable price relative to features and use case.

### Key Features of Commonly Used Tools

- Test case management.

- Test execution management.

- Defect management.

- Traceability.

- Customizable reports.

- Dashboards for key quality metrics (release readiness, pass/fail trends).

- Real-time data tracking.

- Failure classification by root cause.

