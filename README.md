<div align="center">

# DigData Training

In this repository we explain the practices and standards that we use in [DigData-EIRL](https://github.com/DigData-EIRL).

[![DigData-EIRL - digdatatraining](https://img.shields.io/static/v1?label=DigData-EIRL&message=digdatatraining&color=blue&logo=github)](https://github.com/DigData-EIRL/digdatatraining)
[![stars - digdatatraining](https://img.shields.io/github/stars/DigData-EIRL/digdatatraining?style=social)](https://github.com/DigData-EIRL/digdatatraining/stargazers)
[![forks - digdatatraining](https://img.shields.io/github/forks/DigData-EIRL/digdatatraining?style=social)](https://github.com/DigData-EIRL/digdatatraining/fork)

[![GitHub release](https://img.shields.io/github/release/DigData-EIRL/digdatatraining?include_prereleases=&sort=semver)](https://github.com/DigData-EIRL/digdatatraining/releases) [![issues - digdatatraining](https://img.shields.io/github/issues/DigData-EIRL/digdatatraining)](https://github.com/DigData-EIRL/digdatatraining/issues)

[![View site - GH Pages](https://img.shields.io/badge/View_site-GH_Pages-2ea44f?style=for-the-badge)](https://digdata-eirl.github.io/digdatatraining)

</div>

# Table of contents

- [Work on a project](#work-on-a-project)
	- [Pull requests](#pull-requests)
	- [Commits Style Guide](#commits-style-guide)
	- [Keep your Fork updated](#keep-your-fork-updated)
- [Considerations and references](#considerations-and-references)

## Work on a project

1. Fork the project repository.
2. Create a new branch from `main` in your fork. You must create a branch for each ticket. Example: `hotfix/login` or `feature/new-feature`.
3. Make code changes.
4. Commit and push. Remember that the commit must be a description of the change. Example: `fix: Login`.
5. Make pull request from your branch to the `develop` branch of the main repository.
6. Wait for the change to be accepted.

It is very important to separate new features or improvements into separate feature branches, and to send a pull request for each branch.

This allow us to review and pull in new features or improvements individually.

### Pull requests

All pull requests SHOULD adhere to the [Conventional Commits specification](https://conventionalcommits.org/).

Conventional Commits use the [GitHub flow](https://guides.github.com/introduction/flow/) as main versioning workflow.

### Commits Style Guide

The contribution guideline is derived from [ConventionalCommits.org](https://www.conventionalcommits.org/)

### Keep your Fork updated

When you have the Fork repository cloned on your PC, the first thing you have to do is create a remote to the original repository using: `git remote add upstream <repo_url>` (You only have to do this the first time you clone the repository).

Then every time a change is made in the original repository and you want to bring it to your fork use the following commands:

1. `git pull upstream develop`
2. `git push`

**Note:** remember to be located within the branch you wanna update.

As a good practice, it is always recommended to execute these two commands before starting to work, _(just in case there is any change)_:

1. `git pull upstream develop`
2. `gil pull`

## Considerations and references

- The commits must be well-written. Use the [Conventional Commits](https://conventionalcommits.org/) specification for each _commit_.
- Every change must be documented. Use the [GitHub Flavored Markdown](https://github.github.com/gfm/) specification to document your _changes_.
- [GitFlow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) is used to manage the _branches_.
