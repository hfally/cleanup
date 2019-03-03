<p align="center">
    <strong>
        CLEANUP - LINUX & UNIX
    </strong>
</p>

<p align="center">
    <img alt="MIT" src="https://img.shields.io/badge/license-MIT-green.svg">
    <img alt="multi-convert" src="https://img.shields.io/badge/Image-Active-green.svg">
</p>


## Introduction
We all are victims of messy folders, containing lots of file types, ranging from music files to pictures, web-files, etc. A perfect example of such is our Downloads folder.

This tool was built for me and you to help us `cleanup` such folder with just a single command from the terminal.

By `cleanup`, it doesn't delete your files : ).

- This tool creates a folder called **CLEANUP** in the directory it is being ran.
- After this, it creates group folders (eg. Documents, Music, etc)
inside the newly created **CLEANUP** folder.
- Finally, it moves your files using their extensions to group them into
the best-suiting new folder.

After these, you decide what to do with the grouped folders!

## Installation
Go to your home directory on your terminal:

`$ cd ~`

Clone `cleanup` into your home directory:

`$ git clone https://github.com/hfally/cleanup.git`

Add `$HOME/cleanup/bin` to your PATH.

#### How to add to your PATH
Run the command below. There is 70% chances you are using the default bash terminal, but if you happen to be using
another terminal like `zsh` switch `.baschrc` for `.zshrc` in the commands below.

`$ echo 'export PATH="$PATH:$HOME/cleanup/bin"' >> .bashrc`

You will need to source your .bashrc or logout/login (or restart the terminal) for the updates to take effect. 
To source your .bashrc, simply run:

`$ source ~/.bashrc`

**if you use zsh or any other shell, follow the same route (replace .bashrc with .zshrc in the commands above as stated previously)**

## Basic Usage
* Go to the folder you want to cleanup from the terminal

    `$ cd /path-to-files/` 
    
    ***REPLACE** `path-to-files` with the correct path to those files, e.g Downloads*

* To confirm if `cleanup` is properly installed, run:

    `$ cleanup help`
    
    If this returns how to use the tool, then you're good to go, else, go through this manual again.

* Run the command below to do the cleanup

    `$ cleanup start`

Watch your folder get cleaned up.

That's it! 

You can always get help through `$ cleanup help`

## Undo/Revert
To undo/revert cleanup, run:

   `$ cleanup undo`

## Update
To pull latest updates, go into the `cleanup` directory: if you followed the above instructions, run:

`$ cd ~/cleanup`

then run:

`$ git pull`
    
## Supported OS
- Linux
- UNIX
- windows (using git bash): this hasn't been fully tested

## License

Cleanup is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)

## Contribution
For contribution and personal bug reporting, send a mail to the author <a href='mailto:tofex4eva@yahoo.com'>hello@henryfalade.me</a>
