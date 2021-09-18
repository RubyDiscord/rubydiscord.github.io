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

The guide for WSL2 will be written soon, but in the meantime plenty are
available online. After installing WSL2, follow the instructions [above](#linuxosxunix) to install Ruby.

### Editing Code in WSL2

You can use VSCode as it integrates very well with WSL2. Alternatively, you can
try out the insiders [wslg](https://github.com/microsoft/wslg) which allows you to run Linux Graphical programs straight out of WSL.
