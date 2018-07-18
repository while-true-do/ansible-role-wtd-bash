[![Build Status](https://travis-ci.org/while-true-do/ansible-role-wtd-bash.svg?branch=master)](https://travis-ci.org/while-true-do/ansible-role-wtd-bash)

# Ansible Role: wtd-bash
| A role to deploy the bash customizations from wtd

The following customizations will be deployed:

- [Prompt](https://github.com/while-true-do/bash-prompt)
- [Behaviour](https://github.com/while-true-do/bash-behaviour).

## Motivation

Deploying customizations for bash is a regular task. To have the same look and feel on all hosts, this role can be used. It is deploying and updating the customizations.

## Installation

Install from [Ansible Galaxy](https://galaxy.ansible.com/while_true_do/wtd-bash)

```
ansible-galaxy install while_true_do.wtd-bash
```

Install from [Github](https://github.com/while-true-do/ansible-role-wtd-bash)

```
git clone https://github.com/while-true-do/ansible-role-wtd-bash.git while_true_do.wtd-bash
```

## Requirements

**Used Modules**

- [file_module](http://docs.ansible.com/ansible/latest/git_module.html)
- [git_module](http://docs.ansible.com/ansible/latest/file_module.html)


**on host that executes the role**

-   git>=1.7.1 (the command line tool)

## Dependencies

None.

## Role Variables

```yaml
# defaults/main.yml
---
wtd_bash_deploy_directory: '~/.while-true-do'
# https://github.com/while-true-do/bash-prompt
wtd_bash_prompt: 'true'
# https://github.com/while-true-do/bash-behaviour
wtd_bash_behaviour: 'true'
```

## Example Playbook

Simple Example:

```yaml
- hosts: servers
  roles:
    - { role: while_true_do.wtd-bash }
```
## Testing

This role is currently tested with syntax-checking and linting.
You can find the tests in [./tests](./tests/).

## Contribute / Bugs

Thank you so much for considering to contribute. Every contribution helps us. We are really happy, when somebody is joining the hard work. Please have a look at the links first.

-   [Code of Conduct](./docs/CODE_OF_CONDUCT.md)
-   [Contribution Guidelines](./docs/CONTRIBUTING.md)
-   [Create an issue or Request](https://github.com/while-true-do/ansible-role-user/issues)
-   [See who was contributing already](https://github.com/while-true-do/ansible-role-user/graphs/contributors)

## License

This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Author Information

Site: [while-true-do.org](https://while-true-do.org)

Mail: [hello@while-true-do.org](mailto:hello@while-true-do.org)
