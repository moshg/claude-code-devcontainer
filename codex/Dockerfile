FROM mcr.microsoft.com/devcontainers/base:noble
USER vscode

# Prevent bind mounts from causing directories to be owned by root
RUN mkdir $HOME/.codex
