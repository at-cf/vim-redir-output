# vim-redir-output

> Redirect the output of a vim or external command into a scratch buffer

## About

Adapted from a snippet I found online (cannot find original source). Prefix a vim or external command with `Redir` to pipe the command output into a scratch buffer.

## Install

Use your plugin manager of choice, e.g. [vim-plug](https://github.com/junegunn/vim-plug)

```vim
Plug 'https://github.com/at-cf/vim-redir-output.git'
```

## Use

Exposes `:RedirT`, `:RedirV`, and `:RedirS` commands (redirect output to new tab, vertical split, or horizonal split respectively).

```vim
" E.g. vim commands:
:RedirT messages
:RedirS echo $MYVIMRC

" E.g. external commands:
:RedirV !ls
```

