##First, ensure you have your Fedora install up to date:

`sudo yum update`

##Next, let's install the prerequisites we will need:

`sudo yum install git-core curl make bzip2 gcc-c++ patch readline readline-devel zlib zlib-devel libyaml-devel libffi-devel libxslt-devel sqlite sqlite-devel openssl openssl-devel`

##We are now ready to install RVM:

`bash -s stable < <(curl -s https://raw.github.com/wayneeseguin/rvm/master/binscripts/rvm-installer)`

###...followed by,

`echo '[[ -s "$HOME/.rvm/scripts/rvm" ]] && . "$HOME/.rvm/scripts/rvm" # Load RVM function' >> ~/.bashrc`

##Finally, reload your .bashrc file with the following command:

`. .bashrc`

##Ensure that RVM is loaded with the following command, which should output "rvm is a function":

 `rvm | head -1`

##The following steps will install Ruby, Rails and the devise gem. Execute these in order:
###first,

`rvm install 2.2.0`

###then...

`rvm use 2.2.0 --default`

###followed by...

`gem install bundler`

`gem install rails`

`gem install devise`

`rails new test_app`


##The last step will create a sample rails application with all the required dependencies, it is very important.

###Now install heroku

 `wget -qO- https://toolbelt.heroku.com/install.sh | sh`


##Please follow this to install postgresql

http://www.postgresonline.com/journal/archives/329-An-almost-idiots-guide-to-install-PostgreSQL-9.3,-PostGIS-2.1-and-pgRouting-with-Yum.html

`gem install pg`

`sudo yum install nodejs npm`

