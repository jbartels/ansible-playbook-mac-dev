# Ansible playbook for Mac setup and configuration

This is playbook to install and configure software on a Macbook used for devops and cloud development.

![Build status](https://travis-ci.org/bmacauley/ansible-playbook-mac-dev.svg?branch=master)

It is continually evolving and leans heavily on the following examples on Github:

* [geerlingguy/mac-dev-playbook](https://github.com/geerlingguy/mac-dev-playbook)
* [BattleSchool](http://spencer.gibb.us/blog/2014/02/03/introducing-battleschool)
* [osxc](https://github.com/osxc)
* [MWGriffin/ansible-playbooks](https://github.com/MWGriffin/ansible-playbooks)

##Installation

Run the installer script...

```shell
curl -fsSL https://raw.githubusercontent.com/bmacauley/ansible-playbook-mac-dev/master/install | bash
```

The installer script installs Apple's command line tools , Homebrew, Python Pip, Ansible and finally it downloads and runs this playbook


Alternatively...

1. Install Apple's command line tools, if they are not installed (`xcode-select --install`)
2. Install [Homebrew](http://brew.sh/)
3. Install [Ansible](http://docs.ansible.com/ansible/intro_installation.html)
4. Clone this playbook to your Macbook
5. Run $ ansible-galaxy install -r requirements.yml inside this directory to install required Ansible roles
6. Run ansible-playbook main.yml -i inventory -K inside this directory. Enter your account password when prompted.


## Defaults

Not everyone's development environment and preferred software configuration is the same.
You can override any of the defaults configured in default.config.yml by creating a config.yml file and setting the overrides in that file. For example, you can customize the installed packages and apps with something like:




## Included Applications

Applications (Homebrew Casks):




Packages(Homebrew):


## 


