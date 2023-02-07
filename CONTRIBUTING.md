# Contributing

This document aims to provide you with a general overview of what tools we use, but different projects have different guidelines when it comes to submitting code.

## DDEV / Docker

For working locally you need to use [ddev](https://ddev.readthedocs.io/). We use the default ports (80 & 443) of ddev to develop, but if you need to run
ddev on different ports you can alter the global config with the ports values you find in the [configuration reference](https://ddev.readthedocs.io/en/stable/users/configuration/config/).

Some repos use docker directly. But it is a dependency of ddev anyways, so we just mention it here.

## Task

As an alternative to make we often use [task](https://taskfile.dev/). Make sure it's installed

## NVM 

We use [nvm](https://github.com/nvm-sh/nvm) to set a per project node version. For a comfortable setup look at https://github.com/nvm-sh/nvm#deeper-shell-integration.

## Other dependencies

These are dependencies which are usually installed on a system anyways, but make sure that they are present:

- Python (>= 3.10)
- rsync (If you are on macOS make sure to install a recent version from brew.)
- ssh client (We will use the ssh public keys you provided to Github for managing access.)
- make (It does not need to be GNU Make, but that is the base it should be compatible with.)
- git (Github Desktop is fine, and you get bonus points for signing your commits)
