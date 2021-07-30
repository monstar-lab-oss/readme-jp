# Coding Guidelines

## General

### Local development environment

- Use docker
- [TBD] Sample docker files

### API testing

- Utilise postman collections
- Use SwaggerUI

### Git

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

### Coding Style

- name should be UTF8, no trailing spaces etc
- Lint
- Check style with CI/CD tool

### Documentation

- Readme on Github
  - [TBD] Create a template

## Templates

- Use common auth services etc rather creating from scratch
  - Create usage templates
  - Services
    - Keycloak
    - Cognito
    - Firebase Auth

Will be arranged separately by the specialist member

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

### Ruby

- https://github.com/shogo-mitomo/project-template-api-rails

### PHP

- https://github.com/monstar-lab-group/php

### JS

- https://github.com/monstar-lab-group/nodejs-backend

### Go

- TBD

### Java

- TBD
  - Java 11,17 or later
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

### Python

- TBD
  - Usage: for machine learning etc => will be organized by the AI team
  - Frameworks
    - Flusk
    - [TBD] Responder (?)
