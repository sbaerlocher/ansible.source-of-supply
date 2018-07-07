# Ansible Role: source-of-supply

[![Build Status](https://travis-ci.org/sbaerlocher/ansible.source-of-supply.svg?branch=master)](https://travis-ci.org/sbaerlocher/ansible.source-of-supply) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://sbaerlo.ch/licence) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-source-of-supply-blue.svg)](https://galaxy.ansible.com/sbaerlocher/source-of-supply)

## Description

Creates an order structure on the target system, in this case for support tools.

## Installation

```bash
ansible-galaxy install sbaerlocher.source_of_supply
```

## Requirements

None

## Role Variables

| Variable             | Default     | Comments (type)                                   |
| :---                 | :---        | :---                                              |
| source_of_supply_name | Support | Name of main folder. |
| source_of_supply_directorys | - "{{ source_of_supply_root }}\\{{ source_of_supply_name }}\\facts.d" | List of folders to create. |
| | - "{{ source_of_supply_root }}\\{{ source_of_supply_name }}\\startlayouts" | |

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
     - sbaerlocher.source_of_supply
```

## Changelog

### 1.0

* inital commit

## Author

* [Simon Bärlocher](https://sbaerlocher.ch)

## License

This project is under the MIT License. See the [LICENSE](https://sbaerlo.ch/licence) file for the full license text.

## Copyright

(c) 2018, Simon Bärlocher