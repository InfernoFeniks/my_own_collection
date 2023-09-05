# Ansible Role: my_module_file_create
[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)

## Description

Easy creation of a file with content

## Requirements

- Ansible >= 2.18 (It might work on previous versions, but we cannot guarantee it)
- Debian and python on deployer machine.
- Python >=3.10

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `path` | ./my_file.txt | file path and name |
| `content`| Hello from InfernoFeniks (test content) | Default content |


## Example

### Playbook

```yaml
- name: Module testing
  hosts: localhost
  tasks:

  - name: Create file with context
    my_own_module:
      path: './feniks_playbook.txt'
      content: "This file create by playbook"
```

## License

This project is licensed under MIT License. See [LICENSE](/LICENSE) for more details.


## Author Information

Role by `InfernoFeniks`.