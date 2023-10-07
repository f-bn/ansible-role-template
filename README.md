### General informations

Ansible role skeleton template to generate role project repository with Cookiecutter.

**Requirements**
  - Ansible >= 8.x
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

Bootstrap a new project using Cookiecutter with the remote GitHub repository. You will be prompted for various variables to configure role name and other metadata:

```shell
$ cookiecutter gh:f-bn/ansible-role-template
```

Finally, intialize a Git repository in the newly created folder by Cookiecutter and push the initial changes:

```shell
$ git init
$ git remote add origin git@github.com:f-bn/ansible-role-myrole.git
$ git push -u origin main
```
