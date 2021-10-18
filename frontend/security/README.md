# Security Guidelines

- Container security
  - Refer to [Dynamic Application Security Testing (DAST) | GitLab](https://docs.gitlab.com/ee/user/application_security/dast/)
- Don’t hardcode key
- Make sure of SQL Injection, XSS, CSRF etc related handling with relation to the frameworks used
- [TBD] How about internal Bug Bounty program
- Tools may not be able to discover design / business log flaws
  - We must decide a way to fix this
  - [TBD] Possible checklist?
  - Biggest weakness is the webapp side modifying the request parameters.
  - [TBD] Consult to ML Security engineer
