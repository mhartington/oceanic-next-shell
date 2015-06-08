A shell script to change your shell's default ANSI colors but most importantly, colors 17 to 21 of your shell's 256 colorspace (if supported by your terminal). This script makes it possible honor the original bright colors of your shell (e.g. bright green is still green and so on) whilst providing the additional colors to applications such as Vim.

Ported over from the original [base16-shell](https://github.com/chriskempson/base16-shell)

![Base16 Shell](https://raw.github.com/chriskempson/base16-shell/master/base16-shell.png)

## Use Cases
* You want to use a `*.256.*` variant of a Terminal theme designed to honor the original bright colors.
* You prefer to use a script instead of a terminal emulator theme to color your shell.
* You use this script to have different colorschemes appear on different SSH sessions.

## Installation

    git clone https://github.com/mhartington/oceanic-next-shell.git ~/.config/oceanic-next-shell

## Shells

### Bash/ZSH
In `~/.bashrc` or `~/.zshrc` place the following lines:

    # Base16 Shell
    BASE16_SHELL="$HOME/.config/oceanic-next-shell/oceanic-next.dark.sh"
    [[ -s $BASE16_SHELL ]] && source $BASE16_SHELL

### Fish
In `config.fish` place the following lines:

    # Base16 Shell
    eval sh $HOME/.config/oceanic-next-shell/oceanic-next.dark.sh 

