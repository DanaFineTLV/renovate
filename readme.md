![Renovate banner](images/cli_banner.png)

# What is Renovate?

Renovate is an automated dependency update tool.
It helps to update dependencies in your code without needing to do it manually.
When Renovate runs on your repo, it looks for references to dependencies (both public and private) and, if there are newer versions available, Renovate can create pull requests to update your versions automatically.

## Features

- Delivers updates directly to your code base
  - Relevant package files are discovered automatically
  - Pull Requests automatically generated in your repo
- Provides useful information to help you decide which updates to accept (age, adoption, pass rates, merge confidence)
- Highly configurable and flexible to fit in with your needs and repository standards
- Largest collection of languages and platforms (listed below)
- Connects with private repositories and package registries

**Languages**<br>
Renovate can provide updates for nearly all languages, platforms and registries including: npm, Java, Python, .NET, Scala, Ruby, Go, Docker and more.
Supports over 90 different package managers.

**Platforms**<br>
Renovate updates code repositories on the following platforms: GitHub, GitLab, Bitbucket, Azure DevOps, AWS Code Commit, Gitea, Forgejo, Gerrit (experimental)

#  Ways to Run Renovate

The easiest way to run Renovate is to use a job scheduling system that regularly runs Renovate on all enabled repositories and responds with priority to user activity.

Mend provides pre-built systems for automatically running Renovate on your repositories.

## Mend Renovate App (Cloud)

**Supports: GitHub.com, Bitbucket Cloud**<br>
Hosted by Mend.io. No setup required. Community plan available (Free)

* GitHub Cloud: Install the [Renovate App](https://github.com/apps/renovate) on your GitHub org, then select the repos to enable
* Bitbucket Cloud: Add the [Mend App](https://marketplace.atlassian.com/apps/1232072/mend) to your Workspace, the add the Mend Renovate user to the projects you want to enable

## Mend Renovate Server (Self-hosted)

**Supports: GitHub, GitLab, Bitbucket Data Center**<br>
Install and run your own Renovate server. Access internal packages.

* [Mend Renovate Community Edition](https://github.com/mend/renovate-ce-ee/tree/main/docs) (Free)
* [Mend Renovate Enterprise Edition](https://www.mend.io/mend-renovate/) (Paid plan)

## Other ways to run Renovate
If you can’t use a pre-built job scheduling system, or want to build your own, the following options are available:

### Run Renovate on your Pipeline
Mend provides a _**GitHub Action**_ and _**GitLab Runner**_ to make it easier to run Renovate as a CI pipeline job.

* GitHub Action: [renovatebot/github-action](https://github.com/renovatebot/github-action).
* GitLab Runner: [Renovate Runner project](https://gitlab.com/renovate-bot/renovate-runner/)
* AzureDevOps action: [Renovate Me extension](https://marketplace.visualstudio.com/items?itemName=jyc.vsts-extensions-renovate-me)<br>
_Note: This extension is created and maintained personally by a Renovate developer/user so support requests relating to the extension itself cannot be answered directly in the main Renovate repository._
* Custom pipeline: You can create a custom pipeline with a **yml** definition that triggers **npx renovate**. [More details on how to configure the pipeline](https://docs.renovatebot.com/modules/platform/azure/).

### Run Renovate CLI
There are several ways to run the Renovate CLI directly. See docs: [Running Renovate](https://docs.renovatebot.com/getting-started/running/) for all options.<br>
**Targets: all platforms**

# Docs

### More about Renovate
- Renovate basics
  - [Why use Renovate](https://docs.renovatebot.com/#why-use-renovate)
  - [What does it do? / How does it work?](https://docs.renovatebot.com/key-concepts/how-renovate-works/)
  - [Who is using it?](https://docs.renovatebot.com/#who-uses-renovate)
- Supported platforms and languages
  - [Supported platforms](https://docs.renovatebot.com/#supported-platforms)
  - [Supported languages / package managers](https://docs.renovatebot.com/modules/manager/)
- Advanced renovate usage
  - [Accessing private packages](https://docs.renovatebot.com/getting-started/private-packages/)
  - [Merge Confidence data](https://docs.renovatebot.com/merge-confidence/)

### Renovate Docs
- [Renovate Configuration](https://docs.renovatebot.com/configuration-options/)
- [Mend Renovate Server Docs](https://github.com/mend/renovate-ce-ee/tree/main/docs)

### Comparisons
- [Different ways to run Renovate](https://www.mend.io/renovate/)
- [Renovate vs Dependabot Comparison](https://docs.renovatebot.com/bot-comparison/)

# Get involved

### Issues and Discussions
We prefer all items to be opened as a discussion before opening an issue.
- [GitHub Discussions forum
](https://github.com/renovatebot/renovate/discussions)
### Contributing
To contribute to Renovate, or run a local copy, please read the contributing guidelines.
- [Guidelines for Contributing](https://github.com/renovatebot/renovate/blob/main/.github/contributing.md)
- Items that need contribution: [good first issues](https://github.com/renovatebot/renovate/contribute)

### Contact and Social Media
The Renovate project is proudly supported and actively maintained by Mend.io.
- Contact [Mend.io](http://Mend.io) for commercial support questions.

Follow us on Twitter, LinkedIn and Mastodon.
- Twitter: [x.com/mend_io](http://x.com/mend_io)
- LinkedIn: [linkedin.com/company/mend-io](https://linkedin.com/company/mend-io)

