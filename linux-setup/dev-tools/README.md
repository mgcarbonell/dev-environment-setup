# Installfest for Linux 2: The Parade Continues

## Text Editor

Our class will begin the course with [Visual Studio Code](../../mac-dev-tools/editor-vsc.md) as our preferred text editor. I tried to be cool and played around with some other ones (Atom, Sublime, ECMAS, and VIM), but VSCode is just so simple and has lots of support. And I totally get it, shilling for a MSFT product on Linux sounds weird, but trust me, it works. 

## Browser

The class will be using Chrome as the preferred browser. Through Pop!_OS there are two ways to get this browser.

### Method 1, the Prefered Way, go to Chrome

Open up Firefox, go to [Chrome's Official Website](https://www.google.com/chrome/), click on 'Download Chrome,' and get the **64 bit .deb (for Debian/Ubuntu)** package. Debian/Ubuntu make this really easy you navigate to where the package was downloaded to, double click on the package, and click 'Install' in Eddy!

### Method 2, the Command Line 

Open up your command line (Super + T) and copy (ctrl + c) the following and paste it (ctrl + shift + v) it into the command line.

``wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb``

After fetching the .deb file, using dpkg command to install it. 

``sudo dpkg -i google-chrome-stable_current_amd64.deb``

You are also going to want to install the [JSON View](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc) extension.

## Postman

Postman is tricky because in their documentation they want you to use a command called 'snap,' and I get it, you've probably heard sudo is the magic word to get anything you want from Linux. I'm going to tell you straight off the bat don't do what I did and try to install it manually by yourself. Why? Well, beyond installing it to the wrong folder and creating a fatal error you could do what I did and accidentally install it in your download folder. Everytime I wanted to use Postman I would have to navigate to Downloads -> Postman -> launch the exe. So let's just use Snap!

First, we're going to run the following command...

``sudo apt update``

It's always good practice to update first, and then...

``sudo apt install snapd``

Now that we have that, it's as simple as:

``snap install postman``

## Keyboard Shortcuts

Where would I be without ``super + tab``, ``super + t``, or any of the VSCode keyboard shortcuts? Well, still here, just a lot slower. Developers *love* keyboard shortcuts, the more keyboard shortcuts you know the faster you can code!

[Here](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf) helpful Linux keyboard shortcuts for Visual Studio Code, with one added addition: ``ctrl + shift + alt + arrow up/arrow down`` will copy an entire line and duplicate it below. 

When you have some time, check out the [Keyboard Shortcuts](https://support.system76.com/articles/pop-keyboard-shortcuts/) for Pop!_OS. 

You can also see the picture below as to how to customize your keyboard shortcuts, or turn off any that you might accidentally hit and don't want to.

![PopKeyboardShortcuts](../../assets/popkeyshortcuts.png)

## That's it!

![You did it!](https://media.giphy.com/media/3otPoS81loriI9sO8o/giphy.gif)
