# Awosome Fish
> A awosome Bash Shell on OS X.

## Install Homebrew
> The missing package manager for OS X.

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
> install node.js version you choose. After installation, you also have npm command now!

## Install fish
> fish is a smart and user-friendly command line shell for OS X, Linux, and the rest of the family.

```
$ brew install fish
```

Add fish to your shell list.

```
$ echo "/usr/local/bin/fish" | sudo tee -a /etc/shells
```

Set fish as your default shell.

```
$ chsh -s /usr/local/bin/fish
```

### Setting your fish

create fish config folder.

```
$ mkdir -p ~/.config/fish
```

create fish config file.

```
$ vim ~/.config/fish/config.fish
```

add one line command in this file.

```
set -g -x PATH /usr/local/bin $PATH
```

save this file and restart your shell. You will see fish.

```
$ fish_config
```
> you can setting fish on browser.

## Install fisherman
> A plugin manager for fish.

```
$ curl -Lo ~/.config/fish/functions/fisher.fish --create-dirs git.io/fisher
```

And you will get the install plungin command 

```
$ fisher mono
```

## Solution of you can't find npm command in fish.
> you need to let fish know what is npm, and you should use fisherman plungin for this problem.

```
$ fisher nvm
```

## Reference
1. [Homebrew](http://brew.sh/index.html)
2. [fish](https://fishshell.com/)
3. [oh-my-fish](https://github.com/oh-my-fish/oh-my-fish)
4. [fisherman](http://fisherman.sh/)
5. [install-fish-shell-on-os-x](http://jigsawye.com/2016/06/20/install-fish-shell-on-os-x/)
6. [nodejs-installation-guide](http://icarus4.logdown.com/posts/175092-nodejs-installation-guide)
7. [Getting-Started-Installing-Git](https://git-scm.com/book/en/v1/Getting-Started-Installing-Git)
