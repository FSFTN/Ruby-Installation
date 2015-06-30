# Instructions to install dependencies for Ubuntu based distributions 
##First, ensure you have your Fedora install up to date:

`sudo apt-get update`

##Next, let's install the prerequisites we will need:

`sudo apt-get -y install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev`
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

`echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc`

`exec $SHELL`

`git clone https://github.com/sstephenson/rbenv-gem-rehash.git ~/.rbenv/plugins/rbenv-gem-rehash`

`rbenv install 2.2.2`

`rbenv global 2.2.2`

`echo "gem: --no-ri --no-rdoc" > ~/.gemrc`

## Check if its all installed
`ruby -v`

`gem -v`

If either of it doesn't return the version, there is an error. 

##followed by...

`gem install bundler`

`gem install rails`

`gem install therubyracer`

`rbenv rehash`

## Check if rails is installed correctly 

`rails -v`

#Now install heroku

 `wget -qO- https://toolbelt.heroku.com/install.sh | sh`


# Follow this to install Nodejs (Optional)

[https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-an-ubuntu-14-04-server](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-an-ubuntu-14-04-server)




# Follow this to install postgresql (Optional)

[http://www.postgresonline.com/journal/archives/329-An-almost-idiots-guide-to-install-PostgreSQL-9.3,-PostGIS-2.1-and-pgRouting-with-Yum.html](http://www.postgresonline.com/journal/archives/329-An-almost-idiots-guide-to-install-PostgreSQL-9.3,-PostGIS-2.1-and-pgRouting-with-Yum.html)

`gem install pg`
