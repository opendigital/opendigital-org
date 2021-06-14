# 📘 GitLab Handbook: Developer Onboarding


    
# Developer Onboarding
## 
## Getting started with GitLab development

To start development, follow the instructions for the [GitLab Development Kit](https://gitlab.com/gitlab-org/gitlab-development-kit).


## GitLab Repositories

GitLab consists of many subprojects. A curated list of GitLab Repositories can be found at the [GitLab Engineering Projects](https://about.gitlab.com/handbook/engineering/projects) page.
Almost all repositories are available on both GitLab.com and dev.gitlab.org. We also mirror to dev.gitlab.org for availability reasons and [GitHub](https://github.com/gitlabhq) for historical reasons.
All issues should be filed on GitLab.com.

## Infrastructure

For everything related to infrastructure, check out the [Infrastructure handbook](https://about.gitlab.com/handbook/engineering/infrastructure). In particular [production architecture](https://about.gitlab.com/handbook/engineering/infrastructure/production/architecture) might be useful for onboarding.
If you need a VPS for any reason, it's probably easiest to set one up at DigitalOcean. Ask another developer for access.


## Basics of GitLab development

**Workflow**
Please see the [engineering workflow document](https://about.gitlab.com/handbook/engineering/workflow) in the handbook and read the [developer documentation](http://docs.gitlab.com/ee/development/README.html).
**Security**
Read the [developer security documentation](https://gitlab.com/gitlab-org/release/docs/blob/master/general/security/developer.md) prior to working on a security issue.
**Quality**
One of GitLab's strengths is its high quality of software. To achieve this we've introduced some requirements to all source code that is contributed. All requirements are mentioned in [the Contribution guide](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/CONTRIBUTING.md). Make sure you read and follow it.

**Dependencies**
GitLab can be installed through an Omnibus package or from source on different Linux distributions and macOS. In order to maintain portability, we need to avoid adding extra dependencies and use of exotic database extensions. Every time you choose between changes in the application code or adding new dependencies, you should give priority to the first because this is easier to maintain and set up. If you still need to bring new dependencies to GitLab, ask another developer or the CTO for advice.

**Submit your code**
In GitLab all code should go through a review process before it can be merged. Make sure you submit a merge request for any changes you've made. When the merge request is ready, it should be assigned to [someone else on the team](https://about.gitlab.com/handbook/engineering/workflow/code-review/). This person is then responsible for reviewing your code and merging it. Optionally, you can request another developer to help or review by writing a comment. If a merge request is not assigned, it will probably be ignored and create unnecessary delays.
Don't work on one task for multiple days before submitting a merge request. Even the biggest task can be split into smaller tasks. Try to submit a merge request for each part of the functionality. This means that we expect multiple merge requests per week from you. Smaller merge requests are more likely to receive good feedback and will get merged sooner.
Unless the change is very minor, or is fixing a bug that was introduced in the same version, create a changelog entry using the `[bin/changelog](https://docs.gitlab.com/ee/development/changelog.html)` [script](https://docs.gitlab.com/ee/development/changelog.html). Do not include your name in the entry as we only do that to give recognition to volunteer contributors.

