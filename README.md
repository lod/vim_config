# My Vim Setup

To setup vim just run the setup.sh script.

## Requirements
 * git
 * wget
 * Linux system
 * ctags (Optional)

This script will then install all the bundles listed in the vimrc file.

NOTE: If you use vim as your default editor, make sure you update your alternatives to be something other then vim.tiny (e.g. vim.nox).

You may also want to set git to use vim:
```bash
git config --global core.editor vim
```
## Features
  * Toggle the nerdtree (filesystem) split with <f2>
    * Use '?' once in the split to get shortcuts, like 's'
  * Solarized colour theme with dark background
  * Tab is 2 spaces
  * Hack as the default font (in graphical vim like gvim, or macvim)
  * Powerline bar at the bottom gives you:
    * Git branch
    * File encoding
    * and more!
  * Toggle a class browser (tagbar) split with <f9>
    * tagbar not enabled by default as it requires ctags. Uncomment in vimrc to make it work.

### Python specific features
  * Show python docs with 'K'
  * Runs through pyflakess and pep8 on save
  * Auto fix pep8 has been mapped to <F8>
  * Python auto complete
  * Tracks trailing white spaces
  * Highlights column 80, so you can manage width properly
  * Uses vundle to manage vim plugins
  * Fugitive plugin for git
  * Jedi for auto complete
  * If tagbar is setup <f9> will open a class browser.

NOTE: Hopefully gg=G and <F8> will now be enough to fix indents and at least the simple pep8 issues in your python code.
