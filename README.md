# How It Works

Instead of manually setting up each server, you define your entire cluster—all your controller and worker nodes—in a single YAML configuration file (k0sctl.yaml).

Then, you simply run one command: `k0sctl apply`.

The tool takes care of everything else:

• Connecting to your servers via SSH.
• Installing the k0s software.
• Configuring the nodes to form a complete, production-ready cluster.

## What You'll Need (Requirements)

To make this magic happen, you only need a few things:

### 1. On Your Local Machine (where you run the command):

• The `k0sctl` tool itself.
• An SSH client with a private key.

### 2. For Each Target Server (your future nodes):

• A supported OS (like Ubuntu, Debian, RHEL, or Windows Server).
• An SSH server that is running.
• A user account with `sudo` (or root) privileges.
• The public part of your SSH key added to that user's authorized keys for passwordless login.

## Key Takeaway

k0sctl provides an **Infrastructure as Code** approach to cluster management. It makes deploying, upgrading, and managing k0s clusters **simple, automated, and repeatable**.

[node diagram](https://github.com/Daniel-Rosales-DevOps/k0sctl-bootstrap/blob/main/node-diagram.png)
