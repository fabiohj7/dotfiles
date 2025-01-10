# Stow dotfiles

This is my way of using GNU Stow to preserve all my dotfiles.

Given that Stow uses a naming convention I will not be able to separate Linux from Mac. So this will stay as my main mac configuration.

## Install Stow

To install stow use your favourite package manager and install it, example:

- `brew install stow`
- `pacman -S stow`
- `sudo apt install stow`

## How to use

Clone this repo to get all the dotfiles necessary.

As you can see there is a folder for each tool/plugin, this is due to stow's naming convention, this allows you to install everything as a package.

Let's say you want to get the **nvim** config file.

"cd" into the cloned repo and use:

`$ stow nvim`

Check your **.config** directory, you will find the a symlink of nvim pointing directly to the stowed directory from the repo.

### Packages

The name of the package is based on the name of the folder, each folder will then have the path of where you want each config to go to.

For example I want nvim to go to my .config directory so I will make something like this

`nvim/.config/nvim`
