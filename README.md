# VIM Markify

A simple, lightweight plugin for marking lines using signs for entries in
location list or quickfix lists. Location Lists are given preference over
quickfix lists.

## Change Log

### Version 1.0
* Initial release, core functionality works.

## Getting Started
### Installation

There are 2 ways to do this

1. I recommend installing <a
   href="https://github.com/tpope/vim-pathogen">pathogen.vim</a> and then
   adding a git submodule for your plugin:

   ```sh
$ cd ~/.vim
$ git submodule add git@github.com:dhruvasagar/vim-markify.git bundle/markify
   ```
2. Copy plugin/todo-mode.vim, doc/todo-mode.txt to respective ~/.vim/plugin
   and ~/.vim/doc under UNIX or vimfiles/plugin/ and vimfiles/doc under
   WINDOWS and restart VIM

### Usage
   When you have g:markify_autocmd = 1 (default), then markify is run on
   QuickFixCmdPost event and marks the lines with signs automatically.

   Markify can distinguish between errors, warnings &amp; info messages and
   uses different signs for each. By default it uses '>>' to display in the
   signcolumn, however this can be changed.

   If you don't wish to have markify work all the time, you can set
   g:markify_autocmd = 0 in your $VIMRC. You can call :Markify to process the
   current location list or quickfix list (location lists are given
   preference) and add the signs. You can call :MarkifyClear to clear the
   signs set by Markify and you can also use :MarkifyToggle to toggle the
   same.

## Contributing

### Reporting an Issue :
   - Use <a href="https://github.com/dhruvasagar/vim-markify/issues">Github
   Issue Tracker</a>

### Contributing to code :
   - Fork it.
   - Commit your changes and give your commit message some love.
   - Push to your fork on github.
   - Open a Pull Request.
