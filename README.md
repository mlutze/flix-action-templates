# Flix Action Templates

A collection of GitHub workflow templates for use with the Flix programming language.
These templates are intended for users maintaining Flix projects on GitHub,
especially Flix libraries and projects in the Flix community build.

## General Purpose

There are is one script intended for the typical Flix user:
- [test-pr-on-flix-release.yaml](./test-pr-on-flix-release.yaml): Runs tests on a specific Flix release, as specified in the project TOML.

## Development

One script is adapted to Flix developers and those running on the bleeding edge of Flix:
- [test-pr-on-flix-nightly.yaml](./test-pr-on-flix-nightly.yaml): Runs tests on the latest nightly Flix release.

## Community Build

Two scripts are intended for use by developers whose projects are in the Flix community build.

The first is for applications and libraries without dependents in the community build.
Their head commit must stay up-to-date with Flix head.
- [test-nightly-on-flix-nightly.yaml](./test-nightly-on-flix-nightly.yaml): Tests the latest commit against the latest nightly Flix release.

The second is for libraries with dependents in the community build.
Their latest release must stay up-to-date with Flix head.
- [test-release-on-flix-nightly.yaml](./test-release-on-flix-nightly.yaml): Test the latest release against the latest nightly on Flix release.
