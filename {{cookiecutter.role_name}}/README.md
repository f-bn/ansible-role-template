## Ansible role - {{ cookiecutter.role_name | title }}

### General informations

{{ cookiecutter.role_description }}.

**Table of Contents**

- [General informations](#general-informations)
- [Role variables](#role-variables)
- [Examples](#examples)
- [Install and use this role](#install-and-use-this-role)

**Supported Platforms**

This role only supports Ubuntu Server LTS platforms:

  - Ubuntu 22.04 *Jammy Jellyfish*

**Requirements**

  - None

**References**

  - None

### Role variables

| Name                              | Default                      | Description                                                      |
| :-------------------------------- | :--------------------------- | :--------------------------------------------------------------- |

### Examples

```yaml
{{ cookiecutter.role_name }}_version: '1.0.0'
```

### Install and use this role

* Install the role using the command-line :

  ```shell
  $ ansible-galaxy role install git+https://github.com/f-bn/ansible-role-{{ cookiecutter.role_name }}.git
  ```

* You can also install the role in your projects using a `requirements.yml` file and `ansible-galaxy` command-line :

  ```YAML
  $ cat requirements.yml
  ---
  roles:
    - name: {{ cookiecutter.role_name }}
      src: https://github.com/f-bn/ansible-role-{{ cookiecutter.role_name }}.git
      scm: git
      version: '1.0.0'

  $ ansible-galaxy install-f -r requirements.yml
  ```

* Once the role is installed, you can use it in your playbooks :

  ```yaml
  - name: Deploy
    hosts: <hosts>
    roles:
      - role: {{ cookiecutter.role_name }}
  ```
