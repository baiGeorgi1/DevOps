# DevOps

Software Engineering and DevOps - May - 2024 - SoftUni

## Contents

1.  [Software Engineering Fundamentals](#1software-engineering-fundamentals)

    -   [1.1.Software Development Lifecycle](#11software-development-lifecycle)
    -   [1.2.Software Requirements](#12software-requirements)
    -   [1.3.Software Architecture and Design](#13software-architecture-and-design)
    -   [1.4.Software Construction](#14software-construction)
    -   [1.5.Software Quality Assurance](#15software-quality-assurance)
    -   [1.6.Deployment and Maintenance](#16deployment-and-maintenance)

2.  [DevOps Overview](#devops-overview)
3.  [Version Control with Git](#version-control-with-git)
4.
5.  [Automated Testing](#automated-testing)
6.
7.  [Continuous Integration and Continuous Delivery (CI/CD) with GitHub Actions](#continuous-integration-and-continuous-delivery-cicd-with-github-actions)
8.  [Continuous Integration and Continuous Delivery (CI/CD) with Jenkins](#continuous-integration-and-continuous-delivery-cicd-with-jenkins)
9.  [Development Workflow](#development-workflow)

---

# **1.Software Engineering Fundamentals**

#### 1.1.Software Development Lifecycle

> Requirements → Design → Code → Test → Deploy

-   Inexperienced developers consider "coding == development"
-   Software engineering is not just coding!
    -   In most projects coding is only 20%-30% of the project activities!
    -   The software development process involves many more
    -   The important decisions about the software are taken during the requirements analysis and software design phases
    -   QA, testing, integration, reviews, deployment, documentation, and
        management are often disparaged
-   Software engineering is about building software professionally, through a manageable and predictable process
-   Software engineering is an engineering discipline aimed to provide knowledge,processes, practices, and tools for
    -   Defining software requirements
    -   Creating software design
    -   Software construction
    -   Software testing and QA
    -   Software deployment
    -   Software maintenance tasks
    -   Managing the development process
-   The Software Development Lifecycle (SDLC) :
    -   Analyzing and defining software requirements
    -   Creating software architecture and design
    -   Software construction
    -   Software testing and QA
    -   Software deployment
    -   Software maintenance
-   Methodologies manage the development process
    <img src='https://static.javatpoint.com/tutorial/software-engineering/images/software-engineering-software-development-life-cycle.png' width=350px height= 250px alt='SDLC'>

#### 1.2.Software Requirements

1.  Software requirements describe the functionality of the software:

    -   Answer the question "what shall it do?", not "how shall it do it?"
    -   Define constraints on the system

    > Two kinds of requirements:

    -   Functional requirements
        -   Product functions, enabling users to achieve their tasks
    -   Non-functional requirements
        -   Reliability, efficiency, usability, maintainability, etc.

2.  Requirements analysis starts from an idea about the system

    -   Customers often have a broad idea but may lack specifics
    -   Requirements come roughly → adjusted during the development
    -   Requirements change constantly!

    > Analysis produces some requirements documentation

    -   User stories / UI prototype / Software Requirements Specification (SRS) / informal system description:
    -   UI prototype:

        <img src='https://cdn.logojoy.com/wp-content/uploads/20220823141753/mobile-wireframe-sketch-example-e1661278727822-600x382.png' height=150px>

    -   SRS example:

        <img src='https://images.wondershare.com/mockitt/chatgpt/preparing-to-wirte-srs-document.jpg' height=150px>

    -   User story example:

        -   A story starts from a simple idea (1-2 sentences)
        -   As the team discusses the story, they add more details

        <img src='https://assets.justinmind.com/wp-content/uploads/2020/09/user-story-examples-product-plan.png' height=150px>

    -   Should be clear, concise and unambiguous
    -   It is always hard to describe and document the requirements in a comprehensive way
        -   Good requirements save time and money, but are hard to reach
    -   **Requirements always change during the project!**
        -   Good requirements reduce the changes
        -   UI prototypes significantly reduce changes
        -   Agile methodologies are flexible to changes
        -   Use user story tracking tools to handle changing requirements

#### 1.3.Software Architecture and Design

> Software architecture and design

-   Technical descriptions (e.g., diagrams) about how the system implements the requirements

> The software (system) architecture describes the subsystems, their responsibilities and interactions

-   High-level infrastructure of a software system
-   Good software architecture == easier maintenance and scalability

> The software design describes the system design at a lower-level

-   Functions of individual modules, classes, etc.

> Design patterns in software design

-   Proven solutions to recurring problems

-   Fundamental in software engineering

1. System Architecture:
    - The system architecture is a conceptual model, describing
        - How the system will be decomposed into modules (subsystems)
        - Responsibilities of each module
        - Interaction between the modules
        - Platforms and technologies, communication protocols
    - Can be formal or informal (typically)
        - Consists mostly of diagrams / blueprints
2. System Architecture Diagram:

<img src='https://slideplayer.com/slide/15763979/88/images/19/System+Architecture+Diagram-Examples+%5B5%5D.jpg' width=600px height=200px >

3. Software Architecture Diagram:

<img src='https://images.edrawsoft.com/articles/software-architecture/architecture-5.png' width=600px height=200px >

4. Software Design
    - Detailed design
        - Describes the internal module structure
        - Subcomponents, interfaces, process design, data design
    - Object-oriented design
        - Describes the classes, their responsibilities, relationships, dependencies, and interactions (usually in UML)
    - Internal class design
        - Methods, responsibilities, algorithms and interactions
5. UML Class Diagram
    > UML == Unified Modeling Language. Visualize classes and their relationships.

<img src='https://miro.medium.com/v2/resize:fit:1200/1*szU8ngrWSXmBNPYReMyK5w.png' width=600px height=200px >

6. Flowchart Diagram - Visualizes a decision logic/calculation/algorithm

<img src='https://www.smartdraw.com/flowchart/img/color-flowchart-simple.jpg' width=600px height=200px >

7. Software Design Document (SDD) - Formal description of the architecture and design of the system.
    > Essential for software development process

-   Makes communication between collaborators easier
-   Often used for future references
-   Ensures the entire team has a clear understanding of the system's design - Beneficial when onboarding new team members

    > What's typically inside?

-   Architectural design
-   Modules and interactions (diagram)
-   For each module
-   Process design (diagrams)
-   Data design (E/R diagram)
-   Object-oriented design (class diagram)

#### 1.4.Software Construction

> During the construction phase developers build the software. Sometimes it is called "implementation phase".

1.  Software construction includes:
    -   Method design
    -   Writing the source code
    -   Testing and debugging
    -   Writing the unit tests
    -   Code reviews and inspections
    -   Integration of classes / modules
2.  Writing the code:
    -   Coding
        -   The process of writing the programming code (the source code), running and debugging it;
        -   The code adheres to established architecture and design;
        -   Developers perform method design as part of coding.
    -   The source code is the output of the software construction process
        -   Written by developers;
        -   Can include tests (unit, integration, others).
3.  Testing the code:
    -   Testing
        -   The process of checking whether the developed software conforms to the requirements;
        -   Aims to identify defects (bugs).
    -   System testing is done by the QA engineers
        -   Unit / integration testing is done by developers.
    -   Developers test the code after writing it
        -   Run it at least once to see the results;
        -   Unit testing / integration testing work better:
            -   Automated tests are repeatable, executed many times.
4.  Derbugging
    -   Debugging:
        -   Finding the source of an already identified bug and fixing it;
        -   Performed by developers (constantly).
    -   Steps in debugging:
        -   Find the defect in the code
        -   Identify the source of the problem
        -   Identify the exact place in the code causing it
        -   Fix the defect (modify the source code)
        -   Test to check if the fix is working correctly
        -   Write a unit test for the defect to avoid it reoccurring further
5.  Software Verification Activities
    -   Inspections:requirements / design / code inspections
        -   Aim to find flaws early, e.g., in the requirements
        -   Performed by an experienced dev / QA engineer
    -   Code reviews: developer reviews the code
        -   Find flaws / bugs / improve quality
    -   Static analysis: software tools scan the source code for problems
        -   Security, code quality, potential bugs, etc.
    -   Dynamic analysis: tools asses runtime code to find flaws
        -   Memory issues, bad performance, arithmetic overflows, etc.
6.  Code reviews
    -   Code reviews
        -   Assessments of the source code and other assets
        -   Developer A reviews the code written by Developer B
        -   Goals:
            -   Identify bugs
            -   Increase code quality
            -   Apply best practices
            -   Help developers learn the source code and from other developers
    -   Code reviews can be:
        -   Formal or informal
        -   Live or offline
    -   Code review tools are used to perform code reviews online
        -   Example: GitHub Pull Requests
        -   Code under review gets improvement suggestions and comments
        -   Code under review can finally be rejected or approved
7.  Software Integration
    -   Combining multiple software systems to work together seamlessly and efficiently
        -   Enabling data exchange between them
    -   Enhances overall productivity
        -   Reduces redundancy
        -   Improves efficiency
    -   Compile, run and deploy separate modules as a single system
    -   Test to identify defects (integration testing)
8.  Software Integration Strategies

    -   Big bang

        -   All or almost all modules are integrated together at the same time
            <img src='https://media.licdn.com/dms/image/C5112AQEuqNhVssnXpg/article-cover_image-shrink_600_2000/0/1546954191369?e=2147483647&v=beta&t=kypHLxR0eDI7cyNilaA1PSsGMRwsoKxbEidsPbvpusw' width=300px height=100px  >

    <img src='https://www.guru99.com/images/1/Hybrid-Integration.png' width=300px height=130px  align="right">

    -   Top-down

        -   Integration of the higher-level layers first

    -   Bottom-up
        -   Lower layers first
    -   Continuous integration (CI)
        -   Integrate after each commit in the source control system
        -   Integrating the code from different developers frequently (several times a day)
        -   Automated building and testing the software
        -   Typically, at Git push in a certain branch
        -   Finding integration problems and bugs early
        -   Continuously maintain software quality
        -   CI is implemented by a CI system like Jenkins, GitHub Actions, TeamCity, Azure Pipelines

9.  CI/CD Pipeline

    -   CI/CD pipeline
        -   Continuously integrate and release new features
    -   Continuous integration (CI)
        -   Write code, test and integrate it in the product
    -   Continuous delivery (CD)
        -   Continuously release new features
    -   Often QA engineers maintain and monitor the CI/CD pipeline

    <img src='https://blog.openreplay.com/images/what-is-a-ci-cd-pipeline/images/Yy1Tzwx.png' width=500px height=150px  >

#### 1.5.Software Quality Assurance

#### 1.6.Deployment and Maintenance

[Back](#contents)

# **DevOps Overview**

# **Version Control with Git**

# **Automated Testing**

# **Continuous Integration and Continuous Delivery (CI/CD) with GitHub Actions**

# **Continuous Integration and Continuous Delivery (CI/CD) with Jenkins**

# **Development Workflow**
