# Installfest for Linux: The Penguin Parade

## The Choices

At the time of writing this, I made it through my entire bootcamp using the Pop!_OS distrubtion of Linux without any major hiccups. In fact, it was my *first time ever* using Linux! Using Pop!_OS is  **highly recommend** for new users,  however we also recommend seasoned veterans use Pop!_OS  **to maintain consistency across Linux users for debugging**. Using other environments can lead to unstable behavior and limit our ability to help you debug.

If you have some strong aversion to an OS named Pop!_OS because it's not professional enough, then I would strongly recommend the distribution Pop! is built off, and one of the most ubiquitous distributions: Ubuntu. Just know that at the time of writing I am using Pop!_OS.

## Operating System & Command Line Tools

Before we get started we're going to do a simple:

``sudo apt update && sudo apt upgrade``

To make sure all our packages are up to date. By the way, if you're a first time Linux user congratulations on chaining your first commands!


### Install Command Line Tools from the Terminal

While bash is loved by all and amazing most of your cohort will be using Zsh (Zshell). I recommend using Zsh because it's customizable (below) and offers tab completion which can be a time saver when navigating through files!

To install Zsh we're going to enter:

``sudo apt install zsh``

Alright, cool! Now, to make sure it's been installed correctly we're going to run the following in terminal:

``zsh``

If you are not greeted with a 'zsh-newuser-install' that walks you through some basic Zsh configuration you may need to invoke it manually:

``zsh /usr/share/zsh/functions/Newuser/zsh-newuser-install -f``

**Note**: Terminal size might need to be at least 72*15 or *zsh-newuser-install* may not run.

Finally, to make Zsh our default shell we're going to enter:

``chsh -s /bin/zsh``

You may have to log out and back in, but then you should be in Zsh!

More in depth writeups can be found here:

[Installing Zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH) from Oh-My-Zsh

[Zsh](https://pop-planet.info/wiki/index.php?title=Zsh) from Pop!_Planet

## Customization

### Styles (Optional)

Here comes the fun part: Oh-My-Zsh. Oh-My-Zsh is "A delightful community driven framework for manging your zsh config." This is a lot of words for: Make your shell look awesome. 

[Here's](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes) an exhaustive list of themes. The default shell is going to be robbyrussel. A very popular one is agnoster. I personally use [powerlevel10k](https://github.com/romkatv/powerlevel10k).


## Git

You should already have git installed and have an account on GitHub from Fundamentals. If not, sign up for an account on github.com. We'll be using GitHub to track code changes and collaborate on projects.


### Confirm Install

To check if we have git enter ``which git`` into your terminal. The output should be a directory path like ``/usr/bin/git``. If you do not see this, git is not installed on your machine. Go [here](https://github.com/git-guides/install-git), scroll down to Linux, follow the Debian/Ubuntu instructions.

### Configure Git

Configuring your git settings will help GitHub track your contributions and to make it easier and smoother to commit changes.

1. Use the following three `git config` commands to configure your git user information and have git "cache" (remember) it. We use the `--global` (or `-g`) option to make the configuration apply to all repositories.

<p align="center">
<img src='../assets/gitconfig.png' width='600px' alt='git config'>
</p>

To view your git configurations, you can either run following commands on the terminal

```
git config --list
```
OR

```
git config user.name
git config user.email
```


## Next Up
* [Install Development Tools](./dev-tools/README.md)

