vim-hindent
===========

Vim plugin for the Haskell formatter
[hindent](https://github.com/chrisdone/hindent). It consists of the vim file
provided by hindent, but in a format suitable for inclusion using Vundle or
NeoBundle.

![gif](https://raw.githubusercontent.com/octol/vim-hindent/master/screencast.gif)

Prerequisite
------------

A working installation of [hindent](https://github.com/chrisdone/hindent). This
means, the `hindent` binary needs to be in `$PATH`.

Installation
------------

Using NeoBundle, add
```
NeoBundle 'octol/vim-hindent'
```
to `.vimrc`.

Alternatively, to lazily load only for Haskell file types

```
NeoBundleLazy 'octol/vim-hindent', { 'autoload' : { 'filetypes' : 'haskell' }}
```

Then install by running
```
:NeoBundleInstall
```

Usage
-----
Select the code using visual mode, then run `gq`.

Configuration
-------------

The style is "fundamental" by default, configure this using the
`g:hindent_style` variable, such as
```vim
let g:hindent_style = "gibiansky"
```

Credits
-------
Most of the hard work is by [Chris Done](https://github.com/chrisdone) and the
great hindent plugin.
