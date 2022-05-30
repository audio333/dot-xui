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

### Github
* [yt-dlp](https://github.com/yt-dlp/yt-dlp#installation)
  * `$ sudo curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp`
  * `$ sudo chmod a+rx /usr/local/bin/yt-dlp`
* [ytfzf](https://github.com/pystardust/ytfzf#install)
  * `$ sudo apt install jq`
  * `$ git clone https://github.com/pystardust/ytfzf`
  * `$ cd ytfzf`
  * `$ sudo make install doc`
* [torrentflix](https://github.com/ItzBlitz98/torrentflix#install-manual)
  * `$ npm install -g peerflix`
  * `$ git clone https://github.com/ItzBlitz98/torrentflix`
  * `$ cd torrentflix`
  * `$ npm install`
* [ani-cli](https://github.com/pystardust/ani-cli#linux--mac-os)
  * `$ sudo apt install grep sed awk curl openssl mpv aria2 ffmpeg` 
  * `$ sudo curl -sL github.com/pystardust/ani-cli/raw/master/ani-cli -o /usr/local/bin/ani-cli` 
  * `$ sudo chmod +x /usr/local/bin/ani-cli` 
* [mov-cli](https://github.com/mov-cli/mov-cli#shell)
  * `$ git clone https://github.com/mov-cli/mov-cli` 
  * `$ cd mov-cli` 
  * `$ ./mov-cli` 

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

