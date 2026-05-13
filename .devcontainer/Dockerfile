FROM ubuntu:22.04

# Prevent interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Install essential build tools
RUN apt-get update && apt-get install -y \
    git curl wget build-essential bc bison flex libssl-dev libelf-dev pkg-config python3 python3-pip unzip lz4 zstd

# Create a workspace user
RUN useradd -m vscode
USER vscode
WORKDIR /workspaces/GKI-Custom
