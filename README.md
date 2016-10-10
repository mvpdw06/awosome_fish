# Awosome Fish
> A awosome Bash Shell on OS X.

**Let me show you how to set fish for coding environment on your OS X.**

* [Install Homebrew](#install-homebrew)
* [Install iTerm2](#install-iterm2)
* [Install Git](#install-git)
* [Install nvm & npm](#install-nvm--npm)
* [Install fish](#install-fish)
  * [Install](#install)
  * [Setting your fish](#setting-your-fish)
* [Install fisherman](#install-fisherman)
  * [Solution of you can't find npm command in fish.](#solution-of-you-cant-find-npm-command-in-fish)
  * [Recommand git status plungin](#recommand-git-status-plungin)
* [Reference](#reference)

## Install Homebrew
> The missing package manager for OS X.

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## Install iTerm2
> iTerm2 is a terminal emulator for OS X that does amazing things.

Just go [here](https://www.iterm2.com/downloads.html) for download.

> After Intallation, you can replace your terminal emulator from default to iTerm2.

## Install Git
> fast-version-control management.

```
$ brew install git
```

## Install nvm & npm
> Node.js version management.

```
$ brew install nvm
```

And you can get nvm command to install node.js

```
$ nvm ls-remote
```

> list all node.js version you can install.

```
$ nvm install <version>
```
> Install node.js version you choose. After installation, you also have npm command now!

## Install fish
> Fish is a smart and user-friendly command line shell for OS X, Linux, and the rest of the family.

### Install

Step.1 Brew install fish

```
$ brew install fish
```

Step.2 Add fish to your shell list.

```
$ echo "/usr/local/bin/fish" | sudo tee -a /etc/shells
```

Step.3 Set fish as your default shell.

```
$ chsh -s /usr/local/bin/fish
```

### Setting your fish

Step.1 Create fish config folder.

```
$ mkdir -p ~/.config/fish
```

Step.2 Create fish config file.

```
$ vim ~/.config/fish/config.fish
```

Step.3 Add one line command in this file.

```
set -g -x PATH /usr/local/bin $PATH
```

Step.4 Save this file and restart your shell. You will see fish. Command "fish_config", and you can setting fish on browser.

```
$ fish_config
```

## Install fisherman
> A plugin manager for fish.

```
$ curl -Lo ~/.config/fish/functions/fisher.fish --create-dirs git.io/fisher
```

And you will get the install plungin command 

```
$ fisher <owner/git-repository-name>
```

For example, I want to install [RED SNAPPER](https://github.com/oh-my-fish/theme-red-snapper), and I should command like this.

```
$ fisher oh-my-fish/theme-red-snapper
```

### Solution of you can't find npm command in fish.
> You need to let fish know what is npm, and you should use fisherman plungin for this problem.

```
$ fisher nvm
```

### Recommand git status plungin
> You can see your git-status of current folder directly.

**[RED SNAPPER](https://github.com/oh-my-fish/theme-red-snapper)**

It's totally fish symbol in this plungin. Very funny and interesting!

```
$ fisher oh-my-fish/theme-red-snapper
```

> That's all this wrap, and Hope you will like it. Enjoy!

## Reference
1. [Homebrew](http://brew.sh/index.html)
2. [iTerm2](https://www.iterm2.com/)
2. [fish](https://fishshell.com/)
3. [oh-my-fish](https://github.com/oh-my-fish/oh-my-fish)
4. [fisherman](http://fisherman.sh/)
5. [install-fish-shell-on-os-x](http://jigsawye.com/2016/06/20/install-fish-shell-on-os-x/)
6. [nodejs-installation-guide](http://icarus4.logdown.com/posts/175092-nodejs-installation-guide)
7. [Getting-Started-Installing-Git](https://git-scm.com/book/en/v1/Getting-Started-Installing-Git)
