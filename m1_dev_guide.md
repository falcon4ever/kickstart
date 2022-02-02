# Intro

This guide shows you how I set up my M1 / Apple Silicon machine to be productive as a developer at work as well for personal projects. Hopefully it will be helpful to you as well.

## Generating a new SSH Key

If you haven't already done this... GitHub provides a very good guide on how to create a new SSH key and updating your local `~/.ssh/config`.

I highly recommend using this [Generating a new SSH key and adding it to the ssh-agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) guide

And then following this [Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) to install the SSH Key

GitHub is also a nice place to store your public/private projects.

# XCodes

Don't install XCode via the AppStore unless:

* You don't mind waiting hours for it to install
* You don't mind that an overnight automatic upgrade and realizing you're suppose to ship something that morning.

A better way to install XCode is to use XCodes (either the app or the commandline tool):
https://github.com/RobotsAndPencils/XcodesApp

(You will need an apple developer account...)

# Homebrew

It's great.

https://brew.sh

# Ruby

Don't use the pre-installed Ruby build. Get a something newer using rbenv. 

Follow these instructions to install rbenv: https://github.com/rbenv/rbenv#installation

    brew install rbenv
 
 Install a Ruby version:

    rbenv install 2.6.9
    rbenv global 2.6.9

    lmuller@retro ~ % ruby --version
    ruby 2.6.9p207 (2021-11-24 revision 67954) [arm64-darwin21]

For iOS devs:

    gem install bundler
    gem install cocoapods


# Java / OpenJDK

For Android development you probably will need a JDK. You could use the embedded one or [Azul Zulu OpenJDK](https://www.azul.com/downloads/?version=java-11-lts&os=macos&package=jdk) is a great alternative (especially if you plan to do some KMM or Java development).

The link above will take you to the `Java 11 (LTS)` version. Select macOS, ARM64-bit and the JDK. Download the dmg & install.

# Python

Don't use the pre-installed Python build. Get a something newer using pyenv.

Follow these instructions to install pyenv: https://github.com/pyenv/pyenv

    brew update
    brew install pyenv

Install a Python version:

    pyenv install 3.9.9
    pyenv global 3.9.9

List of versions: https://www.python.org/doc/versions/

# Node.js

While you can install node from https://nodejs.org/en/ using nvm is easier and allows you to switch between different versions (similar to rbenv/pyenv).

Follow these instructions: https://github.com/nvm-sh/nvm

    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash


# Docker

🐳: https://www.docker.com/get-started

Just pick the right architecture - apple chip

# JetBrains Toolbox

If you are going to use Android Studio, IntelliJ IDEA, PyCharm etc, it's much easier to install it through the [JetBrains Toolbox](https://www.jetbrains.com/toolbox-app/). It will allow you to install multiple versions side by side and makes updating a breeze.

# Visual Studio Code

A great editor: https://code.visualstudio.com

# Sourcetree

Sometimes it's nicer to use one app to manage all your repos: https://www.sourcetreeapp.com

# Notes

Other tools I use:
* https://folivora.ai/bettersnaptool
* https://bjango.com/mac/istatmenus/
* https://signal.org/en/download/
* https://brave.com/
* https://bitwarden.com/