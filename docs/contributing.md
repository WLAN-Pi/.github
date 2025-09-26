# Contributing

First off, thank you for being awesome and looking into contributing to the multiple applications and OS powering the WLAN Pi. This page aims to help you get started.

The [Open Source Guides](https://opensource.guide/) website has a useful collection of resources for folks who want to learn how to run and contribute to open source projects. Both seasoned contributors and people new to open source will find the guide useful.

- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)

## Code of Conduct

WLAN Pi adopts the [Contributor Code of Conduct](code_of_conduct.md) and expects contributors to adhere to. By participating you agree to follow its terms. Please read the full CoC text so you understand what is and is not acceptable behavior. If you do not agree with our code of conduct, please do not contribute.

## Policy

Additionally, WLAN Pi does not endorse, support, or condone the use of its software for malicious, illegal, or unethical purposes, or to cause direct or indirect harm. By contributing to the software used by WLAN Pi, you agree to comply with all applicable laws and ethical standards. If you don't agree with these terms, please do not contribute. [Disclaimer](disclaimer.md).

## AI and LLM Assistance Disclosure

When contributing code to WLAN Pi, please disclose if you have used AI tools, large language models (LLMs), or other automated code generation services to assist in developing your contribution. This includes tools like GitHub Copilot, ChatGPT, Claude, or similar AI-powered coding assistants.

While we welcome the use of these tools to enhance productivity and code quality, transparency about their usage helps maintainers better understand the code's origin and ensures proper review processes. Please mention any AI assistance in your pull request description, noting which tools were used and to what extent they contributed to the code changes.

## Getting Involved 

We're thrilled that you'd like to contribute to this project. And people like you make WLAN Pi a great tool. One of the best places to start is by working on something that you use. Ideally, start with fixing a bug or issue that directly bothers you.

There are different ways to contribute to WLAN Pi and some of them don't include writing any code.

- If you've noticed a bug or have a specific feature request, make one! Notice multiple bugs? Create separately focused issues for each.

- If you're fixing a bug, open an issue on the respective repo, and then submit and link a PR to that issue. For new features, you're awesome! Thanks! Please consider talking to a team member and starting a [discussion](https://github.com/WLAN-Pi/feedback/discussions/categories/general-feedback) before spending too much time on coding to make sure everyone is on the same page.

- Are you working on code already? Cool! Please open an issue (is the issue reproducible? how so?) or feature request (does the feature fit with the project?) before getting too far.

- Have you never contributed to open source before? That's OK! Contributing to open source could be anything from updating documentation, triaging issues, and bugs, or writing code.

## Triaging Issues and Pull Requests

One way you can contribute without writing any code is to help triage issues and pull requests.

- Ask for more information if you believe there are not enough details to solve the issue.
- Flag issues that are stale or that should be closed.
- Ask for test plans and review code.

Unsure what Pull Requests are?

- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)

## Questions

