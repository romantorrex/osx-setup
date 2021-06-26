<h1 align="center">My Mac OSX Setup</h1>
<p align="center">This is documentation for my future self. Describes the tools that I use in my daily work and how to install/configure them in a computer with MAC OSX.</p>

##  Shell
I work with zsh, the default shell in Mac OSX. I use  [Oh My Zsh](https://ohmyz.sh/) to manage its configuration, plugins and themes. You have to install **Oh My Zsh** via command line as follows:

```
> sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

To make my shell a little bit prettier I use the free version of [Dracula Theme](https://draculatheme.com/zsh). To install dracula zsh theme using Oh My Zsh run these commands one by one:

```
> git clone https://github.com/dracula/zsh.git dracula-zsh
> DRACULA_ZSH_THEME=$PWD/dracula-zsh
> ln -s $DRACULA_ZSH_THEME/dracula.zsh-theme ~/.oh-my-zsh/themes/dracula.zsh-theme
```

And finally you have to **activate the dracula theme** by going to your `~/.zshrc` file and set `ZSH_THEME="dracula"`.

## Script
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

# terminal
brew cask install iterm2

# code editors
brew cask install visual-studio-code
brew cask install intellij-idea-ce
brew cask install macdown

# command line utilities
brew install bat
brew install tree
brew install wget
brew install trash

# JS Development
brew install node
```

## Code editors
### Visual Studio Code

#### Installation
```
brew cask install visual-studio-code
```

#### Extensions
* **Settings Sync.** Keep synced all your extensions and setting in all the machines where you use visual studio code.
* **Intellij IDEA keybindings** Since I use intellij a lot this extension allows me to use the shortcuts I am already used to.
* **CodeSnap** Useful to take screenshots of pieces of our code that we can share as an image.
* **Prettier** Code formatter.
* **Bracket Pair Colorizer** Highlights brackets with colors.

#### Themes
* Dracula
* Monokai Pro 


## Build tools
### Gradle

```
brew install gradle
```

