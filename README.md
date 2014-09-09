# ohai .vim

My Vim files. Please mind the dust.

## Installation

This is mainly a Mac install. I haven't tested it on any flavors of Linux.

First, install [Cousine](http://www.google.com/fonts#UsePlace:use/Collection:Cousine).

    $ brew install macvim --override-system-vim

At this point I check to make sure I have `+python` enabled so YouCompleteMe works.
This is easy to do via `vim --version`.

Also necessary for YouCompleteMe:
    $ brew install cmake

Then the easy part:
    $ git clone https://github.com/bergren2/dotvim.git ~/.vim
    $ cd $_
    $ ruby install.rb
    $ git clone https://github.com/gmarik/vundle.git bundle/Vundle.vim
    $ vim +PluginInstall +qall

And finally, the rest of YouCompleteMe:
    $ cd bundle/YouCompleteMe
    $ ./install.sh --clang-completer