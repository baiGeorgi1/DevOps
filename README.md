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
    -   [1.7.Summary](#17summary)

2.  [DevOps Overview](#2devops-overview)
    -   [2.1.What is DevOps?](#21what-is-devops)
    -   [2.2.DevOps Practices](#22devops-practices)
    -   [2.3.DevOps Trends](#23devops-trends)
    -   [2.4.Summary](#24summary)
3.  [Version Control with Git](#3version-control-with-git)
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

1. What is "software quality assurance" (SQA)?
    - Software quality assurance aims to
        - Minimize software defects
        - Ensure it behaves as expected
    - Defects are reported and tracked through a bug tracking system
    - Performed by the Quality Assurance engineers (QA engineers)
    - Continuous integration and delivery (CI/CD pipeline)
2. Quality Assurance (QA) Engeneers - QA engineers ensure the software quality
    - Plan and execute testing activities
        - Test the software, its functionality, UX, etc.
        - Create test plans, design test cases, execute tests
        - Develop and execute test automation scripts
    - Report and track bugs and their lifecycle
        - Perform regression testing when bugs are resolved
    - Track the development process and its quality
        - Review the requirements, design and code
        - Build and monitor CI/CD pipeline, track QA metrics
3. Bugs and Bug Tracking
    - Defects (bugs) in software are problems in the source code / requirements / design, which cause incorrect behavior
    - Once found (typically by the QA), bugs are tracked in a bug trackers / issue tracking software.
        - Examples: Jira, GitHub Issues
    - Bugs have a lifecycle
        - new → assigned / rejected → fixed → closed / reopened
4. Test Plan, Test Scenarios and Test Cases
    - ▪ Test plan
        - A guiding document outlining the testing approach, environments, schedule, and acceptance criteria to ensure software meets quality requirements.
    - Test Scenarios
        - High-level descriptions/stories representing the functionality or feature to be tested in the software.
    - Test Cases
        - Detailed, step-by-step instructions designed to validate specific conditions or functions of the software based on the associated test scenarios.
5. Manual and Automation Testing
    - Most of the QA work is software testing
        - Manual testing:
            - Fill forms
            - Click
            - Check the results
        - Automated testing:
            - QA automation
            - Test cases as code

#### 1.6.Deployment and Maintenance

1. What is software deployment? - Getting software out of the hands of the developers into the hands of the users. Compile, package, install, configure and run the software into the customer environment / ship the app to the customer.

    - Web app → deploy the new version to the Web servers
    - Mobile app → publish a new version to app stores
    - Desktop app → release a new version installer to the customers

2. Continuous deployment (CD) - Automatically deploy the software after each commit → ensure the changes are deployable.
3. Deployment Environments
   | Dev environment | Staging environment | Test environment | Production environment |
   |------------------|--------------------|------------------|------------------------|
   |Used by developers| Used by QA engineers and/or clients for UAT|Used by QA engineers|Used by clients|
   |No client data |Limited production data | No client data | Full Production data|
4. Container-Based Deployment Environments - Containers and clouds simplify creating, configuring and running the required environments
5. Software Maintenance
    - What is software maintenance?
        - The process of changing a system after it has been released
    - Reasons for maintenance changes
        - Fixing bugs and patching security vulnerabilities
        - Changing business needs: new features and requirements
        - Adapting to new environments: hardware / platforms / software
    - Typical change process
        - Analysis → requirements → issue backlog → prioritization
        - For each fix: design / re-engineering → code → QA → deploy
6. Software Documentation
    - Documentation makes software maintainable
        - Allow new people to join the development team over the time
    - Best practices in software documentation
        - Visualize the development process (use a project board)
        - Written requirements (in a requirements tracking system)
        - Design and architecture documents (e.g., project Wiki)
        - Code documentation (comments and built-in docs in the code)
        - Test management system and CI system (with a dashboard)
        - User documentation, installation guide, quick start guide, etc.

#### 1.7.Summary

1. **Software engineering** provides knowledge, processes, practices
   and tools for all the phases in software development lifecycle
   (SDLC)
2. **Software requirements** describe the functionalities of the software
3. **Software design and architecture** describe system structure –
   modules and interactions
4. **Software constructions** involves coding, debugging, unit testing,
   code reviews and integration (including CI)
5. The **QA engineering** process ensures the software works as
   intended, mostly through testing (manual and automated)
6. **Software deployment** ships the software to customers and goes
   through different deployment environments

[Back](#contents)

# **2.DevOps Overview**

#### 2.1.What is DevOps?

> DevOps is a set of practices, tools, and philosophy that combines development (Dev) and operations (Ops) into one, continuous process.

> Unites people, process, and technology in application planning, development, delivery, and operations.
> Enables coordination and collaboration between isolated roles like development, IT operations, quality engineering, and security.

1. DevOps Lifecycle - DevOps lifecycle (or pipeline) is a series of automated development processes or workflows within an iterative development lifecycle. Represents the processes, capabilities, and tools for development (left side) and operations (right side). Merging both sides into one seamless process.
   Follows a continuous approach.

<img src='https://miro.medium.com/v2/resize:fit:2000/format:webp/1*57INuyf56018l0Y_Pel0ig.png' width=600px height=250px >

2. DevOps Lifecycle Stages:

    - **_Plan_** - Identify business requirements and collect end-user feedback.
    - **_Code_** - Code development.
    - **_Build_** - Finished code is committed to a shared repository.
    - **_Test_** - Build is deployed to a test environment and tests are performed.
    - **_Release_** - Operations team schedules the releases or deploys multiple releases to production.
    - **_Deploy_** - The production environment is built and the build is released.
    - **_Operate_** - Release is live now. Operations team takes care of server configuring and provisioning.
    - **_Monitor_** - evOps pipeline is monitored to find problems / bottlenecks.

3. DevOps Pipeline Phases:

    - Continuous **_Development_** - Plan and Code.
    - Continuous **_Integration_** - Update code and add new features.
    - Continuous **_Testing_** - Run automated or manual tests.
    - Continuous **_Deployment_** - Code is automatically deployed on production servers.
    - Continuous **_Feedback_** - Evaluate user experience to improve future releases.
    - Continuous **_Monitoring_** - Monitor for system errors or performance issues.
    - Continuous **_Operations_** - Automate launching the app and its updates.

4. DevOps Tools - click the image!

    [<img src='https://www.devopsschool.com/blog/wp-content/uploads/2024/01/image-302-1536x864.png' height=200px>](https://www.devopsschool.com/blog/wp-content/uploads/2024/01/image-302-1536x864.png)

5. DevOps Culture - this is a collaborative approach to software development and delivery that emphasizes communication, automation, and improvement.

    > Collaboration is crucial - All teams should communicate honestly and openly about DevOps
    > processes, priorities, and concerns together.
    >
    > As teams align, they take ownership and become involved in other lifecycle phases, not just the ones central to their roles.
    >
    > DevOps teams remain agile by releasing software in short cycles.
    >
    > Teams strive to learn and continuously improve.

6. DevOps Engeneers - they are responsible for the deployment, and maintenance of software applications.
   Collaborate with development and operations teams. Balance a blend of soft skills with their tech knowledge. They understand development lifecycles, DevOps culture, practices and tools.
    > The Role of DevOps Engineers - Their job and responsibilities include:
    >
    > - Automating processes.
    > - Managing and maintaining the infrastructure system.
    > - Monitoring performance.
    > - Ensuring the security of the software.
    > - Scale systems and ensure the availability of the services with developers.

#### 2.2.DevOps Practices

> Many practices, varying on the specific context and organization. Some practices are:
>
> -   [<img src='https://miro.medium.com/v2/resize:fit:1400/0*NXlBkHolIQvfO_Rr' width=550px height=150px align='right'>](https://miro.medium.com/v2/resize:fit:1400/0*NXlBkHolIQvfO_Rr)
> -   CI/CD
> -   Infrastructure as code (IaC)
> -   Version control
> -   Monitoring and logging
> -   Automation
> -   Agile software development

1. **CI/CD Pipeline** - Cornerstone of DevOps describing the code journey from a developer's machine to production.
    - Consists of multiple stages:
        - Development;
        - Integration;
        - Testing;
        - Deployment.
    - End goal:
        - Deliver features, updates and fixes to users quickly and reliably.
    - CI/CD allows organizations to ship software quickly and efficiently:
        - **Continuous integration**
            - Developers regularly merge code changes into a central repository, which are validated by automated tests.
        - **Continuous delivery**
            - Code changes are automatically prepared for a release to production (and can be manually deployed).
        - **Continuous deployment**
            - Changes that pass all stages of production pipeline are released automatically (optional).
    - Tools: **GitHub Actions, Jenkins, CircleCI, etc**.
2. **Infrastructure as Code (IaC)** - Managing and provisioning of infrastructure through code instead of through manual processes. Used to automatically manage infrastructure resources:
    - Servers
    - Operating systems
    - Software platforms
    - Storage
    - Networking
    - Etc.

-   IaC Tools - define infrastructure resources using code / config files. Can be version controlled, tested, and deployed automatically.
    > Tools:Ansible, Puppet, Chef, Saltstack, Terraform, etc.

Approaches to IaC:

-   Declarative - Defines the desired state of the system, i.e. resources you need and their properties.
-   Imperative - Defines the specific commands for the desired configuration.

3. **Version Control**

-   The practice of managing code in versions to make code easy to review and recover.
-   Includes tracking revisions and change history.
    -   Saves each individual changes in a special database.
-   Necessary for CI/CD and IaC. - Helps enhance efficiency. - Allows preserving agility when a team grows larger.

    > Tools: Git, SVN, Mercurial, etc.

-   Essential for software development
    -   Serves as a safety net to protect code
    -   Allows several people to work on a project simultaneously
        -   Improves collaboration and enhances development speed
-   Manages changes in:
    -   Code
    -   Configurations
    -   Infrastructure definitions
    -   Documentation

4. **Monitoring and logging**

-   Monitoring means having full, real-time visibility into the health and performance of the entire application stack. - App metrics, event data, logs, traces, etc. are collected and analyzed. - Actionable and meaningful alerts are set for failures in the entire deployment pipeline. - Thus, DevOps team can mitigate issues in real time.

    > Tools: ELK Stack, Splunk, Prometheus, Grafana, Alertmanager,Nagios, etc.

5. **Automation**

-   DevOps teams aim to automate as much of the software lifecycle as possible to have more time for writing code and developing features. - With automation the simple act of pushing code changes to a source code repository can trigger a build, test, and deployment process. - Pros: software delivery is faster, processes are consistent, predictable and scalable, teams don't perform tedious manual tasks.
    > Tools are different for each step of the DevOps process.

6. **Agile software development**

[<img src='https://agilefirst.io/content/images/2022/06/agile-devops.png' width=400px height=150px align='right'>](https://agilefirst.io/content/images/2022/06/agile-devops.png)

-   Agile == modern software development approach.
-   It emphasizes on:
    -   High adaptability to change through short release cycles;
    -   Customer and user feedback;
    -   Team collaboration.
-   In DevOps, Agile practices include increased automation, improved collaboration, etc.

#### 2.3.DevOps Trends

1. **DevOps movement trends include:**

-   Increased focus on security and compliance;
-   Adoption of microservices architecture;
-   Evolution of automation and AI;
-   And many more…

    They improve overall job productivity.

2. **DevSecOps** = development + security + operations

-   Includes DevOps framework with security as a shared responsibility
-   Its mindset is to integrate security practices into applications and infrastructure from the start.
-   Identifying security vulnerabilities via analysis.
-   Tools:
    -   Static analysis - SonarCube, Fortify , Veracode, Chekmarx.
    -   Dynamic analysis - OWASP Zed Attack Proxy, Burp Suite, Acunetix, WebInspect.

3. **DevOps** vs **DevSecOps**
   | |DevOps | DevSecOps |
   |--|--|--|
   | **Focus** | Increasing quality and speed of software development and delivery |Secure software development processes by integrating security|
   | **Process** | CI/CD | CI/CD + additional security-related processes|
   | **Activities**|Continuous testing, development and monitoring QA tasks|Pre-commit, commit-time, build-time, test-time, deploy time checks of code|
4. **Static** vs **Dynamic Analysis** in DevSecOps:
   |**Static Analysis**|**Dynamic Ananlysis**|
   |-------------------|---------------------|
   |Used for identifying security vulnerabilities|Used for identifying security weaknesses|
   |Analysis of the code without executing it|Analysis of the code by executing the app in real or simulated environment|
   |Catch potential security issues early in the development stage|Detect security issuesat runtime|
5. **Serverless Computing** - refers to outsourcing back-end cloud infrastructure and operations tasks to a cloud provider.

-   Developers focus on writing code.
-   Cloud provider manages the infrastructure, ensuring agility and scalability.
-   Serverless computing == Function-as-a-Service (Faas)
-   Based on event-driven execution - Allows functions to be triggered in response to specific events (changes in data or user requests, etc.)
-   Stateless nature - Serverless functions are designed to be stateless.
-   Wide range of tools - Frameworks, SDKs, CLIs.

6. **Microservices Architecture**
    > Microservices == architectural approach to development that breaks the application into different loosely coupled services.

-   Each service focuses on a specific business capability - Can be independently developed, deployed and scaled.
-   As everything is broken down into separate services, development teams can also be divided to tackle each service - Makes the development process more flexible.
-   Communication between services is typically achieved through lightweight protocols, e.g., HTTP/REST.
-   Each microservice can have its own technology stack, programming language and database - These depend on the specific business requirements.

<img src='https://ncube-digest.com/wp-content/uploads/2020/04/monolithic-vs-microservice.jpg' width=750px height= 250px>

7. **AIOps and MLOps**

-   AIOps (Artificial Intelligence for IT Operations) refers to the use of artificial intelligence (AI) and machine learning (ML) technologies to automate and enhance various IT operations and processes.
-   AIOps helps with identifying the main cause of the problems that hamper operational productivity.
-   MLOps helps with optimizing operations and enhancing productivity.

#### 2.4.Summary

-   **DevOps** == a set of practices, tools and a cultural philosophy that automate and integrate the processes between software development and IT operations teams.
-   8 DevOps lifecycle stages and 7 pipeline phases
-   DevOps practices include CI/CD, Infrastructure as Code, Version Control, Monitoring and Logging, Automation, Agile Software Development, etc.
-   DevOps trends include DevSecOps, Microservices, Serverless Computing and AIOps.

[Back](#contents)

# **3.Version Control with Git**

# **Automated Testing**

# **Continuous Integration and Continuous Delivery (CI/CD) with GitHub Actions**

# **Continuous Integration and Continuous Delivery (CI/CD) with Jenkins**

# **Development Workflow**
