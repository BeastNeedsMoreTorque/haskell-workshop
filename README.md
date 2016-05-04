# haskell-workshop

Haskell Workshop - Spring 2016

## Overview

This is intended to be a zero-to-something introduction to Haskell for working programmers who are
interested in functional programming, but don't know where to start.

We assume a basic knowledge of web development in this tutorial. If you're familiar with basic
client/server interaction and HTML, this tutorial should be easy to follow!

The workshop will consist of two parts:

1. Matt Parsons will present an overview of the syntax/look and feel of Haskell, so you won't get lost! You can
follow along with this section using the `Syntax.hs` source file.
2. Benjamin Kovach will walk you through an implementation of a simple web application that reads posts from
multiple subreddit listings concurrently and presents them to a user in a web browser. We will work through this
together, fleshing out `MyReddit.hs` as we go.

## Getting Started

### Prerequisite tools you'll need

#### git

A version control system. You'll need this to pull down the boilerplate code located in this repository.

Installation instructions are located here, for various operating systems.

https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

#### stack

The haskell toolchain and package manager. Stack will install the Haskell compiler for you _and_ manage the dependencies of your project.

Installation instructions are located here, for various operating systems:

http://docs.haskellstack.org/en/stable/install_and_upgrade/#mac-os-x

#### a computer

You'll need this to compile and run your project.

#### an open mind

Haskell might look strange at first, but it's no more difficult than any other language! Keep an open mind and you'll be writing your own code in no time.

### Setting up the project

To get the project set up, you'll need to run the following series of commands:

```bash
$ git clone https://github.com/sellerlabs/haskell-workshop
$ cd haskell-workshop
$ stack setup
$ stack install
```

**This will take a long time the first time you do it!** If all goes well, you should see something along the following lines:

```
Copying from /Users/Ben/projects/haskell-workshop/.stack-work/install/x86_64-osx/lts-5.13/7.10.3/bin/redditui to /Users/Ben/.local/bin/redditui

Copied executables to /Users/Ben/.local/bin:
- redditui
```

If `/Users/$USER/.local/bin` is properly set in your `PATH`, you should be able to do this:

```hs
$ redditui
redditui: Not implemented...yet!
```

At this point, you should be good to go!
