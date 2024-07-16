# First..
1. install poetry, pyenv
1. create project directory

# Folder structure
1. src(with current project, subprojects)
1. scripts
1. data, experiments(tensorboard), configs(hydra), ...

# Dealing with python version with pyenv
1. `pyenv install {preferred_version}`
1. `pyenv global {preferred_version}`

# Dependency and virtualenv control with poetry
1. `poetry init`
1. `poetry env use python` # activate virtualenv using current python version
1. `poetry shell`  # activate virtualenv using poetry
1. `poetry install` # install dependencies + current project (as editable package, so that modules in src/ can be cross-imported or imported in scripts/)

# submodules
1. Basically, there are two ways to add submodules. 
    1. `git submodule add {url} {external/submodule1}` and make symlink using `ln -s {/path/to/external/submodule1} {/path/to/src/submodule1}`
    1. `git submodule add {url} {src/submodule2}` if python files(and __init__.py) are exposed in the main directory

# debug
You can easily debug your code (using script or module directly) in vscode since we installed this package.

# github setting
1. create repo in github
1. follow the instruction in README.md




