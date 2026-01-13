# Description of the project:
This repository consists of knowledge that I've gained through self-education journey about Quality Assurance topic.

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
1. Launch a site in chrome browser: [http://www.site.com].
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
