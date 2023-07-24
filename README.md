# template-py
A template for creating Python projects and packages.

## .github/workflows: TODO

## data
Folder to store any static data files.

## env
Virtual environment used to store project dependencies.
1. python3 -m venv env
2. source env/bin/activate
3. python3 -m pip install module_name
4. deactivate
"pip freeze" to list installed dependencies

## pkg_name
The directory containing the Python package code.
### \_\_init__.py
Tells Python the directory is a package. Contains code that is executed when the package is imported to define its public interface.
>   from .examplemodule import greet, add\
>   \_\_all__ = ['greet', 'add',]
### Modules
The .py files in the package directory that contain definitions and statements.

## tests: TODO

## .gitignore
Used to block commits of included directories and files.

## LICENSE
Specifies open-source license of code.

## main.py
If not exporting module to PYPI, this file is used to run module.

## pyproject.toml
Specifies project configuration and is used to pip install the package.
*   Install: pip install -e .
*   Install with extra: pip install -e .[extra_feature]

## README.md
Provides description and usage of project.

## requirements.txt
Provides dependencies and versions required to run project.
*   Install: pip install requirements.txt