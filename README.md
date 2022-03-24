# X-platform terminal / graphical ui apps

### Apt
* `$ sudo apt install cmatrix newsboat cowsay fortune`

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

