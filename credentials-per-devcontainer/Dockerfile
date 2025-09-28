FROM mcr.microsoft.com/devcontainers/base:noble

USER vscode

# install claude code
RUN curl -fsSL https://claude.ai/install.sh | bash

# move and link claude config files to mount all claude config files
RUN mv /home/vscode/.claude.json /home/vscode/.claude/settings.json && \
    mv /home/vscode/.claude.json.backup /home/vscode/.claude/settings.json.backup && \
    ln -s /home/vscode/.claude/settings.json /home/vscode/.claude.json && \
    ln -s /home/vscode/.claude/settings.json.backup /home/vscode
