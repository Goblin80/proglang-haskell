# proglang-haskell

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Goblin80/proglang-haskell)


## Gitpod

> Gitpod is an open source platform for automated and ready-to-code development environments that blends into your existing workflow. It enables developers to describe their dev environment as code and start instant and fresh development environments for each new task directly from your browser.


![](https://www.gitpod.io/images/docs/gitpod-architecture.png)

## What's inside?

*Using `fpco/stack-build` as a base image.*

* GHC (patched)
* Stack
* cabal-install
* Happy
* Alex
* ...

and system developer libraries required to build all Stackage packages.

## New project

```bash
$ stack new YourProject # Create a project
$ cd YourProject
$ stack setup # Setup everything, this can take a while
$ stack build # Build everything
```

## Install QuickCheck

1. Locate the `package.yml` file inside your project.
1. Append `QuickCheck` to the list of dependencies and save.
1. Run `stack build`.

```yaml
dependencies:
- base >= 4.7 && < 5
- QuickCheck
- containers
- ...
```

---

## Cold start

When you first create a workspace, it takes time to pull the base image and allocate necessary resources, please be patient.

**Subsequent runs should be faster.**

## Persist changes

> Gitpod backs up the state of the `/workspace/` folder between workspace starts, so that you can revisit them later.

**Attention: Files in other locations will not be saved!**

## Timeout

> Any running workspace will automatically stop after some time of inactivity. Normally, this timeout is 30 minutes.

> The timeout will always be reset to the full 30 minutes (or other applicable timeout depending on your subscription) by any activity — mouse move or keystroke — in the IDE.


## IDEs

From the settings menu, you can choose between VS Code or Theia the default IDE for you workspaces.

![IDEs](https://i.imgur.com/gnH2Fww.png)