# automation

## Explanation

This project will a github bot that automatically updates the `Current List Of Ideas` section in the [README](./README.md).  It will also manage the status of other repos in files.

Example of what it can do:
`/ideas stars WalterDevelopment/ideas` would replace that line with a comment before it and the current number of stars on this repo.

For example, the commit for this project would add a new idea to the `Current List Of Ideas` section in the [README](./README.md), and other properties can be added using the 
`/ideas` command in the description for the commit.  An example commit for this idea would be:

`+ automation.md`

(Description:)

```'
/ideas title automation
/ideas description 'ideas repo manager'
/ideas assign WilWa
```

## Resources
- Python project
- A system to constantly update the info, running our python project.

## Setup
For the first time setup, we need to create a python package containing a `__init__.py` file and a `__main__.py` file. The `__main__.py` file would run _app.py_, which would be the
entrypoint to the project.  _app.py_ would run and host a github bot, accessible using `/ideas`.

To install this project to work on it, all they have to do is **_install python and enter the virtual environment_**.
