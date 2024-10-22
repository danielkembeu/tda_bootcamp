# Github commands to upload your project

## Starting from a new project

### Configuration phase

#### NOTE: This assumes that you do have already created a repository on Github

![Github: Create a new repository](https://github.com/danielkembeu/tda_bootcamp/blob/main/web3/html/gh.jpg)

1. Create a repository on [Github](https://github.com/)

`Note`: Make sure that you select the good visibility for your project (either ``private`` or ``public``)

2. Open the project you want to upload in Visual Studio Code.

3. Open your terminal at the root of the project directory and type these commands:

```bash
    git init
```

To initialize the project's configuration for github. After that,

```bash
    git remote add origin <the link to your repository>
```

`Example:` If i've created a repository called ``tda_bootcamp`` and my github username is ``danielkembeu``, i should have this link:

```bash
https://github.com/danielkembeu/tda-bootcamp.git
```

to use with git remote add origin.

Next, you have to define the main stream for the repository (The main branch, usually called ``main``):

```bash
git branch -M <the branch name>
```

### Upload phase

Next, you now have the possibility to add your project's files to the repository:

1. Add files

```bash
git add .
```

2. Commit changes

```bash
git commit -m "Any message here to describe the changes you made"
```

3. Deploy changes onto github repository.

```bash
git push -u origin <here the name of the main branch>
```

Since we defined our main branch to have the name of ``main``, we should write:

```bash
git push -u origin main
```

## Already have a project and just want to upload new changes

For this, you just have to take again the same phases of the the ``Upload phase`` seen previously...

## How to pull changes made by others on the same project ?

To do so, we just need one command:

```bash
git pull
```

`Note:` This requires you to already be a member of the repository or to have the permission to write/read to the repository.
