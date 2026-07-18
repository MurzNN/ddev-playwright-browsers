[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/MurzNN/ddev-playwright/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/MurzNN/ddev-playwright/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/MurzNN/ddev-playwright)](https://github.com/MurzNN/ddev-playwright/commits)
[![release](https://img.shields.io/github/v/release/MurzNN/ddev-playwright)](https://github.com/MurzNN/ddev-playwright/releases/latest)

# DDEV Playwright

## Overview

This add-on installs Playwright and browsers (Chromium, Firefox, WebKit) to launch Playwright tests directly in the
[DDEV](https://ddev.com/) container with GUI forwarding to the host machine.

## Installation

```bash
ddev add-on get MurzNN/ddev-playwright
```

## Overview

Add-on downloads the latest version of Playwright and installs dependencies, required to launch browsers (Chromium,
Firefox, Webkit) during the DDEV `web` container build, to not re-configure them on each restart.

Also, it mounts a reusable host's browsers cache directory, shared with other DDEV projects, to not download a new
copy of the same browsers for each DDEV project.

Additionally, it mounts an X11 Unix socket to allow opening GUI windows on the host machine from the apps, launched
in the container.

## Credits

**Contributed and maintained by [@MurzNN](https://github.com/MurzNN)**
