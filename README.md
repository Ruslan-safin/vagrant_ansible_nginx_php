# README #

### Vagrant Ansible Nginx PHP Draft ###

* Version 16.02.25

### How do I get set up? ###

* Install Vagrant and trusty64 box
`sudo apt-get install --assume-yes vagrant ansible`
`vagrant box add ubuntu/trusty64 https://atlas.hashicorp.com/ubuntu/boxes/trusty64`

* change current directory and run `vagrant up`

* if need change ip settings or port translation rules edit "Vagrantfile" section  "config.vm.network 
  config.vm.network "forwarded_port", guest: 80, host: 8080 "

* to configure nginx vHosts edit roles/webserver/templates/virtual-hosts.conf.j2 

* project file must be placed in "app" directory

Default project available http://127.0.0.1:8080 

### Who do I talk to? ###

* Repo owner CyberManiac