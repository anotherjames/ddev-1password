[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/anotherjames/ddev-1password/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/anotherjames/ddev-1password/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/anotherjames/ddev-1password)](https://github.com/anotherjames/ddev-1password/commits)
[![release](https://img.shields.io/github/v/release/anotherjames/ddev-1password)](https://github.com/anotherjames/ddev-1password/releases/latest)

# DDEV 1password

## Overview

This add-on integrates 1password into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get anotherjames/ddev-1password
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for 1password |
| `ddev logs -s 1password` | Check 1password logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.1password --1password-docker-image="busybox:stable"
ddev add-on get anotherjames/ddev-1password
ddev restart
```

Make sure to commit the `.ddev/.env.1password` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `1PASSWORD_DOCKER_IMAGE` | `--1password-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@anotherjames](https://github.com/anotherjames)**
