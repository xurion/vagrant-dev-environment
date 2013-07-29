Vagrant development environment
===============================

My personal vagrant dev environment for OSX.
Acts as an easy-to-setup LAMP stack on OSX. Uses Ubuntu.

## Link

https://github.com/xurion/vagrant-dev-environment

## Installation & use

Unpack or clone the files to your Sites directory. The path should be
~/Sites/vagrant-dev-environment/

Navigate to this directory in Terminal and simply run 'vagrant up'

In your hosts file (/etc/hosts) set your localhost to 33.33.33.10.

This vagrant box will automatically set your Sites directory as localhost.

### Setting up other virtual hosts

The vagrant-dev-environment directory houses templates for virtual hosts.
Out of the box, this project will have only one vhost file called default, found
in:
~/Sites/vagrant-dev-environment/provisions/templates/etc/apache2/sites-enabled/

Any other vhost files you place here will be picked up next time you run vagrant
provision.

By default, the vagrant machine will be set on 33.33.33.10 on your network.
This allows you to assign your virtual hosts to that IP so you can run them on a
customised domain name rather than having to develop everything on localhost.