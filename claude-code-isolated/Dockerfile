FROM mcr.microsoft.com/devcontainers/base:noble

USER vscode

# install claude code
RUN curl -fsSL https://claude.ai/install.sh | bash

# move and link claude config files for persistence in mounted volume
RUN mv /home/vscode/.claude.json /home/vscode/.claude/.claude.json && \
    ln -s /home/vscode/.claude/.claude.json /home/vscode/.claude.json

