# Ansible Role: vim

An Ansible role that installs and configures vim on Linux.

## Requirements

None

## Role Variables

Available variables are listed below, along with default values:

    vim_custom_config_file: ~
    vim_plugins:
      - "tpope/vim-surround"
    vim_users:
      - vagrant

### Users

The role configures vim for each user defined in the variable `vim_users`.
The home directories must be under `/home/{user}`.

### Custom configuration

If you want to install a config file which contains your custom configuration, you can put the path into the variable `vim_custom_config_file`.

### Plugins

The variable `vim_plugins` can be used to install vim plugins using [Vundle](https://github.com/VundleVim/Vundle.Vim).

## Dependencies

None

## Example Playbook

    - hosts: all
      roles:
        - { role: mjanser.vim }

## License

MIT
