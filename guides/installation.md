## Installing Ruby

Ruby can be installed in many ways on many different platforms. I will try to
outline the best possible ways for each platform.


### Linux/OSX/Unix

For Unix systems, you should use a Ruby version manager. Some popular ones are:

- [rbenv](https://github.com/rbenv/rbenv)
- [RVM](https://rvm.io/)
- [chruby](https://github.com/postmodern/chruby)

A Ruby version manager is simply a tool that allows you to switch between 
multiplle installed versions of Ruby.

A key point to note is that for most of your projects, you SHOULD NOT use the
System Ruby that is installed. This is because of root user permissions which
causes a lot of issues and headache.

I would recommend either installing rbenv or chruby, as they provide the
simplest solution managing Ruby. They also come with a choice of Ruby 
installers: `ruby-install` or `ruby-build`.


## Windows

For the best experience of Ruby on Windows the solution is simple. Don't use
Windows. Instead use [WSL2](https://docs.microsoft.com/en-us/windows/wsl/about). 

WSL2 allows you to run a full Linux environment inside Windows, without any VM,
or dual booting or anything of the sort.

A fleshed out guide for installing WSL2 can be found [here](https://docs.microsoft.com/en-us/windows/wsl/install), but for users looking for the simplest guide, first check if you meet the prerequisites. Updated Windows 10 supports WSL2 out of the box and can be installed with Ubuntu as the default distribution using `wsl --install` in an elevated terminal. After setting up a user account, follow the instructions [above](#linuxosxunix) to install Ruby.

If you prefer to install Ruby on Windows without WSL, you can do so with [RubyInstaller](https://rubyinstaller.org/). The installation process is straightforwared, and the default options work well. This also would allow for more code editing options outside of VSCode but prepare to install an entire unix system. 

### Editing Code in WSL2

You can use VSCode as it integrates very well with WSL2. Alternatively, you can
try out the insiders [wslg](https://github.com/microsoft/wslg) which allows you to run Linux Graphical programs straight out of WSL.
