Installing this vimrc manually
==============================
Although a vimrc is a very personal thing, you may use mine if you
like it.  To do so, please do the following:

1. Clone this repo::

   	git clone git://github.com/gchou/vimrc.git

2. In your ~/.vimrc, add the following line::

   	source ~/path/to/vimrc/vimrc

3. Create a symbolic link from ~/.vim to vimrc/vim::

   	cd ~
   	ln -s ~/path/to/vimrc/vim .vim

4. Fetch submodules::

   	git submodule init
   	git submodule update

5. Recompile Command-T Ruby C extension for your platform::

   	cd vim/bundle/commandt
   	rake make

6. Touch::

   	touch ~/.vim/user.vim

That's it.


Updating submodules.
==============================
Run the following command to get the latest update for submodules.::
   	git submodule foreach git pull
