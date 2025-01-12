# Part 1
```shell
cd ~ && sudo pacman -S git && git clone "https://github.com/TormentedProgram/archinstall.git" && sudo archinstall --config ./archinstall/user_configuration.json```
```
# Part 2
```shell
cd ~ && git clone https://aur.archlinux.org/yay-bin.git && cd yay-bin && makepkg -si && cd ~ && git clone "https://github.com/TormentedProgram/archinstall.git" && yay -S --noconfirm - < ./archinstall/aur.txt
```

# Part 3
```shell
chezmoi init --apply tormentedprogram
```
