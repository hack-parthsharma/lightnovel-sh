# lightnovel.sh

A terminal-based lightnovel reader written in Bash. It scrapes [freewebnovel](https://freewebnovel.com/).

![preview](https://user-images.githubusercontent.com/75286649/174728555-0d3b288d-4aba-473a-9779-e2d7d925eb90.gif)

## Table of Contents

* [Features](#features)
* [Installation](#installation)
  * [Arch Linux](#arch-linux)
  * [Linux](#linux)
* [Usage](#usage)

## Features

- Read daily updated english translated novels, retrieved from [freewebnovel's](https://freewebnovel.com/) extensive library.
- Focused on simplicity, minimalism and usability.
- Written in Bash, with minimal dependencies and easily tweakable.
- Stores your 20 most recently read novels[^1] to continue reading where you left off.
- It uses the `less` pager by default, which can be changed by setting the `PAGER` environment variable.

[^1]: This can be easily changed by editing the `HISTORY_LENGHT` variable on the script.

## Installation

### Arch Linux

```sh
yay -S lightnovel.sh-git
```

### Linux

#### Dependencies

Make sure you have these installed

```text
cat curl grep head less mkdir sed tput tr w3m
```

#### Installing

```sh
git clone https://github.com/hack-parthsharma/lightnovel.sh && sudo cp lightnovel.sh/lightnovel.sh /usr/local/bin/lightnovel.sh
```

#### Uninstalling

```sh
sudo rm /usr/local/bin/lightnovel.sh
```

## Usage

```text
A terminal-based lightnovel reader written in Bash.

USAGE:
  lightnovel.sh [OPTION]

OPTIONS:
  -c, --clear-cache     Clear cache
  -h, --help            Print this help page
  -l, --last-session    Restore last session
  -V, --version         Print version number
```
