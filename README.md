# Maven Git Versioning Demo

## Background
The first objective is to be able to provide release candidate version for each commit on a "release" branch.
The second objective is to be able to make snapshot version for non-release branches that are easy to identify.

## Conventions Used
For release versions the date, time and short git hash is used as the version.
For snapshot versions the branch name is used as prefix for the snapshot version.
The convention used is branch-based. If the branch is `main` or `master`, a release version is used, otherwise a snapshot using the branch name.
