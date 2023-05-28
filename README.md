# shoe-closet-backend-python
Backend for the Shoe Closet Project. Written in Python.


## Managing Dependencies Via Poetry

Poetry is a powerful dependency management tool for Python projects. It simplifies the process of managing project dependencies and provides a unified workflow for development. This section outlines how to init and activate your venv and how to add and delete dependencies using Poetry.

### Init Virtual Environment

Run `poetry init`

## PREREQUISITES: Python 3.11

### Activate Virtual Environment

Run `poetry shell` and we use `poetry shell no-dev` in production (if we get there lol)

### Deactivate Virtual Environment

Run `exit`

### Adding Dependencies

To add a new dependency to your project using Poetry, follow these steps:

1. Make sure you have Poetry installed. If not, you can install it by following the instructions at [https://python-poetry.org/docs/#installation](https://python-poetry.org/docs/#installation).

2. Activate your project's virtual environment. If you're using a virtual environment, activate it before proceeding.

3. Open a command-line interface and navigate to your project's root directory.

4. Run the following command to add a new dependency to your project: `poetry add ${package_name}` or if it is just a dev dependency run: `poetry add --group dev ${package_name}`
5. Poetry will resolve and install the package along with its dependencies.

6. Update your project's virtual environment by running: `poetry install`


### Deleting Dependencies

To remove a dependency from your project using Poetry, follow these steps:

1. Open a command-line interface and navigate to your project's root directory.

2. Run the following command to remove a dependency from your project: `poetry remove package_name`
3. Update your project's virtual environment by running: `poetry install`

## Local Development

Run `poetry shell` to start your virtual environment.

Run `poetry install` to download the dependencies.

Run `black .` to format your files at any time and `ruff .` to see issues in the code. 

`black` and `ruff` are run as a pre-commit hook. If rough returns fixes run `ruff . --fix`

