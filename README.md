This template repository makes it easier to create new agents for [Upkie](https://github.com/upkie/upkie) wheeled bipeds.

## Getting started

1. Create a new repository from this template.
2. Search for the string "TODO: set project name" and update files accordingly
3. Replace ``LICENSE`` with the license of your choice (the default one is Apache-2.0)
4. Implement your agent in the ``agent`` directory.
5. Optional: customize your C++ spines in the ``spines`` directory.

## Installation

You can install and keep track of your dependencies using the Conda environment file (for instance using [Micromamba](https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html)):

```console
conda create -f environment.yaml
```

Alternatively, you can install the interface for Upkie from PyPI by ``pip install upkie`` and develop your agent in your local Python environment.

## Usage

Run your agent directly as a Python script:

```bash
$ python ./agent/agent.py
```

Use the Makefile to start a simulation using your custom Bullet spine:

```bash
$ make simulate
```

The Makefile includes other rules to cross-compile and upload your spine and agent to the robot. Run ``make help`` for a list of available rules.
