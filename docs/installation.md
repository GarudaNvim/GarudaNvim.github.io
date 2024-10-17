# Installation Guide

Installing GarudaNvim is a breeze. Follow the steps below to get GarudaNvim up and running on your machine.

### Installation Command

Run the following command to install GarudaNvim on your system:

```sh
LATEST=$(curl -s https://api.github.com/repos/GarudaNvim/Installer/releases/latest | grep '"tag_name"' | cut -d '"' -f 4)
wget -q https://raw.githubusercontent.com/GarudaNvim/Installer/$LATEST/installGarudaNvim.sh
chmod +x installGarudaNvim.sh && { ./installGarudaNvim.sh } || { echo }
rm -f installGarudaNvim.sh
```

</br>

#### Uninstallation
To uninstall GarudaNvim, use the command below:
```sh
LATEST=$(curl -s https://api.github.com/repos/GarudaNvim/Installer/releases/latest | grep '"tag_name"' | cut -d '"' -f 4)
wget -q https://raw.githubusercontent.com/GarudaNvim/Installer/$LATEST/uninstallGarudaNvim.sh
chmod +x uninstallGarudaNvim.sh && { ./uninstallGarudaNvim.sh } || { echo }
rm -f uninstallGarudaNvim.sh
```
