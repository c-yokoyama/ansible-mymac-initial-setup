# ansible-mymac-initial-setup

Initial setup Ansible playbook for my Mac(macOS.

## Get Started

### Before executing this playbook

```
$ sudo xcodebuild -license
$ xcode-select --install

$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

$ brew doctor && brew update
$ brew install ansible python git
```

### Execute playbook

- Before executiing, register public key to github
  - https://qiita.com/shizuma/items/2b2f873a0034839e47ce

```
$ git clone git@github.com:c-yokoyama/ansible-mymac-initial-setup.git
$ ansible-playbook -i hosts playbook.yml --ask-become-pass

// if executing specific role
$ ansible-playbook -i hosts playbook.yml --tags "dotfiles" --ask-become-pass
```
