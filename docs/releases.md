<div>
    <h1><span class="th-color h-font"><b>Releases</b></span></h1>    
</div>

GarudaNvim continuously evolves with each update, refining features, squashing bugs, and adding tools to make your Neovim experience smoother and more efficient. As a Neovim distribution designed for code and keyboard enthusiasts, GarudaNvim receives regular updates that improve performance, introduce new plugins, and enhance the user interface, allowing coders to be more productive and enjoy coding even more.

Below, you’ll find details on our current and previous releases, including version numbers, release dates, new features, and links to each update. Each release strives to bring GarudaNvim closer to the needs of developers who value simplicity, speed, and robust functionality.

---

## <span class="sh-font tsh-color">Current Release</span>

### **Version: 1.5.0**
- **Release Date:** June 17, 2026
- **Features:**
    - Full **LSP support**: clangd (C/C++), pyright (Python), jdtls (Java), gopls (Go), ts_ls (JS/TS/JSX/TSX) via **Mason 2.0**
    - Intelligent code **completion** with **blink.cmp** (LSP, snippets, path, buffer sources)
    - **Format on save** for all supported languages via **conform.nvim**
    - **Claude Code AI integration** — AI coding assistant as a native panel inside Neovim
    - **GarudaNvim self-updater** (`<Space> Z`) — update to stable or bleeding-edge from inside the editor
    - Minimum Neovim version bumped to **0.10.0**
- **Link:** [GarudaNvim v1.5.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v1.5.0)

---

## <span class="sh-font tsh-color">Past Releases</span>

### **Version: 1.4.0**
- **Release Date:** June 16, 2025
- **Features:**
    - Precise, grammar-based syntax highlighting with **nvim-treesitter**
    - Revamped command-line and notification UI with **Noice**
    - Effortless text surrounding with **nvim-surround**
    - New **Doom One** colorscheme
    - Modular **plugin structure overhaul** (dump_plugins refactored into separate files)
    - **Keymap bug fixes** for a smoother navigation experience
- **Link:** [GarudaNvim v1.4.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v1.4.0)

### **Version: 1.3.0**
- **Release Date:** November 1, 2024
- **Features:**
    - Streamlined keybindings with **WhichKey**
    - Versatile Terminal Management with **ToggleTerm**
    - Enhanced git functionality with **Lazygit**
    - Visual git tracking with **Gitsigns**
    - Intelligent new **Installer**
    - More **Colorschemes** so that no one feels left out
- **Link:** [GarudaNvim v1.3.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v1.3.0)

### **Version: 1.2.0**
- **Release Date:** October 19, 2024
- **Features:**
    - Fuzzy finder with **Telescope plugin**
    - Simplified project management with **Project.nvim**
    - Dashboard screen with **Alpha.nvim**
    - New **Colorscheme** options for users
- **Link:** [GarudaNvim v1.2.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v1.2.0)

### **Version: 1.1.0**
- **Release Date:** October 13, 2024
- **Features:**
    - New **Colorscheme plugins** added
    - Updated **Default colorscheme** to better suit the user's needs
    - Better tab and buffer management with **Barbar.nvim**
    - Sleek and informative statusline with **Lualine.nvim**
- **Link:** [GarudaNvim v1.1.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v1.1.0)

### **Version: 1.0.0**
- **Release Date:** October 11, 2024
- **Features:**
    - Extended OS support for **Linux Distributions**
    - Hassle free plugin installation with **Lazy plugin manager**
    - Enhanced file exploration with **NvimTree**
    - Set the **Onedarkpro** theme as default colorscheme
    - **Custom keymaps** for streamlined navigation and code editing.
    - Reorganized **Folder structure**
    - **Readme** updated
- **Link:** [GarudaNvim v1.0.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v1.0.0)

### **Version: 0.2.0**
- **Release Date:** October 7, 2024
- **Features:**
    - Clener **Folder Structure**
    - Core GarudaNvim Settings with **Options.lua** file
- **Link:** [GarudaNvim v0.2.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v0.2.0)

### **Version: 0.1.0 - Initial Release**
- **Release Date:** October 4, 2024
- **Features:**
    - Automated **Installer Script**
    - Intuitive keybindings with **Keymaps.lua** file
- **Link:** [GarudaNvim v0.1.0 Release Notes](https://github.com/GarudaNvim/GarudaNvim/releases/tag/v0.1.0)

---

## <span class="sh-font tsh-color">Installer Releases</span>

The installer is versioned separately from GarudaNvim. The install command always fetches the latest installer release automatically.

### **Version: 0.6.0** — Current
- **Release Date:** June 17, 2026
- **Changes:**
    - Minimum Neovim version bumped from **0.9.0** to **0.10.0**, matching GarudaNvim v1.5.0 requirements
- **Link:** [Installer v0.6.0 Release Notes](https://github.com/GarudaNvim/Installer/releases/tag/v0.6.0)

### **Version: 0.5.0**
- **Release Date:** June 15, 2026
- **Changes:**
    - Fixed shell compatibility (`bash` shebang instead of `sh`)
    - Fixed OS detection for derivative distros via `$ID_LIKE`
    - Fixed dangerous `pacman -Sy` on Arch Linux
    - Added Neovim minimum version check (>= 0.9.0)
    - Added warnings for RHEL/CentOS dependency gaps (ripgrep, lazygit)
    - Fixed `git describe` crash on repos with no tags
    - Fixed font detection to use glob instead of exact filename
- **Link:** [Installer v0.5.0 Release Notes](https://github.com/GarudaNvim/Installer/releases/tag/v0.5.0)

### **Version: 0.4.0**
- **Link:** [Installer v0.4.0 Release Notes](https://github.com/GarudaNvim/Installer/releases/tag/v0.4.0)

### **Version: 0.3.0**
- **Link:** [Installer v0.3.0 Release Notes](https://github.com/GarudaNvim/Installer/releases/tag/v0.3.0)

### **Version: 0.2.0**
- **Link:** [Installer v0.2.0 Release Notes](https://github.com/GarudaNvim/Installer/releases/tag/v0.2.0)

### **Version: 0.1.0 - Initial Release**
- **Link:** [Installer v0.1.0 Release Notes](https://github.com/GarudaNvim/Installer/releases/tag/v0.1.0)

---

Keep an eye on this page for more updates, as GarudaNvim continues to roll out enhancements and new features with each release!

<div class="navigation">
    <a href="/themes" class="nav-link">
        <div class="nav-content">
            <span class="arrow">⬅️</span>
            <div class="nav-text left">
                <span class="label">Previous</span>
                <span class="page-name">Themes</span>
            </div>
        </div>
    </a>
    <a href="/codeofconduct" class="nav-link">
        <div class="nav-content">
            <div class="nav-text right">
                <span class="label">Next</span>
                <span class="page-name">Code of Conduct</span>
            </div>
            <span class="arrow">➡️</span>
        </div>
    </a>
</div>
