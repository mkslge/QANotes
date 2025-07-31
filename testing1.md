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


    New → Assigned → Open → Fixed → Retested → Verified → Closed
                            ↑       ↓
                      Rejected ← Reopen


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
    -Unit Testing - Tests individual functions or methods in isolation
    -Integration Testing - Tests interactions between modules or services
    -System Testing - Tests the entire system as a whole
    -Smoke Testing - Basic tests to check if the build is stable enough for deeper tests
    -Sanity Testing - Verifies that functionality works after minor changes
    -Regression Testing - Ensures new changes haven't broken existing features
    -UAT - Confirms the system meets the bufiness needs and is ready for release


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

Regression testing
    -Repeated testing of already built components to make sure that modification of a certain part of our code
    didn't cause any defects on any previous code.

    -Done in the following cases:
        -New functionalities are added to the app
        -Change Requirement
        -Defect Testing
        -Performance Issue FIx
        -Environment Change (Updating DB to MySQL to Oracle)


Retesting is usually only done after we find a bug, and is only done to that specific module/unit



***Exploratory Testing***
A hands on, unscripted software testing approach where testers actively explore an application to find bugs,
understand behavioral, and evaluate usability, without any predefined test cases.


***Adhoc Testing***

Adhoc Testing is an informal testing type with an aim to break the system
    -Usually unplanned
    -It does not follow any test design technique to create test cases, doesn't use test cases.
    -Testers randomly test the application without any test cases or any business requirement.



***Sanity && Smoke Testing***

Sanity Testing
    -Usually done after you fixed a bug to make sure that specific component/unit works

Smoke Testing
    -Run some basic tests to make sure the systems basic functionality works before running
    a more extensive fleet of test cases


***End-To-End Testing***
End-to-End Testing is the process of testing an application from start to finish, simulating real 
user workflows to ensure the entire system works as expected — including frontend, backend, databases,
external integrations, and APIs.

    -The goal of E2E testing is to verify that all parts of the application work together correctly.
    -The user can complete workflows without issues
    -Dependencies function properly in the work flow:

Example:
1. User logs in
2. Searches for an item
3. Adds the item to cart
4. Proceeds to checkout
5. Enters shipping & payment details
6. Places the order
7. Gets confirmation email



**Test Design Techniques**



***Equivalence Partitioning***

Divide input data into partitions where all values are expected to behave similarly. 
Test one value from each.

Example: Input age field: partitions can be <18, 18–60, >60


***Boundary Value Analysis***

Focus on values at the edges of boundaries of partitions, where errors are most
likely to occur

For ages 18-65, focus on 17, 18, 19 and 64, 65, and 66

***Decision Table Testing***

Create a table of conditions and actions to cover all possible combinations

For login: conditions like "correct username" + "correct password" = success

***State Transition Testing***

Tests based on system states and transitions in between them

ATM Idle -> Card Inserted -> Pin Entered -> Authenticated

***Use case testing***

Based on real user workflows

Buying an item on Amazon: search → add to cart → checkout




***Statement Coverage***

Ensure every line of code is executed at least once

So if you have a codeblock with 10 statements, 10 test cases would suffice

***Branch/Decision Coverage***

Test each decision (e.g., if/else) to be true and false at least once.

***Condition Coverage***

Test each Boolean sub-expression independently.

independently.	In if (A && B), test A=true/false and B=true/false


***Path coverage***
Test all possible paths through code


***Loop Testing***
Check for zero, one, and multiple iterations.	

Test for loops for boundary issues



**Use Case, Test Scenario, and Test case**

Use case:
    -Describes the requirement
    -Contains 3 items:
        -Actor
        -Action/Flow
        -Outcome

Test scenario:
    -Possible are to be tested (What to test)

Test Case:
    -How to test
    -Describe test steps, expected result & actual result
