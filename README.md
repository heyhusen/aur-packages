# AUR Packages

A monorepo for all AUR package I maintain.

## Motivation

I use Arch Linux every day. One of the advantages of Arch Linux, of course, is the large number of application libraries it has. If I have to install an AUR package, I always prioritize packages that have built-in binaries. Since some of the apps I needed weren't available, I decided to make my own.

## How this works?

I use GitHub Actions with a scheduled workflow. This workflow will check for updates from upstream daily at 00:00 (UTC). If there is an update, the AUR package will also be updated automatically.

## Why monorepo?

At first, all AUR packages I maintain had their own GitHub repos. I rely on a GitHub Action with a scheduled workflow, which GitHub can disable for being inactive in 60 days. I will rarely touch the repo once the automation is running. Activity in the GitHub repo will depend on Dependabot updating dependencies or there is a new version from upstream. Because of this, some AUR packages will not be updated.

Therefore, I decided to create this monorepo to hold all the AUR packages I maintain. This will make the activity in the repo more intense and (hopefully) the automation will continue to work well.

## Packages

### code-minimap-bin

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/hapakaien/aur-packages/CI%20-%20code-minimap-bin?label=CI&style=flat-square)](https://github.com/hapakaien/aur-packages/actions/workflows/code-minimap-bin.yml) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wfxr/code-minimap?style=flat-square)](https://github.com/wfxr/code-minimap) [![AUR version](https://img.shields.io/aur/version/code-minimap-bin?style=flat-square)](https://aur.archlinux.org/packages/code-minimap-bin/)

A high performance code minimap render.

### docker-slim-bin

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/hapakaien/aur-packages/CI%20-%20docker-slim-bin?label=CI&style=flat-square)](https://github.com/hapakaien/aur-packages/actions/workflows/docker-slim-bin.yml) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/docker-slim/docker-slim?style=flat-square)](https://github.com/docker-slim/docker-slim) [![AUR version](https://img.shields.io/aur/version/docker-slim-bin?style=flat-square)](https://aur.archlinux.org/packages/docker-slim-bin/)

Don't change anything in your Docker container image and minify it by up to 30x (and for compiled languages even more) making it secure too!

### ncspot-bin

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/hapakaien/aur-packages/CI%20-%20ncspot-bin?label=CI&style=flat-square)](https://github.com/hapakaien/aur-packages/actions/workflows/ncspot-bin.yml) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/hrkfdn/ncspot?style=flat-square)](https://github.com/hrkfdn/ncspot) [![AUR version](https://img.shields.io/aur/version/ncspot-bin?style=flat-square)](https://aur.archlinux.org/packages/ncspot-bin/)

Cross-platform ncurses Spotify client written in Rust, inspired by ncmpc and the likes.

> ncspot depends on ncurses, which can be implemented differently in each Linux distribution. Since the official binary is built using Ubuntu, I decided to build ncspot myself on Arch Linux (via GitHub Actions).

### nonicons-font

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/hapakaien/aur-packages/CI%20-%20nonicons-font?label=CI&style=flat-square)](https://github.com/hapakaien/aur-packages/actions/workflows/nonicons-font.yml) [![AUR version](https://img.shields.io/aur/version/nonicons-font?style=flat-square)](https://aur.archlinux.org/packages/nonicons-font/)

A set of SVG icons representing programming languages, designing & development tools.

### nordic-polar-theme

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/eliverlara/nordic-polar?style=flat-square)](https://github.com/EliverLara/Nordic-Polar) [![AUR version](https://img.shields.io/aur/version/nordic-polar-theme?style=flat-square)](https://aur.archlinux.org/packages/nordic-polar-theme)

A Gtk3.20+ theme created using the awesome Nord color palette.

### plenti-bin

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/hapakaien/aur-packages/CI%20-%20plenti-bin?label=CI&style=flat-square)](https://github.com/hapakaien/aur-packages/actions/workflows/plenti-bin.yml) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/plentico/plenti?style=flat-square)](https://github.com/plentico/plenti) [![AUR version](https://img.shields.io/aur/version/plenti-bin?style=flat-square)](https://aur.archlinux.org/packages/plenti-bin/)

Static Site Generator with Go backend and Svelte frontend.

## Thanks

Big thanks to GitHub Actions, which has made it easy for me to maintain all these packages with automation.
