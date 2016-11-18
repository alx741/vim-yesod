# Vim - Yesod

Vim plugin for the Haskell [Yesod web framework](http://www.yesodweb.com/).

![Yesod](yesod_logo.png)


* Syntax for `config/models` and `config/routes`
* Jump to handler files from declared routes
* Create new handlers for routes under the cursor while in `config/routes`

**Note:** This plugin *does not* add syntax for *shakesperean templates*, there is
another plugin that does:
[vim-syntax-shakespeare](https://github.com/pbrisbin/vim-syntax-shakespeare).


## Installation

Compatible with `Vundle`, `Pathogen`, `Vim-plug`.


## Usage

*vim-yesod* gives you some predefined mappings.

For the `config/routes` file:

Map | Command | Action
--- | ------- | ------
**gh** | :YesodOpenHandler | Jump to the handler of the route under the cursor
**gH** | :YesodAddHandler | Create a new handler for the route under the cursor


## Configuration

You can disable the predefined `gH` and `gh` mappings with:

    let g:yesod_disable_maps = 1

And then add your own like:

    nnoremap <leader>H :YesodAddHandler<CR>
    nnoremap <leader>h :YesodOpenHandler<CR>


### Screenshots

`config/models` and `config/routes` files:

![Screenshot](screenshot.png)
