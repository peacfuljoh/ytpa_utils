# ytpa-utils

## Description

This package contains utility functions used by the YouTube video predictive analytics (YTPA) system.
They support extended functionality for:
- pandas: `df_utils.py`
- gensim (text processing): `gensim_utils.py`
- data I/O: `io_utils.py`
- numpy: `np_utils.py`
- SQL: `sql_utils.py`
- timing: `time_utils.py`
- object type validation: `val_utils.py`
- other: `misc_utils.py`

## Installation

Install from PyPI with `pip install ytpa-utils`.

## Make commands

Several make commands are implemented in `Makefile`.

### Testing

Tests are implemented in the `test/` directory, one file per module. Run them locally with `make test`.

### Deploying a new package version

A new version of the package can be deployed by incrementing the version number in `pyproject.toml` and running 
`make deploy`. 
A better practice is to `git push` and allow the Github Actions pipeline to take care of running tests and deploying 
the new version only when the entire pipeline succeeds.
Make sure to use the right version of the package in your other environments (update it in a requirements file and 
update the environment).
