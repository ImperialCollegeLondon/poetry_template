# SPARTA Control

*Note: The final application will be a standalone pice of software. The
 instructions below are just for development.*

## Installation instructions

- Requirements: [Python (we will use version 3.8)](https://www.python.org) and Git. The latter is usually already available in MacOS and Linux
 systems or can be installed from their package managers. For Windows, you can 
 get it from [here](https://git-scm.com/).
- [Download and install Poetry](https://python-poetry.org/docs/#installation) 
following the instructions for your OS.
- Clone this repository with:

```bash
git clone https://github.com/ImperialCollegeLondon/SPARTA_control.git
```
- Enter into the `SPARTA_control` directory and run:

```bash
poetry install
```

### Virtual environment

The last command will create a virtual environment with all the required
 dependencies for SPARTA Control. However, this environment is deactivated. It
  can be activated by running in the terminal (or PowerShell):
  
```bash
poetry shell
```

At this point, SPARTA Control is ready for you to work on it. If you do not
 activate the environment, any python-related command you want to run for the
  project will need to be preceded by `poetry run`.
  
From now on, it will be assumed that the virtual environment is activated.
  
### Pre-commit

SPARTA Control uses `pre-commit` to run a few tools before every commit to
 make sure that the code follows some standards, as well as other checks. To
  enable this, run the following command in the terminal (or PowerShell):
  
```bash
pre-commit
```
  
## Using SPARTA Control

Just execute in the terminal - or PowerShell in windows:

```bash
python -m sparta_control
```

At the moment, the only thing this does is printing the version information.

## Testing SPARTA Control

Tests can be run in a similar way, being enough to run:
 
```bash
pytest
```