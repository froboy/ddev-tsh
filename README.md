[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/froboy/ddev-tsh/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/froboy/ddev-tsh/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/froboy/ddev-tsh)](https://github.com/froboy/ddev-tsh/commits)
[![release](https://img.shields.io/github/v/release/froboy/ddev-tsh)](https://github.com/froboy/ddev-tsh/releases/latest)

# DDEV Tsh

## Overview

This add-on integrates Tsh into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get froboy/ddev-tsh
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Tsh |
| `ddev logs -s tsh` | Check Tsh logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.tsh --tsh-docker-image="busybox:stable"
ddev add-on get froboy/ddev-tsh
ddev restart
```

Make sure to commit the `.ddev/.env.tsh` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `TSH_DOCKER_IMAGE` | `--tsh-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@froboy](https://github.com/froboy)**
