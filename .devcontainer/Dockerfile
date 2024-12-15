FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:0-14

# Install additional dependencies if needed
# RUN apt-get update && apt-get install -y <package-name>

# Install vscode-cli
RUN npm install -g @vscode/vscode-cli

# Set environment variables for license acceptance and token
ENV VSCODE_CLI_ACCEPT_LICENSES=true
ENV VSCODE_CLI_TOKEN=<your-token>

# Set the default user
USER vscode

# Run VS Code CLI as a server with license terms accepted
CMD ["vscode", "server", "--accept-server-license-terms"]
