## Welcome User!
I will be showing you how to setup a good looking terminal that will make all your friends jealous of you :3

At the end your terminal should look like this:
![](http://i.imgur.com/thSR7hI.png)

## 1. Install Tilix:
    $ sudo apt install tilix

## 2. Install ZSH:
    $ sudo apt install zsh

## 3. Install Oh-My-Zsh:
    $ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
> Note: This will set the default shell to ZSH (You will no longer be on Bash anymore.)

## 4. Install the PowerLevel9k Theme for our Oh-My-Zsh:
    $ git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k

## 5. Edit '.zshrc':
    $ vim ~/.zshrc
> replace `vim` with the editor of your predilection. (e.g. gedit, kWrite, etc., etc.)

##### Replace :

#### `ZSH_THEME="robbyrussell"`
##### With: 
#### `ZSH_THEME="powerlevel9k/powerlevel9k"`

Restart your terminal and it should look a little better now.

## 6. Download & Install any Nerd Font from here:
[https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts)
> I used Hack Regular Complete font for my example, but you can use any font flavor that you'd like.

## 7. Configure your Terminal to use our newly added Font!
> Note: Just follow the images, they are in order!

[https://imgur.com/a/o42f3Z6](https://imgur.com/a/o42f3Z6)

## 8. Configure '.zshrc' once more:
Now, add this below the theme line that we edited a while ago.

    ...
    POWERLEVEL9K_MODE="nerdfont-complete"

    POWERLEVEL9K_DISABLE_PROMPT=true
    POWERLEVEL9K_PROMPT_ON_NEWLINE=true
    POWERLEVEL9K_MULTILINE_LAST_PROMPT_PREFIX="▶ "
    POWERLEVEL9K_MULTILINE_FIRST_PROMPT_PREFIX=""

    POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(custom_user_icon dir vcs)

    POWERLEVEL9K_CUSTOM_USER_ICON="echo "
    POWERLEVEL9K_CUSTOM_USER_ICON_BACKGROUND=069
    POWERLEVEL9K_CUSTOM_USER_ICON_FOREGROUND=015
    ...

to edit your unicode symbol in `POWERLEVEL9K_CUSTOM_USER_ICON`, you must select one from here: 

> [Online CharacterMap](https://bluejamesbond.github.io/CharacterMap)

Once you open the website up, select the Hack Nerd Complete font, that you downloaded and installed from a couple of steps ago. (it must be the actual `*.ttf` file, and it should be in `/usr/local/share/fonts/h/` or just search it where your fonts installation directory is.)

Once you load up the font in the website, go to `2800 -> 2999`, there it will show all the unicode glyphs you can use in that line.

example:

![](http://i.imgur.com/4H5l15U.png)


___

We're done!

Enjoy and have fun with your new terminal!

___

###### Credits: baby WOGUE /w https://www.youtube.com/watch?v=wM1uNqj71Ko
