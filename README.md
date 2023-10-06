### General informations

Ansible role skeleton template to simply generate role project repository with Cookiecutter.

**Requirements**
  - Ansible 8.x
  - Cookiecutter

### How-to bootstrap a new role project with Cookiecutter ?

First, you need to install Cookiecutter in your environment:

```console
$ pip3 install cookiecutter [options]
```

Create an empty repository on your favorite Git platform, i.e with GitHub using the CLI:

```console
$ gh repo create ansible-role-myrole [options]
```

Bootstrap a new project using Cookiecutter. You will be prompted for various variables to configure role name and metadata:

```console
$ cookiecutter https://https://github.com/f-bn/ansible-role-template.git
```

Finally, intialize a Git repository in the newly created folder by Cookiecutter and push the initial changes:

```console
$ git init
$ git remote add origin git@github.com:f-bn/ansible-role-myrole.git
$ git push -u origin main
```
