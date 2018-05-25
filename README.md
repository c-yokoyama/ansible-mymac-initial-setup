# mac-localsetup-ansible]

Initial setup for my mac with Ansible.

## Get Started

```
ansible-playbook -i hosts mymac.yml

# if executing specific role
ansible-playbook -i hosts mymac.yml --tags "dotfiles"
```
