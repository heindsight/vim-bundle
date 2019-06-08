# Vim Bundle

This repository defines my vim plugin bundle.

To use this you will need [vim-pathogen](https://github.com/gcmt/taboo.vim/issues/22) and [myrepos](https://myrepos.branchable.com/). To bootstrap do:

    $ git clone git@github.com:heindsight/vim-bundle ~/.vim/bundle
    $ cd ~/.vim/bundle
    $ mr --force checkout

All the plugin repos are configured to use lazy checkout. This means that you have to use `mr --force checkout` to clone repos that you do not already have checked out.

To update all bundled plugins, just do

    $ cd ~/.vim/bundle
    $ mr update


## License

Copyright (c) Heinrich Kruger. Distributed under the MIT license (see LICENSE).
