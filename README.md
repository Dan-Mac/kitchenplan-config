# Kitchenplan Configuration

This is a Kitchenplan configuration repository. This repository contains all configuration to install and configure our OSX workstations. More information about Kitchenplan and on how to use it can be found in the [Kitchenplan README](https://github.com/kitchenplan/kitchenplan).

## OSX Installation instructions

1. Install Xcode
2. Install rbenv
  * `git clone https://github.com/sstephenson/rbenv.git ~/.rbenv`
  * `echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile`
  * `echo 'eval "$(rbenv init -)"' >> ~/.bash_profile`
  * restart shell
  * check by executing `type rbenv` - you should see `rbenv is a function`
3. Install ruby-build
  * `git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build`
4. Instll ruby version
  * `rbenv install -l` (lists available versions)
  * `rbenv install *<version>*`
5. Install kitchenplan
  * `rbenv shell *<version>*`
  * `gem install kitchenplan`
  * open new terminal
  * `rbenv shell *<version>*`
  * `kitchenplan setup`
  * answer Y to "Do you have a config repository"
  * `https://github.com/Dan-Mac/kitchenplan-config.git`
  * `kitchenplan provision` (if you get a sudo error when installing java, re-run this command)

This should install all applications listed in my config files.
