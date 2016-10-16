# Ansible Role: wtd-bash
| A role to deploy the bash customizations from wtd - [Prompt](https://github.com/while-true-do/bash-prompt) and [Behaviour](https://github.com/while-true-do/bash-behaviour).

## Installation

Galaxy Link: <https://galaxy.ansible.com/while-true-do/wtd-bash>

```
ansible-galaxy install while-true-do.wtd-bash
```

Github Link: <https://github.com/while-true-do/ansible-role-wtd-bash>

```
git clone https://github.com/while-true-do/ansible-role-wtd-bash while-true-do.wtd-bash
```

## Requirements

git must be installed on the target host. This can be done with this role, too.

## Dependencies

None.

## Role Variables

```
# defaults/main.yml
bash_install_git: 'false'

wtd_deploy_directory: '~/.while-true-do'

# https://github.com/while-true-do/bash-prompt
bash_wtd_bash_prompt: 'true'
# https://github.com/while-true-do/bash-behaviour
bash_wtd_bash_behaviour: 'true'
```

## Example Playbook

Simple Example:

```
- hosts: servers
  roles:
    - { role: while-true-do.wtd-bash }
```

## License

This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Contribute / Bugs

**bug reports:** <https://github.com/while-true-do/ansible-role-wtd-bash/issues>

**contributers:** <https://github.com/while-true-do/ansible-role-wtd-bash/graphs/contributors>

## Author Information

**blog:** <https://blog.while-true-do.org>

**github:** <https://github.com/daniel-wtd>

**contact:** [mail@while-true-do.org](mailto:mail@while-true-do.org)
