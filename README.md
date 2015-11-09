Go IDE in a Container
=========================

This is an example container that packages zsh, tmux, tmuxinator, vim, and Go-related plugins in a single container.
This example assumes you know how to run Docker.

This is not an official Google product.

Running the Container
---------------------
To run this container:

    $ docker run -ti charneykaye/go-ide 
    
Mount a volume so you don't lose your work:

    $ docker run -v /some/path:/go/src -ti charneykaye/go-ide

Or, mount a volume from a named container.

Building the Container
----------------------
Nothing special if you already have Docker installed:

    $ git clone https://github.com/charneykaye/go-ide-container
    $ cd go-ide-container
    $ docker build -t go-ide-container .

