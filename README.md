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
    $ mr bundleupdate

This will delete your local copies of any repos that have been deleted from the
bundle before updating the remainging repos (and cloning any newly added
repos). If you do not want removed repos to be deleted automatically, you can
use

    $ mr update

instead. **Note** that the addition of the custom `bundleupdate` command means
that you will have to configure myrepos to trust the vim bundle `.mrconfig`
file. You can do that by adding `~/.vim/bundle/.mrconfig` to your `~/.mrtrust`
file:

    $ echo "~/.vim/bundle/.mrconfig" >> ~/.mrtrust

## License

Copyright 2019 Heinrich Kruger. Distributed under the [MIT licence](LICENCE).
