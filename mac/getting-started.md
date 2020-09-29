# Mac Getting Started
> Isn't it dark with no windows

You have it slightly easier than the Windows lot, but there’s still some work to do! Luckily for you people, 
a lot of the work is done for you and doesn’t require typing much.

## Step 1: Homebrew and Developer Tools
[Homebrew](https://brew.sh) will change and/or save your life as a Mac developer. It will also install the C compiler, 
amongst many other bits and pieces that will be super useful. So let’s do it!

Load up a Terminal window (from /Applications/Utilities) and paste the following command in, all on one line. 
Enter your password when it asks you to:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

**Tip:** when you're typing in your password, you won't actually see it being typed (not even the asterisks!).
Don't worry and just type your password and press Enter at the end. If you got it wrong, the Terminal will ask
you to try again!

Once installed, you may see some extra updates for the macOS Developer Tools in the Mac App Store. Go ahead and 
install those. Now back in terminal, run these commands:

```bash
brew install python3 ghc cabal-install stack
```

Once they are all installed (which may take some time!), you can continue with the rest of the guide for setting up
your IDEs.

## Step 2: Jetbrains Toolbox
The tools you use can transform development from being a chore to a joy. Having a consistent environment across all
languages is key. Throughout this guide we will be using the free (for students) Jetbrains tools, they have by
far the most advanced IntelliSense (auto code completion) capabilities, although sadly there is no tool for Haskell.

1. If you have not already, sign-up for the [Jetbrains Student Pack](https://www.jetbrains.com/student/).

2. Download the [Toolbox App](https://www.jetbrains.com/toolbox-app/) and sign in with your account. This will
automatically license any Jetbrains tools on your system.

### Note on IDE's
IDE's are a personal preference, this guide will primarily use Jetbrains where possible but you may wish to use
Visual Studio Code for everything instead.

## Step 3: Git
Git should already be installed, and you can verify that with:
```bash
git --version git
```
If not installed you can install with Homebrew:
```bash
brew install git
```

You can then configure your username and email:
```bash
git config --global user.name "Username"
git config --global user.email "Email-Use-Github-Anonymous"
```
To find your 
[github email address](https://docs.github.com/en/free-pro-team@latest/github/setting-up-and-managing-your-github-user-account/setting-your-commit-email-address) 
you can go here: https://github.com/settings/emails. You can also connect to github via 
[ssh](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/connecting-to-github-with-ssh).
