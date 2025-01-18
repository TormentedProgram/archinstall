# Part 1
```shell
pacman -Sy && pacman -S git && git clone "https://github.com/TormentedProgram/archinstall.git"
archinstall --config ./archinstall/user_configuration.json
```
# Part 1.5 (OPTIONAL)
```shell
cd ~ && git clone https://aur.archlinux.org/hyde-cli-git.git && cd ./hyde-cli
makepkg -si
Hyde-install
```
# Part 2
```shell
cd ~
git clone https://aur.archlinux.org/yay-bin.git && cd yay-bin && makepkg -si && cd ~ && git clone "https://github.com/TormentedProgram/archinstall.git" && yay -S --noconfirm - < ./archinstall/aur.txt
chezmoi init --apply tormentedprogram
```
