***Software Development Lifecycle (SDLC)***

    -Requirement
    -Design
    -Implementing
    -Testing
    -Deploying
    -Maintnence

Note that testing is a part of the SDLC


***Software Testing Lifecycle (STLC)***

    -Requirement Analysis
    -Test Planning
    -Test Development
    -Test Environment Setup
    -Test Execution
    -Test Closure


***Defect Lifecycle***
    -New 
    -Assigned
    -Opened
        ->Duplicate Rejected, Deffered, Not a bug
    -Fixed
    -Pending Retest
    -Retest
        ->ReOpened
    -Verified
    -Closed

***QA & QC***
    
    -QA:
        -Focus: Process
        -Nature: Preventive
        -Goal: Avoid defects
        -Methods: Audits
        -Timing: before production/testing

    -QC:
        -Focus: Product
        -Nature: Detective
        -Goal: Identify and fix changes
        -Methods: Inspections, testing
        -Timing: after production/testing


***Static And Dynamic Testing***

Static Testing:
    -Execution? No code execution
    -Performed on: documents, code, requirements
    -Goal: prevent defects
    -Type verification
    -Examples Techniques: reviews, walkthroughs, code analysis
    -When? Early in SDLC

Dynamic Testing:
    -Execution? Yes
    -Performed on: running software
    -Goal: Detect and fix defects
    -Type: Validation
    -Examples Techniques: Unit tests, UI tests, integration tests
    -When? Later in SDLC

***Verification && Validation***

    -Verification: Did we follow the process? Before testing
    -Validation: Does the product meet user needs? Happens after testing


***Different Levels of Software Testing***

-Unit Testing:
    -Focus: Individual functions/modules
    -Done by Developers
    -Example: testing a calculateTotal() function

-Integration Testing:
    -Focus: Module Interactions
    -Done by Developers/QA
    -Example: Checking API calls between components

-System Testing:
    -Focus: Entire system functionality
    -Done QA/Testers
    -Example: Testing a full web application flow

-Acceptance Testing:
    -Focus: business requirements
    -Done by End-users / Clients
    -Example: Final user testing before release


***White Box Testing***
Testing where you know the inner working of the code
    Types of testing that are generally white box testing:
        -Unit Testing
        -Integration Testing

***Black Box Testing***
Testing where you do not know how the inner workings of the code works

    Types of testing that are generally black box testing:
        -System Testing
        -User Acceptance Testing (UAT)


***Funcational & Non-Functional Testing Types***

FUNCTIONAL TESTING TYPES:
Unit Testing - Tests individual functions or methods in isolation

Integration Testing - Tests interactions between modules or services

System Testing - Tests the entire system as a whole

Smoke Testing - Basic tests to check if the build is stable enough for deeper tests

Sanity Testing - Verifies that functionality works after minor changes

Regression Testing - Ensures new changes haven't broken existing features

UAT - Confirms the system meets the bufiness needs and is ready for release


NON-FUNCTIONAL TESTING TYPES:
Performance Testing - Evaluates speed and responsiveness under load
    ->Load Testing, Checks how the system handles expected user traffic
    ->Stress Testing, 	Tests system behavior under extreme conditions.
    -> Soak/Endurance Testing, 	Tests system stability over a long period.

Security Testing - 	Finds vulnerabilities and checks data protection mechanisms.

Usability Testing - Evaluates how user-friendly the given software is

Compatibility Testing	Ensures the app works across browsers, OSs, and devices.

Reliability Testing	Tests the consistency and correctness over time.

Scalability Testing	Measures the software’s ability to grow (e.g., user base, data volume).

Maintainability Testing	Assesses how easy it is to maintain or update the system.

Portability Testing	Checks if the software can run in different environments.

Accessibility Testing	Verifies that users with disabilities can use the system.


***Re-testing and regression testing***


