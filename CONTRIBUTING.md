# Contributing

This document aims to provide you with a general overview of what tools we use,
but different projects have different guidelines when it comes to submitting 
code.

Also check out the tools folder after reading this document, it contains some
tips and tricks that really can speed up development. Also tool-specific FAQs
will be documented there.

## DDEV / Docker

For working locally you need to [ddev](https://ddev.readthedocs.io/).

Some repos use docker directly. But it is a dependency of ddev anyways, so we
just mention it here.

## Task

As an alternative to make we often use [task](https://taskfile.dev/). Make sure
it's installed

## NVM 

We use [nvm](https://github.com/nvm-sh/nvm) to set a per project node version.
For a comfortable setup look at https://github.com/nvm-sh/nvm#deeper-shell-
integration.

## 1Password CLI

We use [1password](https://1password.com) for secret management. For easy
integration into our deployments we use the cli, which you will need to have
installed too: [1Password Command Line](https://1password.com/de/downloads/
command-line/)

## Other dependencies

These are dependencies which are usually installed on a system anyways, but
make sure that they are present:

- Python (>= 3.10)
- rsync (If you are on macOS make sure to install a recent version from brew.)
- ssh client (We will use the ssh public keys you provided to Github for
  managing access.)
- make (It does not need to be GNU Make, but that is the base it should be
  compatible with.)
- git (Github Desktop is fine, and you get bonus points for signing your
  commits)
- bash (not only sh, we have some bashisms in older projects)
