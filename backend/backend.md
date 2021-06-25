# Backend

## Tools

### Plan

#### Task management

- Jira
  - [TBD]Sample ticket template
  - Status management flow

#### Spec

- Confluence
  - [TBD] Sample directory structure for concerning easier visibility

#### Documentation

- Readme
  - [TBD] Sample skeleton with examples
  - [TBD] Create a changelog from commit :question_mark:

#### Communication

- Slack

#### Diagrams

- Draw.io
- Miro
- PlantUML(C4)
  - [plantuml-stdlib/C4-PlantUML](https://github.com/plantuml-stdlib/C4-PlantUML)

#### OpenAPI

- Use Github Pages for hosting swagger

#### Database

- MySQLWorkbench
- Other SQLs Schema Management => ?
- NOSQL Schema Management => ?
- [TBD] DataBase Design best practice

#### File management

- Google Drive
  - [TBD] Directory Structure

#### Presales

- Google Slide
- [TBD] Requirement gathering

#### Estimation

- https://github.com/monstar-lab-group/readme/blob/master/core/estimations.md
- Dev estimation
  - [TBD] Sample Google Sheets Template
- Infra Cost
- [TBD] Sample Google Sheets Template
- [Amazon Web Services Simple Monthly Calculator](https://calculator.s3.amazonaws.com/index.html)

#### Git Branching rules

Best practice => ?

### Code

#### General

- Local development environment
  - Use docker
  - [TBD] Sample docker files
- API testing
  - Utilise postman collections
  - Use SwaggerUI
- Git
- Github/ Gitlab/ Bitbucket
  - Issue/ PR templates
  - Use cases of Labels, Asignee etc
    - Use Template Repository (may be can be done from organization)
    - https://github.com/organizations/monstar-lab/settings/repository-defaults
  - Branch naming/ PR title conventions
    - Include Jira ticket numbers etc
  - Branch restriction policy
  - Reviewing policy
  - History/ simple explanation of choosing the architecture
    - why the architecture/ pattern was chosen (so that others can relate the )
      - e.g. Markdown Architectural Decision Records
  - Commit message convention
  - Create changelog automatically from commit message (align with the app team as well)
- Coding Style
  - name should be UTF8, no trailing spaces etc
  - Lint
  - Check style with CI/CD tool
- Documentation
  - Readme on Github
    - [TBD] Create a template
- Template
  - Use common auth services etc rather creating from scratch
    - Create usage templates
    - Services
      - Keycloak
      - Cognito
      - Firebase Auth

#### Will be arranged separately by the specialist member

- Coding convention
- Frameworks
  - For REST API
- Common libraries for specific purposes (?)
- Unit test
  - Test suite
  - Best practice
    - Mocking etc
- Create template

  - How to collaborate with global team
    - #tech-monstack

- Ruby
  - https://github.com/shogo-mitomo/project-template-api-rails
- PHP
  - https://github.com/monstar-lab-group/php
- JS
  - https://github.com/monstar-lab-group/nodejs-backend
- Go
- Java
  - Java 11,15 or later
  - Spring Boot
  - Gradle
  - Flyway
  - Libraries
    - Lombok
  - Test
    - JUnit
    - [Error Prone](http://errorprone.info/)
    - [Find Security Bugs](https://find-sec-bugs.github.io/)
    - [checkstyle – Checkstyle 8.43](https://checkstyle.sourceforge.io/)
  - IntelliJ Idea
- Python
  - Usage: for machine learning etc => will be organized by the AI team
  - Frameworks
    - Flusk
    - [TBD] Responder (?)

### Build, Release/ Deploy

- Docker

  - [TBD] Prepare necessary docker files
    - Image size => should be as much small as possible
      - Build, deploy and container start gets faster
  - Services
    - DockerHub
    - Github Container Registry
      - Permissions are easy to manage
      - Is there any other drawback?

- Github Actions
  - [Pricing · Plans for every developer](https://github.com/pricing)
    - https://docs.github.com/en/github/setting-up-and-managing-billing-and-payments-on-github/about-billing-for-github-actions
  - [TBD] Create usage template/ actions
    - Can actions be private? => need to confirm
      - https://docs.github.com/en/actions/learn-github-actions/sharing-workflows-with-your-organization
    - Is it okay to keep it as public? => may be, should keep the secrets/ important parameters as Env Var over Github
  - Will vary on language/ stack

### Test (language independent)

- Add at least one sample test for each layer (controller, service, repository etc) in the project so that the same pattern can be followed later on
- Maintain coverage information in each project
- https://github.com/monstar-lab-group/readme/blob/db7c04e1963f5f10e548bd477ca97ef5c03ac9d8/tech/code-modes.md
- What to when there is lack of time?
  - Write test for important features? How to decide on that?
    - Consider impact, dependencies etc
- Use security testing
  - Github
  - Gitlab
    - [Dynamic Application Security Testing (DAST) | GitLab](https://docs.gitlab.com/ee/user/application_security/dast/)
- Use SonarCube?
  - [TBD]

### Operate / Monitor

- Log
  - Format
    - List down what kind of data cannot be logged (passwords, private data etc)
  - Error level
    - Define use case for each environment
  - Tool
    - Cloudwatch
    - ELK
    - Sentry
    - Datadog
- APM usage
  - Tool
    - ELK
    - NewRelic
- Health check API
  - Use common pattern
    - access db check
    - common api req and response format

### Security

- Container security
  - Refer to [Dynamic Application Security Testing (DAST) | GitLab](https://docs.gitlab.com/ee/user/application_security/dast/)
- Don’t hardcode key
- Make sure of SQL Injection, XSS, CSRF etc related handling with relation to the frameworks used
- Virus scan, WAF => infra
- How about internal Bug Bounty program
- Access Control (ACL) is a hard topic.
  - We must create awareness and consider workshop / discussion meetings.
- Tools may not be able to discover design / business log flaws.
  - We must decide a way to fix this.
  - Possible checklist?
  - Biggest weakness is the webapp side modifying the request parameters.
  - [TBD] Consult to ML Security engineer
