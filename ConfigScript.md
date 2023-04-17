install apts
-----------------------------------------------------------------------------------------------------------

#!/bin/bash

installz() {
# Update package lists
    sudo apt update

# Install Git
    sudo apt install git -y

# Install Vim
    sudo apt install vim -y

# Install Python 3
    sudo apt install python3 -y

# Install GIMP
    sudo apt install gimp -y

# Print success message
    echo "Installation of Git, Vim, Python 3, and GIMP has been completed!"
}

# Call the install_packages function
installz



VIM config
-------------------------------------------------------------------------------------------------------------

#!/bin/bash

nightflyz() {
  # Create .vim/colors directory if it doesn't exist
  mkdir -p ~/.vim/colors

  # Download Nightfly color scheme
  curl https://raw.githubusercontent.com/bluz71/vim-nightfly-guicolors/master/colors/nightfly.vim -o ~/.vim/colors/nightfly.vim

  # Set Nightfly as the default color scheme in .vimrc
  echo "syntax on" >> ~/.vimrc
  echo "colorscheme nightfly" >> ~/.vimrc

  # Print success message
  echo "Nightfly color scheme set as default in Vim!"
}

# Call the set_nightfly function
nightflyz