Please note that the various GitHub issue trackers are mostly for *bug reports* and *feature requests*. Please do
not use GitHub issues to ask questions about usage. These questions should instead be directed through the [feedback discussions](https://github.com/WLAN-Pi/feedback).

## Good Bug Reports

Please be aware of the following things when filing bug reports:

1. Avoid raising duplicate issues. *Please* use the GitHub issue search feature
to check whether your bug report or feature request has been mentioned in
the past.

2. When filing bug reports about exceptions or tracebacks, please include the
*complete* traceback. Partial tracebacks, or just the exception text, may not be enough for us to help you.

3. Make sure you provide a suitable amount of information to work with. This
means you should provide:

- Guidance on **how to reproduce the issue**. Ideally, this should be a
 *small* code sample that can be run immediately by the maintainers.
 Failing that, let us know what you're doing, how often the issue happens, what
 environment you're using, etc. Being thorough will prevent us needing to ask
 further questions.
- Tell us **what you expected to happen**. When we run your example code,
 what are we expecting to happen? What does "success" look like for your
 code?
- Tell us **what actually happens**. It's not helpful for you to say "it
 doesn't work" or "it fails". Tell us *how* the failure happens: do you get an
 exception? How was the actual result different from your expected result?
- Tell us **what version you're using**, and
 **how you installed it**. Different versions behave
 differently and have different bugs.
- Tell us **where the bug is in the code** if you know. This helps other developers quickly resolve the bug if you are not solving it yourself.

If you do not provide all of these things, time to resolution will take us much longer to
fix your problem. If we ask you to clarify something and you never respond, we
will close your issue without fixing it.

## Development Process

WLAN Pi uses [GitHub](https://github.com/wlan-pi) as our source of truth. The core team works directly here and all changes are public.

Pull Requests will be checked using GitHub actions to run tests, style tests, builds, and more.

### Issues

When opening a new issue, always make sure to fill out the issue template. This step is very important! Not doing so may result in your issue not being managed in a timely fashion. Don't take this personally if this happens, and feel free to open a new issue once you've gathered all the information required by the template.

Again, please don't use the GitHub issue tracker for questions. If you have questions about using WLAN Pi, use any of our support channels, and we will do our best to answer your questions.

### Bugs

WLAN Pi uses GitHub Issues for our public bugs. If you would like to report a problem, take a look around and see if someone already opened an issue about it. If you are certain this is a new, unreported bug, please submit a bug report.

- One issue, one bug: Please report a single bug per issue.
- Provide reproduction steps: List all the steps necessary to reproduce the issue. The person reading your bug report should be able to follow these steps to reproduce your issue with minimal effort.

If you're only fixing a bug, it's fine to submit a pull request right away but we still recommend filing an issue detailing what you're fixing. This is helpful in case we don't accept that specific fix but want to keep track of the issue. The PR should be closing an issue #.

## Development 

Your code contributions should follow the same conventions and pass the same code quality checks as the rest of the project. Take a look around at the rest of the code in the particular project for ideas. Match the style you see used throughout the project such as formatting, naming files, etc.

If you're writing documentation, please do not wrap lines. Configure your editor to softwrap for documentation.

With that said, our documentation, style, and conventions are a work in progress welcoming suggestions for improvement. Check out [WLAN-Pi/developers](https://github.com/WLAN-Pi/developers) to find our developer docs around code style, workflow, and processes.

## Submitting a pull request

Ok, so you want to contribute code to WLAN Pi by opening a pull request. You're invested. Thank you, we appreciate this.

Checklist:

0. Keep your PR small. These are easier to review and get merged. Your PR in general should only do one thing. Otherwise, likely needs split into multiple PRs.
0. Use descriptive titles. Start with feat, fix, docs, refactor, test, or chore. Follow with a summary in the present tense. for example: `fix: address profiler crash on Rx of certain (re)assoc frames`.
0. Test your changes. Describe how to test and validate your contribution.

Generally, this is the process you'll follow:

0. Create an issue in the corresponding repository which the PR will close.
0. Fork and clone the repository you want to contribute to
0. Configure and install the dependencies
0. Make sure the tests pass on your machine (if the repository has tests)
0. Create a new branch: `git checkout -b <branch name>` (for how to name your branch see [https://github.dev/WLAN-Pi/developers])
0. Make your change, add tests, and make sure the tests still pass (if the repository has tests)
0. Push to your fork and submit a pull request
0. Pat yourself on the back and wait for your pull request to be reviewed and merged

We use Github Actions which will run our CI/CD to archive and deploy packages. In some repos, Github actions will run test suites and other checks. These must pass before a PR will be accepted and merged.

## Breaking Changes

If you're adding breaking changes, make sure to note that in the PR.


```
1. Who is affected
2. What needs migrated
3. Why this breaking change
4. Severity
```

## Get the documentation right

Make sure you submit any corresponding documentation updates along with your code. This might look different depending on what your change is. For example, a bug fix requires less documentation than a new feature but is still important to note in commit messages and changelogs.

If your PR is to add a new feature, the odds are documentation will need updated in multiple places. For example usage guides, README.md for the respective repo, man pages, and even our documentation website [docs.wlanpi.com](https://docs.wlanpi.com).

## Getting your Pull Request accepted

Here are a few things you can do that will increase the likelihood of your pull request being accepted:

- Follow standards for style and code quality.
- Documentation.
- Write tests.
- Keep your change as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
- Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

##  Merging a PR (maintainers only)

A PR should only be merged into the default branch if:

* PR is passing CI (tests/checks).
* PR has been approved by a code owner.
* PR has no requested changes by a reviewer.
* PR is up to date with the default branch and does not erase or re-write history.

PRs should be squash-merged into the default branch.

## Shipping a release (maintainers only)

Maintainers need to do the following to push out a release:

* Switch to the `main` branch and make sure it's up to date.
* Update the version info in `debian/changelog` which will trigger a workflow on push to build and deploy a new version of the package to packagecloud. This CI will also check that the Python package version (`<package>/__version__.py`) aligns with the Debian package version (`debian/changelog`).
* Update release notes accordingly

