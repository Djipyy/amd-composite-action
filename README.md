# Python VirtualEnv composite action
This is a composite action that can be used to setup a Python "virtual
environment" by providing requirements and constraints. It is then possible to run a command in it.

## Inputs
- python-version : Optional
- requirements : Optional
- constraints : Optional
- requirements-file : Optional
- constraints-file : Optional
- run : Required

The `requirements` and `constraints` inputs are lists of strings. The `requirements-file` and `constraints-file` inputs are paths to files containing the requirements and constraints. They are not exclusive, and will be concatenated. It is the user's responsibility to ensure that everything is compatible and that there are no duplicates.