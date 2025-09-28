# Claude Code Devcontainer

A minimal [development container](https://code.visualstudio.com/docs/devcontainers/containers) setup for [Claude Code](https://claude.com/product/claude-code) with two options for managing your Claude API credentials:

1. **Host Credentials**: This option allows you to use your existing Claude API credentials stored on your host machine. It mounts your host's `~/.claude`, `~/.claude.json`, and `~/.claude.json.backup` files into the container, making it easy to manage your credentials without duplicating them.

2. **Container Credentials**: This option allows you to provide your Claude API credentials directly within the container. Using a named Docker volume instead of mounting host files, the credentials persist across Dev Container rebuilds until you remove the volume.

## Usage

Copy the desired directory (`host-credentials` or `credentials-per-devcontainer`) to `.devcontainer` in your project, then open the project in a Dev Container.
