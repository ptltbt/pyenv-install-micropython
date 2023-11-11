# pyenv-install-micropython
Pyenv plugin to install recent versions of Micropython.

## Notes
Recent versions of Micropython have different build steps than the versions supported by `pyenv`. A [PR is open](https://github.com/pyenv/pyenv/pull/2754) to introduce support for new versions, but as of November 2023 it hasn't been merged.

In order to leverage `pyenv`to build and install Micropython on Unix systems, this plugin provides a (hacky) workaround to do so without messing with `pyenv`internals.

## Usage 
* Clone this git repo into `.pyenv/plugins/`
* Execute the patched ìnstall command, adding the path to the Micropython definition as an argument

Example
```bash
pyenv installmp ~/.pyenv/plugins/pyenv-install-micropython/definitions/micropython-1.21.0
```
