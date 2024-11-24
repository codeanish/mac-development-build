# mac-development-build
Ansible scripts to build/configure a new Mac for development


## Installation steps

1. Ensure xcode command line utils are installed `xcode-select -v`. If it's not installed, install it (`xcode-select --install`)
2. Install Ansible using pip - You should already have a version of pip installed on the new mac, this is the one time we'll be using the system configured python/pip
    1. Ensure python is on your path. You can find the default installation of Python in Mac OS at `/Users/{YOUR_USERNAME}/Library/Python/{PYTHON_VERSION}` add the path to python to your PATH variable.
    > export PATH=$HOME/Library/Python/{PYTHON_VERSION}/bin:$PATH
3. Install homebrew
    > /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
4. Configure the defaults in this project to ensure that the Mac setup is to your liking (They can be found in the main.yaml files in the defaults directory for each role)
5. From the root directory of this repository, run the playbook:
    > ansible-playbook main.yaml

Wallpapers:

https://github.com/dharmx/walls/blob/main/apocalypse/kanistra-studio-8-unicorn.jpg

Install Oh my ZSH
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

## To Do:

* Install Oh My ZSH 
  > sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
* Configure Kitty Config
* Install & Configure Neovim (just install nvchad for now https://nvchad.com/docs/quickstart/install)