# puppet_vim

#### Table of Contents

1. [Description](#description)
1. [Setup - The basics of getting started with puppet_vim](#setup)
    * [What puppet_vim affects](#what-puppet_vim-affects)

## Description

This module is designed to work on NIX based systems to ensure that vim-enhanced is installed ans the correct syntax and indenting files have been added for vim to play nicely with vim.

This has been tested on Ubuntu 14.04, CentOS 6.7 and CentOS 7.2. The module will
add syntax and indenting files for vim to their system locations represented by the default $VIM. In CentOS this is **/usr/share/vim/vim74** and in Ubuntu this is **/etc/vim**. The system vimrc is updated with the origianl and additons in CentOS as the **/etc/vimrc** file where as with Ubuntu we can just add the additons to **/etc/vim/vimrc.local**.

The module will also intall **vim** on Ununtu and **vim-enhanced** on CentOS. Make sure you use the command vim on CentOS and not vi.

### What puppet_vim affects 

On Red hat based system the /etc/vimrc file is replaced, on Debian based systems this is the /etc/vim/vimrc.local

