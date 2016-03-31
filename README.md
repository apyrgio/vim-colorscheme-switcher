# Colorscheme Switcher

Change the color scheme from a list of color scheme names.

This a fork from the
[twe4ked/vim-colorscheme-switcher](https://github.com/twe4ked/vim-colorscheme-switcher)
repo. The main update is the introduction of a more random number generator and
the inclusion of the user's colorschemes (and not the usage of pre-defined
ones) by default.

## Keybindings

* `F8` - Next scheme
* `Shift-F8` - Previous scheme
* `Alt-F8` - Random scheme

## Commands

Set the list of color schemes used by the above (default is 'all').

* `:SetColors all` - All `$VIMRUNTIME/colors/*.vim`
* `:SetColors my` - Names built into script
* `:SetColors blue slate ron` - These schemes
* `:SetColors` - Display current scheme names
* `:SetColors now` - Set the current color scheme based on time of day

You can use the following autocommand to automatically set up your normal colorshemes.

```
autocmd VimEnter * :silent! SetColors bclear solarized jellybeans
```

