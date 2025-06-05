[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/anotherjames/ddev-1password/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/anotherjames/ddev-1password/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/anotherjames/ddev-1password)](https://github.com/anotherjames/ddev-1password/commits)
[![release](https://img.shields.io/github/v/release/anotherjames/ddev-1password)](https://github.com/anotherjames/ddev-1password/releases/latest)

# DDEV 1password

## Overview

This add-on integrates 1password into your [DDEV](https://ddev.com/) project to
make it available as your SSH agent.

## Installation

```bash
ddev add-on get anotherjames/ddev-1password
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev 1password` | Set up 1password for use as the SSH agent to be used globally for every client (not just DDEV). |

## Credits

**Contributed and maintained by [@anotherjames](https://github.com/anotherjames)**
