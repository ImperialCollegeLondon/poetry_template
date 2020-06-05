# SPARTA Control

*Note: The final application will be a standalone pice of software. The
 instructions below are just for development.*

## Installation instructions

- Requirements: [Python (we will use version 3.8)](https://www.python.org
/) and Git. The latter is usually already available in MacOS and Linux
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

The last command will create a virtual environment with all the required
 dependencies for SPARTA Control. At this point, SPARTA Control is ready for
  you to work on it. 
  
## Using SPARTA Control

If you have the virtual environment activated (you can activate it by running
 `poetry shell`), just execute in the terminal - or PowerShell in windows:

```bash
python -m sparta_control
```

At the moment, the only thing this does is printing the version information. 

If you don't have the environment activated you can run:

```bash
poetry run python -m sparta_control
```

## Testing SPARTA Control

Tests can be run in a similar way, depending on whether the environment is
 activated or not. In the first case, it is enough to run:
 
```bash
pytest
```

Otherwise, the following will do:

```bash
poetry run pytest
```