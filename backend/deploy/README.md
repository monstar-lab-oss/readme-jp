# Build and Deployment Guidelines

## Docker

- [TBD] Prepare necessary docker files
  - Image size => should be as much small as possible
    - Build, deploy and container start gets faster
- Services

  - DockerHub
  - Github Container Registry
    - Permissions are easy to manage
    - Is there any other drawback?

## Github Actions

Use for testing and deployment

- [Pricing · Plans for every developer](https://github.com/pricing)
  - https://docs.github.com/en/github/setting-up-and-managing-billing-and-payments-on-github/about-billing-for-github-actions
- [TBD] Create usage template/ actions
  - Can actions be private? => need to confirm
    - https://docs.github.com/en/actions/learn-github-actions/sharing-workflows-with-your-organization
  - Is it okay to keep it as public? => may be, should keep the secrets/ important parameters as Env Var over Github
- Will vary on language/ stack
