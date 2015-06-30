# Instructions to install dependencies for Ubuntu based distributions 
##First, ensure you have your Fedora install up to date:

`sudo apt-get update`

##Next, let's install the prerequisites we will need:

`sudo apt-get -y install curl git-core python-software-properties build-essential zlib1g-dev libssl-dev libreadline-gplv2-dev libcurl4-openssl-dev `
------------------------
# Instructions to install dependencies for Fedora/RPM based distributions
##First, ensure you have your Fedora install up to date:

`sudo yum update`

##Next, let's install the prerequisites we will need:

`sudo yum install git-core curl make bzip2 gcc-c++ patch readline readline-devel zlib zlib-devel libyaml-devel libffi-devel libxslt-devel sqlite sqlite-devel openssl openssl-devel`

-------------------------

# Instructions to install ruby using rbenv
## Fire up your terminal, and copy paste the following commands 

`git clone https://github.com/sstephenson/rbenv.git ~/.rbenv`

`echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc`

`echo 'eval "$(rbenv init -)"' >> ~/.bashrc`

Note: Zsh users please use `~/.zshrc` in place of `~/.bashrc`.

`git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build`

`source ~/.bashrc` or `source ~/.zshrc`

`rbenv install  2.1.2`

`source ~/.bashrc` or `source ~/.zshrc`

## Check if its all installed

`ruby -v`

`gem -v`

If either of it doesn't return the version, there is an error. 

###followed by...

`gem install bundler`

`gem install rails`

`gem install therubyracer`

`rbenv rehash`

## Check if rails is installed correctly 

`rails -v`

###Now install heroku

 `wget -qO- https://toolbelt.heroku.com/install.sh | sh`


##Please follow this to install postgresql

http://www.postgresonline.com/journal/archives/329-An-almost-idiots-guide-to-install-PostgreSQL-9.3,-PostGIS-2.1-and-pgRouting-with-Yum.html

`gem install pg`


