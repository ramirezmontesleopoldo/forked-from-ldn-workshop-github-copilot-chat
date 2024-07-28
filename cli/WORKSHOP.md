﻿# Copilot CLI

Remember to **DISCONNECT VPN**.

## Setup

```shell
unset GITHUB_TOKEN
gh auth login

bash .devcontainer/scripts/init.sh

gh copilot --version
gh copilot
```

## Suggest comands

```shell
gh copilot suggest "grep for # in md files"
@terminal grep for # in md files

gh copilot suggest "remove all files with pyc and pyo extension"
@terminal remove all files with pyc and pyo extension

gh copilot suggest "list free memory in GiB and list file system utilization"
@terminal "list free memory in GiB and list file system utilization"

gh copilot suggest "make POST request with JSON body"
@terminal "make POST request with JSON body"

gh copilot suggest "Rename all folders in the current directory to lower case"
@terminal Rename all folders in the current directory to lowercase

gh copilot suggest "Install rename package in ubuntu"
@terminal Install rename package in ubuntu

gh copilot suggest "GET weather in CPH now"
@terminal GET weather in CPH now
```

## Explain commands

``` shell
gh copilot explain 'find . -name "__pycache__" -type d -exec rm -rf {} +'
@terminal explain find . -name "__pycache__" -type d -exec rm -rf {} +
@workspace /explain find . -name "__pycache__" -type d -exec rm -rf {} +

gh copilot explain "docker run -d --name flask-app -p 80:8080 --rm flask-mini"
@terminal explain docker run -d --name flask-app -p 80:8080 --rm flask-mini
@workspace /explain docker run -d --name flask-app -p 80:8080 --rm flask-mini

gh copilot explain "kubectl autoscale deployment api-backend --cpu-percent 80 --min 3 --max 6"
@terminal explain kubectl autoscale deployment api-backend --cpu-percent 80 --min 3 --max 6
@workspace /explain kubectl autoscale deployment api-backend --cpu-percent 80 --min 3 --max 6

gh copilot explain "tmux new-session \; split-window -v -p 55 \; split-window -v -p 55 \; select-pane -U\; split-window -h \; select-pane -U \;"
@terminal explain tmux new-session \; split-window -v -p 55 \; split-window -v -p 55 \; select-pane -U\; split-window -h \; select-pane -U \;
@workspace /explain tmux new-session \; split-window -v -p 55 \; split-window -v -p 55 \; select-pane -U\; split-window -h \; select-pane -U \;
```

## Questions

```shell
@terminal How to grep markdown code block in terminal?
@terminal How to grep markdown code block in terminal using pcregrep?
```
