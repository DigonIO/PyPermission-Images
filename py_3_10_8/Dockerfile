FROM archlinux:base-20221106.0.100148

RUN echo 'Server = https://archive.archlinux.org/repos/2022/11/06/$repo/os/$arch' > /etc/pacman.d/mirrorlist

RUN pacman -Syy
RUN pacman -S zsh python python-pip mariadb gcc --noconfirm

RUN chsh -s /usr/bin/zsh root

RUN pacman -Q -s python
RUN pacman -Q -s mariadb