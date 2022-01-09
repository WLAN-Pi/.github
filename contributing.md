# Contributing

First off, thank you for being awesome and looking into contributing to WLAN Pi. We're thrilled that you'd like to contribute to this project. And it is people like you that make WLAN Pi a great tool.

Please note that WLAN Pi releases software under the [Contributor Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). Please review it. By participating you agree to follow its terms. If you don't vibe with the code of conduct, consider not contributing.

## Where do I go from here?

If you've noticed a bug or have a specific feature request, make one! 

Please get confirmation and approval of your bug (is it reproducible? how so?) or feature request (does it fit with the project?) before starting to code. If you're fixing a bug, open an issue on the respective repo. For features, start a [discussion](https://github.com/WLAN-Pi/feedback/discussions/categories/general-feedback) before coding.

## Get the style right

Your code should follow the same conventions & pass the same code quality checks as the rest of the project. 
Check out [WLAN-Pi/developers](https://github.com/WLAN-Pi/developers) to find documentation around style, workflow, processes, and more.

## Submitting a pull request

Generally, this is the process you'll follow:

0. Fork and clone the repository you want to contribute to
0. Configure and install the dependencies
0. Make sure the tests pass on your machine (if the repository has tests)
0. Create a new branch: `git checkout -b my-branch-name` (`fix/short_bug_desc` or `feature/widget`)
0. Make your change, add tests, and make sure the tests still pass (if the repository has tests)
0. Push to your fork and submit a pull request
0. Pat your self on the back and wait for your pull request to be reviewed and merged

We use Github Actions which will run our CI/CD to archive and deploy packages. In some repos, Github actions will run test suites. These must pass before a PR will be accepted and merged.

## Get the documentation right

Make sure you submit documentation along with your code. This might look different depending on what your change is. A bug fix requires less documentation than a new feature.

If your PR is to add a new feature, it is likely documentation will need updated in multiple places. Usage guides. The README.md for the respective repo. Our documentation website [docs.wlanpi.com](https://docs.wlanpi.com).

## Here are a few things you can do that will increase the likelihood of your pull request being accepted:

- Follow standards for style and code quality.
- Documentation.
- Write tests.
- Keep your change as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
- Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

##  Merging a PR (maintainers only)

A PR can only be merged into `main` by a maintainer if:

* It is passing CI.
* It has been approved by at least one core maintainers.
* It has no requested changes.
* It is up to date with current `main`.

Any maintainer is allowed to merge a PR if all of these conditions are met.

## Shipping a release (maintainers only)

Maintainers need to do the following to push out a release:

* Switch to the `main` branch and make sure it's up to date.
* Update the version info in `debian/changelog` which will trigger a workflow on push to build and deploy a new version of the package to packagecloud. 
* Update release notes

## Resources

- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub Help](https://help.github.com)
