# X-platform terminal / graphical ui apps

### APT
* `$ sudo apt install tldr mycli newsboat`
* `$ sudo apt install cmatrix cowsay fortune figlet sl`

### PPA
* alacritty
  * `$ sudo add-apt-repository ppa:aslatter/ppa`

### WGET
* [sublime-text](https://www.sublimetext.com/docs/linux_repositories.html#apt)  
* [sublime-merge](https://www.sublimemerge.com/docs/linux_repositories#apt)
  * `$ wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -`
  * `$ sudo apt-get install apt-transport-https`
  * `$ echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list`

### Fresh Install Info
    sudo apt install git stow

    # clone dotfiles
    cd ~
    git clone https://github.com/audio333/dot-xui.git

    #backup current dotfiles
    mkdir -p ~/Downloads/stowbackup
    mv ~/.bashrc ~/Downloads/stowbackup

    # symlink all files in dotfiles dir to home dir
    cd ~/dot-xui

    # link only folders (trailing slash)
    stow -v -t ~ */

        # delete (-D flag)
        stow -v -D -t ~ */
        stow -v -D -t ~ newsboat

        # redo link (-R)
        stow -v -R -t ~ */
        stow -v -R -t ~ newsboat


    src: https://github.com/gotbletu

