### General informations

Ansible role skeleton template to generate role project repository with Cookiecutter.

**Requirements**

  - Ansible >= 9.x
  - Cookiecutter

**References**

  - Cookiecutter: https://github.com/cookiecutter/cookiecutter

### How to bootstrap a new role project using Cookiecutter ?

First, you need to install Cookiecutter in your environment:

```shell
# Using pip package manager
$ pip3 install cookiecutter [options]
# Using brew (on MacOS)
$ brew install cookiecutter
```

Create an empty repository on your favorite Git platform, i.e with GitHub using the CLI:

```shell
$ gh repo create ansible-role-myrole [options]
```

Bootstrap a new project using Cookiecutter with the remote GitHub repository. You will be prompted to define the role name and other metadata:

```shell
$ cookiecutter gh:f-bn/ansible-role-template
  [1/6] Role name (): myrole
  [2/6] Short role description (): Ansible role to setup and configure...
  [3/6] Author name (f-bn): <enter>
  [4/6] Source code license (SPDX format)
    1 - MIT
    2 - BSD-3-Clause
    Choose from [1/2] (1): <enter>
  [5/6] Min. Ansible compatible version (8.0.0): <enter>
  [6/6] Issue tracker URL (https://github.com/f-bn/ansible-role-myrole/issues):
```

Finally, intialize a Git repository in the newly created folder by Cookiecutter and push the initial changes your repository:

```shell
$ cd myrole/
$ git init
$ git remote add origin git@github.com:f-bn/ansible-role-myrole.git
$ git push -u origin main
```
