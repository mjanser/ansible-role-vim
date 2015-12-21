# Ansible Role: vim

An Ansible role that installs and configures vim on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    vim_plugins:
      - "tpope/vim-surround"
    vim_users:
      - vagrant

## Dependencies

None

## Example Playbook

    - hosts: all
      roles:
        - { role: mjanser.vim }

## License

MIT
