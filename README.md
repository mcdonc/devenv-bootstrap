# devenv-bootstrap

Install [Nix](https://nixos.org/), [devenv](https://devenv.sh/), and [cachix](https://cachix.org/) in one command.

## Quick Install

```bash
curl -sSf https://raw.githubusercontent.com/mcdonc/devenv-bootstrap/main/bootstrap.py | python3 - --unattended
```

## Interactive Install

```bash
curl -sSf https://raw.githubusercontent.com/mcdonc/devenv-bootstrap/main/bootstrap.py | python3
```

## Options

```
--unattended       Don't ask questions
--uninstall        Uninstall Nix and devenv
--devenv-version   devenv version to install (default: v2.1.2)
--cachix-version   cachix version to install (default: v1.10.0)
```

## What It Does

1. Installs Nix via the [Determinate Systems installer](https://install.determinate.systems/nix)
2. Installs devenv from the cachix/devenv flake
3. Installs cachix CLI
4. Configures trusted users for Nix
