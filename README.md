# Dotfiles for devcontainers

This repository contains dotfiles specifically used in [devcontainers](https://code.visualstudio.com/docs/remote/containers#_personalizing-with-dotfile-repositories).

Things you'll find in this dotfiles (for now):

- Aliases
- ZSH Syntax Highlighting

## Getting started

Add the following to your VS Code's `settings.json`.

```json
{
  "remote.containers.dotfiles.repository": "https://github.com/JorgenKrieger/dotfiles_devcontainers.git",
  "remote.containers.dotfiles.installCommand": "~/dotfiles/install.sh",
  "remote.containers.dotfiles.targetPath": "~/dotfiles",
}
```

## Not working as expected?

Dotfiles are installed while creating the container. Any devcontainer project already build needs to be rebuild.
To rebuild the container press <kbd>⌘ cmd/alt</kbd> + <kbd>⇧ shift</kbd> + <kbd>P</kbd>. Next, search for **Remote-containers: Rebuild and Reopen in Container**.