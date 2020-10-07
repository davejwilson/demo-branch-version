# Maven Git Versioning Demo

## Background
The first objective is to be able to provide release candidate version for each commit on a "release" branch.
The second objective is to be able to make snapshot version for non-release branches that are easy to identify.

## Conventions Used
For release versions the date, time and short git hash is used as the version.
For snapshot versions the branch name is used as prefix for the snapshot version.
The convention used is branch-based.  
If the branch is `main` or `master` or the branch starts with `hotfix`, a release version is used, otherwise a snapshot using the branch name.

## Format Used
For release branches: `${git.commit.time}.${git.commit.id.abbrev}` e.g. `20201007-120033.12604f6`  
For any other branches: `${git.branch}-SNAPSHOT` e.g. `mybranch-SNAPSHOT`