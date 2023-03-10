# Nix Flake Templates

A collection of personal nix flake templates, mainly development focussed, which
I put together to save me a minute or three while writing software.

## Pre-requisites

- **Nix** (obviously) with experimental features enabled for commands and flakes
- **direnv** (optional) so each flake is applied automatically on entry to the
  project directory

## Available Templates

- csharp/dotnet - _the official SDK for .NET (previously .NET Core) development_
- javascript/js/node - _JavaScript/node environment, predominantly for building
  web apps_

## Planned Templates

- rails - _ruby on rails environment with foreman for task management and a
  customised bundix for managing gem dependencies via nix_
- ruby - _ruby environment with customised bundix for managing gem dependencies
  via nix_

## Usage

```
mkdir <project-dir>
cd <project-dir>
nix flake init -t github:arti5an/flake-templates#<template-name>
direnv allow
```
