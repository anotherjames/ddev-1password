[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/anotherjames/ddev-1password/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/anotherjames/ddev-1password/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/anotherjames/ddev-1password)](https://github.com/anotherjames/ddev-1password/commits)
[![release](https://img.shields.io/github/v/release/anotherjames/ddev-1password)](https://github.com/anotherjames/ddev-1password/releases/latest)

# DDEV 1password

## Overview

This add-on integrates 1password into your [DDEV](https://ddev.com/) project to
make it available as your SSH agent.

> [!NOTE]
> DDEV v1.25.5 and newer explicitly support 1Password and other existing SSH
> agents, so this add-on is only needed for DDEV v1.24.3 through v1.24.5. On newer
> versions, run:
>
> ```bash
> ddev config global --ssh-agent-upstream=host
> ddev auth ssh
> ```
>
> See [Using an Existing SSH Agent](https://docs.ddev.com/en/latest/users/usage/cli/#using-an-existing-ssh-agent)
> in the DDEV docs, especially
> [macOS: which agent do my containers get?](https://docs.ddev.com/en/latest/users/usage/cli/#macos-which-agent-do-my-containers-get)

## Installation

```bash
ddev add-on get anotherjames/ddev-1password
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev 1password` | Set up 1password for use on macs as the SSH agent to be used globally for every client (not just DDEV). |

## Credits

- Inspired by [@darthsteven's work](https://github.com/ddev/ddev/issues/3878#issuecomment-2491614576)**
- Contributed and maintained by [@anotherjames](https://github.com/anotherjames)**
