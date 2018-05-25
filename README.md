# mac-localsetup-ansible

Initial setup for my mac with Ansible.

## Get Started

Before Cloning this repository.

```
sudo xcodebuild -license
xcode-select --install

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew doctor
brew update

brew install ansible python git
```

Clone this repo.

```
ansible-playbook -i hosts mymac.yml

# if executing specific role
ansible-playbook -i hosts mymac.yml --tags "dotfiles"
```
