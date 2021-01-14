# Installfest Step 1: Development Environment Setup

Whew, welcome to Installfest! It can be kind of daunting, I know for me it was because I had all this Mac documentation in front of me and I was on Linux. I even tried to install some of the tools for Mac on Linux until I got stuck and asked my instructor for help who then told me I didn't need to do most of what was going on (Linux for the win). 

## Operating System & Command Line Tools

You've probably read Pop!_OS ad nauseam by now, but it's the distribution that I'm the most familiar with and it is so similar to Ubuntu that anything done on Pop can be done on Ubuntu. That being said, a lot of this is written assuming you're using Pop.

So, before we get started we're going to do a simple:

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

## Customization

### Styles (Optional)



## Git



### Confirm Install



### Configure Git


```

## Next Up
* [Install Development Tools](../)

