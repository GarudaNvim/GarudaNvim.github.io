<div>
    <h1><span class="th-color h-font"><b>Installation</b></span></h1>    
</div>

Installing GarudaNvim is a breeze. Follow the steps below to get GarudaNvim up and running on your machine.

## <span class="sh-font tsh-color">Installation Command</span>

Run the following command to install GarudaNvim on your system:

```sh
LATEST=$(curl -s https://api.github.com/repos/GarudaNvim/Installer/releases/latest | grep '"tag_name"' | cut -d '"' -f 4)
wget -q https://raw.githubusercontent.com/GarudaNvim/Installer/$LATEST/installGarudaNvim.sh
chmod +x installGarudaNvim.sh && { ./installGarudaNvim.sh } || { echo }
rm -f installGarudaNvim.sh
```

</br>

## <span class="sh-font tsh-color">Uninstallation</span>

To uninstall GarudaNvim, use the command below:

```sh
LATEST=$(curl -s https://api.github.com/repos/GarudaNvim/Installer/releases/latest | grep '"tag_name"' | cut -d '"' -f 4)
wget -q https://raw.githubusercontent.com/GarudaNvim/Installer/$LATEST/uninstallGarudaNvim.sh
chmod +x uninstallGarudaNvim.sh && { ./uninstallGarudaNvim.sh } || { echo }
rm -f uninstallGarudaNvim.sh
```
</br>

For more information on the script used for Installation (and Uninstallation), checkout our [Installer Repo](https://github.com/GarudaNvim/Installer)

<div class="navigation">
    <a href="/" class="nav-link">
        <div class="nav-content">
            <span class="arrow">⬅️</span>
            <div class="nav-text left">
                <span class="label">Previous</span>
                <span class="page-name">Home</span>
            </div>
        </div>
    </a>
    <a href="/features" class="nav-link">
        <div class="nav-content">
            <div class="nav-text right">
                <span class="label">Next</span>
                <span class="page-name">Features</span>
            </div>
            <span class="arrow">➡️</span>
        </div>
    </a>
</div>
