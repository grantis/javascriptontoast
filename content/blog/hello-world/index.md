---
title: Node Version Manager
date: "2015-05-01T22:12:03.284Z"
description: "How to use nvm"
---

`nvm` or Node Version Manager is the easiest way to have all your NodeJs projects working correctly and on the version they require. By using nvm you no longer need to manage this dependency manually. Hooraa!! 🎉🎉🎉

# Setup and Install

Assuming you have Node installed. Run:

`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.2/install.sh | bash`

This command uses curl to download the install script and pipe it into bash to run. nvm is cloned into `~/.nvm` and will add nvm to your
`~/.bash_profile`, `~/.profile`, `~/.bash_rc` or `~/.zshrc` in order to run globally.

# Automatically switch node versions 🚀

## .nvmrc

[From `nvm`'s usage guide](https://github.com/nvm-sh/nvm#nvmrc)

You can create a .nvmrc file containing a node version number (or any other string that nvm understands; see nvm --help for details) in the project root directory (or any parent directory). Afterwards, `nvm use`, `nvm install`, `nvm exec`, `nvm run`, and `nvm which` will use the version specified in the `.nvmrc` file if no version is supplied on the command line.

For example, to make nvm default to the latest 5.9 release, the latest LTS version, or the latest node version for the current directory:

\$ echo "5.9" > .nvmrc

\$ echo "lts/\*" > .nvmrc # to default to the latest LTS version

\$ echo "node" > .nvmrc # to default to the latest version
Then when you run nvm:

\$ nvm use
Found '/path/to/project/.nvmrc' with version <5.9>
Now using node v5.9.1 (npm v3.7.3)

[`nvm` on Github](https://github.com/nvm-sh/nvm#install--update-script)
