# Contributing

First off, thank you for being awesome and looking into contributing to WLAN Pi. We're thrilled that you'd like to contribute to this project. And it is people like you that make WLAN Pi a great tool.

This is important. Please note that WLAN Pi releases software under the [Contributor Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). By participating you agree to follow its terms. If you do not agree with our code of conduct, do not contribute.

## Where do I go from here?

If you've noticed a bug or have a specific feature request, make one! 

Are you working on code already? Cool! Please open an issue (is it reproducible? how so?) or feature request (does it fit with the project?) before getting too far.

If you're fixing a bug, open an issue on the respective repo, and then submit and link a PR to that issue. For new features, you're awesome! Thanks! Please consider talking to a team member and starting a [discussion](https://github.com/WLAN-Pi/feedback/discussions/categories/general-feedback) before spending too much time on coding to make sure everyone is on the same page.

Have you never contributed to open source before? Check out the resources at the bottom of this post.

## Get the style right

Your code should follow the same conventions & pass the same code quality checks as the rest of the project. With that said, our documentation, style, and conventions is a work in progress. We could use help. Check out [WLAN-Pi/developers](https://github.com/WLAN-Pi/developers) to find our developer docs around code style, workflow, processes, and more.

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

Make sure you submit documentation along with your code. This might look different depending on what your change is. For example, a bug fix requires less documentation than a new feature, but is still important.

If your PR is to add a new feature, it is likely documentation will need updated in multiple places. For example: usage guides, README.md for the respective repo, and even our documentation website [docs.wlanpi.com](https://docs.wlanpi.com).

## Getting your Pull Request accepted

Here are a few things you can do that will increase the likelihood of your pull request being accepted:

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
- [Figuring out how to contribute to open source](https://jvns.ca/blog/2017/08/06/contributing-to-open-source/)
- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub Help](https://help.github.com)
