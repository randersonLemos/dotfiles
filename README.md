# dotfiles
## VIM
> Create file ".vimrc" at $HOME and on it write and save "source ~/dotfiles/.vimrc".

> Install airline/powerline fonts from here "https://github.com/powerline/fonts".

> Do not forget to set your text editor font to the newly installed fonts.

> Attention! If Plug vim plugin manager fails to install/run, check if
> you have installed the Curl program.

## GIT-BASH
> Save the files .git-completation.bash and .git-prompt.sh at "$HOME"
> Than, to the end of the .bashrc file, add:

```
# Colors!
green="\[\033[0;32m\]"
blue="\[\033[0;34m\]"
purple="\[\033[0;35m\]"
reset="\[\033[0m\]"
white="\[\e[1;37m\]"

# Enable tab completion
source ~/.git-completion.bash

# change command prompt
source ~/.git-prompt.sh
export GIT_PS1_SHOWDIRTYSTATE=1
# '\u' adds the name of the current user to the prompt
# '\$(__git_ps1)' adds git-related stuff
# '\w' adds the name of the current directory
export PS1="$purple\u$green\$(__git_ps1)$white \w $ $reset"
```

> Attention: PS1 may be specified as ps1. Also the same for GIT_PS1_SHOWDIRTYSTATE