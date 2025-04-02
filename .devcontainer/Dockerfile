# syntax=docker/dockerfile:1

# Comments are provided throughout this file to help you get started.
# If you need more help, visit the Dockerfile reference guide at
# https://docs.docker.com/go/dockerfile-reference/

# Want to help us make this template better? Share your feedback here: https://forms.gle/ybq9Krt8jtBL3iCk7

ARG NODE_VERSION=22
FROM node:${NODE_VERSION}-alpine as devcontainer

# Install Git using apk (Alpine package manager)
RUN apk add --no-cache git openssh

# Set the working directory inside the container (devcontainer workspaces)
WORKDIR /workspace
# Run the application as a non-root user.
USER node

# Install necessary dependencies for development
# RUN apt-get update && apt-get install -y \
#   git \
#   openssh-client  # Install SSH client

