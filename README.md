# Ansible MacOS Playbook

This is the playbook to configure a MacOS build machine.

## Roles/Tasks

- Installs Homebrew packages and app casks (Role `homebrew`)
- Installs App Store apps with [`mas-cli`](https://github.com/mas-cli/mas) (Role `mas`)
- Modifies MacOS settings (Role `settings`)
- Changes the user shell, if configured (Role `shell`)

## Installation

1. Install [Homebrew](https://brew.sh).
1. Install [Ansible](http://docs.ansible.com/intro_installation.html).
1. Run `ansible-playbook main.yml`. Enter account password when prompted.
   - If you have a configuration stored elsewhere (e.g. in a dotfiles folders), run `ansible-playbook main.yml --extra-vars=@/path/to/my/config.yml`
