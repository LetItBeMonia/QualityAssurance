# Description of the project:
This repository consists of knowledge that I've gained through self-education journey about Quality Assurance topic.

## Types of tests - test pyramid (from bottom up):
### 1. Unit Tests
Testing individual code modules (which should perform only one function). They can be run automatically using tools like Jest or Karma. The goal: to verify that all functions in the code work correctly.

### 2. Component Tests 
Testing individual elements (/components) of an application. For example, in a web application with a front-end, API, and database, the API is tested in isolation from the other components. This is important because, for instance, the database might fail or a request might be incorrect. The goal: to check whether the application behaves as expected without involving other components.

### 3. Integration Tests
Testing how different parts (/components) of the application work together. Here, connections such as API–database, frontend–API, etc., are tested (the opposite of component tests). Additionally, external APIs are often tested. These tests frequently reveal issues like typos in SQL queries, inconsistent variable naming conventions, incorrect database addresses, etc. The goal: to verify communication between all major components of the application. Types of integration tests:
- white-box testing
- black-box testing

### 4. End-to-End Tests 
Automated UI tests (a mix of functional tests [checking whether all features work, e.g., login, search, etc.] and acceptance tests [ensuring the application meets all business requirements]). Test scenarios are written in the "Gherkin" language (given–when–then), which is understandable for both developers and business stakeholders. Running these tests can take a long time, so they are often executed overnight, and not all parts of the application are always tested.
Software often used for end-to-end testing:
- Selenium, Cypress (for automated UI testing)
- SpecFlow, Cucumber (for writing Gherkin scenarios)
Often, only the essential parts of the application are tested, and tests are divided into groups, including a critical group that must be executed before every release. End-to-end tests require all application components to work together, so they are performed in environments such as QA (Quality Assurance) or UAT (User Acceptance Testing). This category also includes various types of tests, such as:
- performance testing
- regression testing
- security testing

### 5. Manual Tests 
Used for tests that are too complex to automate or not worth the effort. In practice, they may be carried out when there are too few (or no) testers in the team.

## MANUAL TESTING IN PRACTICE
## Test scenarios
### What is a test scenario and how to write it?
A test scenario is a short, one-line description of a software functionality that needs to be tested. It can be derived from software requirements documentation, user stories or any other documents that will help you to come up with test scenarios.

For example:
If I had to test login functionality in chrome browser, I would come up with the following scenarios:
- login with valid email & valid password in chrome browser
- login with valid email & invalid password in chrome browser
- login with invalid email & valid password in chrome browser
- login with invalid email & invalid password in chrome browser

## Test case

### What is a test case?
A test case is assigned to a scenario. It is a list of steps that need to be executed to complete a test scenario.

For example:
If I had to write a test case for "login with invalid email & valid password" scenario, I would come up with the following steps:
1. Launch a site in chrome browser: [http://www.example-site.com].
2. Click on a "Login" button in the top-right corner of the website.
3. Type invalid email in username field (username: email@gmaill.com).
4. Type valid password in password field (password: password111$).
5. Click on the login button below the password field.

## Reporting bugs

### What a bug report should consist of?
#### Summary
A bug summary should consist of information about: what happened, where it happened and under which circumstances.
#### Prerequisites
A list of requirements to be able to recreate a bug.
#### Steps to reproduce
A list of steps required to take to reproduce a bug.
#### Actual result
A result that you get upon reproducing all the steps mentioned above.
#### Expected result
A desired result upon reproducing all the steps mentioned above.

### What bug reporting software is out there?
The most common software for bug reporting is Jira.
