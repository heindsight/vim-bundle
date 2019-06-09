# Vim Bundle

This repository defines my vim plugin bundle.

To use this you will need [myrepos](https://myrepos.branchable.com/). To
bootstrap do:

    $ mr bootstrap https://raw.githubusercontent.com/heindsight/vim-bundle/master/.mrconfig ~/.vim/bundle/

You also need to configure [pathogen.vim](https://github.com/tpope/vim-pathogen)
to load the plugins (pathogen.vim is included in the bundle). The following
should be added to your `~/.vimrc` file:

    runtime bundle/vim-pathogen/autoload/pathogen.vim
    execute pathogen#infect()

To update the bundle, do:

    $ cd ~/.vim/bundle
    $ mr update

## License

Copyright (c) Heinrich Kruger. Distributed under the [MIT license](LICENSE).
