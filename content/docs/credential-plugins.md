---
title: Credential Plugins
prev: /docs
---

Credential plugins can be used to add authentication protocols not natively supported by the Kubernetes client. To use a credential plugin, you must install its binary and place it in your `PATH`.

### Flatpak

The Flatpak has limited access to your system, it can only access files in your home directory. Credential plugins must therefore be placed in a home path such as `~/.local/bin`. Alternatively, you can use [Flatseal](https://flathub.org/apps/com.github.tchx84.Flatseal) to grant access to system directories.

### macOS

Your shell configuration files such as `.profile` do **not** apply to graphical applications on macOS.
To set the `PATH`, create a file in `/etc/paths.d` with the directory of your binary. You may need to restart your user session for the change to apply.
