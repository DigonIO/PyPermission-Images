FROM archlinux:base-20221204.0.107760

RUN echo 'Server = https://archive.archlinux.org/repos/2022/12/04/$repo/os/$arch' > /etc/pacman.d/mirrorlist

RUN pacman -Syy
RUN pacman -S zsh python python-pip mariadb gcc npm --noconfirm

RUN chsh -s /usr/bin/zsh root

RUN pacman -Q -s mariadb
RUN pacman -Q -s python
RUN pacman -Q -s npm