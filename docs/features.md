<div>
    <h1><span class="th-color h-font"><b>Features of GarudaNvim</b></span></h1>    
</div>

GarudaNvim is more than just another Neovim setup – it’s a finely tuned machine built for those who want to code, not configure. From productivity-boosting keymaps to eye-pleasing themes, GarudaNvim takes Neovim to new heights. Dive in to see what makes it tick:

---

## <span class="sh-font tsh-color">Effortless Installation</span>
- **Automatic Setup, Minimal Hassle:** Our installer handles everything from OS detection to Neovim version validation to plugin setup, leaving you more time to focus on your code and less time wondering why things don’t work.
- **Cross-Platform Magic:** Whether you’re on macOS, Arch, Fedora, Ubuntu, Debian, CentOS/RHEL, or any of their derivative distributions (Manjaro, Mint, Pop!\_OS, Rocky Linux, and more), GarudaNvim’s installer has you covered. One run, and it’s all set up – no more wrestling with dependencies.

## <span class="sh-font tsh-color">Productivity Powerhouse</span>
- **Shortcut Wizardry:** With GarudaNvim’s custom keymaps, you’ll forget what “slow” feels like. Jump between files, split windows, resize buffers – it’s all a keystroke away. Less typing, more coding.
- **Which-Key Guidance:** With Which-Key as your guide, every possible keybinding is right at your fingertips. No more `<leader>` + ??? guessing games – just press, discover, and power up.
- **Text Surrounding with nvim-surround:** Add, change, or delete surrounding characters (brackets, quotes, tags) with minimal keystrokes. Works seamlessly with motions and visual selections.

## <span class="sh-font tsh-color">Enhanced Navigation</span>
- **Telescope for Search-Anything:** Need to find a file, buffer, or command? Telescope integration lets you glide through your project faster than a Ctrl+F on steroids. Say goodbye to scrolling aimlessly.
- **NvimTree for File Management:** A built-in, intuitive file explorer keeps all your files accessible with a simple shortcut. Navigate like a pro without ever leaving Neovim’s window.
- **Treesitter for Syntax-Aware Editing:** Grammar-based syntax highlighting and code-aware navigation powered by **nvim-treesitter**. Far more accurate than regex highlighting, across all major languages.
- **Alpha Dashboard:** A clean, welcoming dashboard greets you on startup with quick access to recent files and project shortcuts.

## <span class="sh-font tsh-color">Customizable UI Elements</span>
- **Polished Status and Tab Lines:** With **Lualine** for the statusline and **Barbar** for the tabline, you get a sleek, customizable interface that keeps tabs on your workflow without becoming a cluttered mess.
- **Revamped Command Line and Notifications with Noice:** The command line floats as a centered popup, notifications appear as non-blocking toasts, and LSP messages are rendered with clarity — keeping your editing surface clean and distraction-free.
- **Eye-Friendly Highlights:** Each highlight color and cursorline has been meticulously chosen to ensure comfort, visibility, and minimal eye strain – because staring at code all day is already hard enough.

## <span class="sh-font tsh-color">IDE-Grade Language Support</span>
- **Full LSP Support Out of the Box:** GarudaNvim ships with five language servers pre-configured and auto-installed via **Mason 2.0**: clangd (C/C++), pyright (Python), jdtls (Java), gopls (Go), and ts_ls (JavaScript/TypeScript/JSX/TSX). Diagnostics, hover docs, go-to-definition, references, and code actions all work immediately after opening a supported file.
- **Intelligent Code Completion with blink.cmp:** A fast, modern completion engine with LSP, snippet, path, and buffer sources active by default. Rounded popup menus, inline signature help, and `<Tab>`/`<S-Tab>` navigation make completion feel natural and unobtrusive.
- **Format on Save with conform.nvim:** Every supported language has a dedicated formatter (clang-format, ruff, google-java-format, goimports, prettier, stylua) that runs automatically on save. conform.nvim is the single source of truth — LSP formatting providers are disabled to prevent conflicts.
- **`<Space> l` for All LSP Actions:** Code actions, rename symbol, format buffer, hover docs, references, document and workspace symbols, LSP info, restart — all discoverable through Which-Key.

## <span class="sh-font tsh-color">AI-Powered Development</span>
- **Claude Code Integration:** The **Claude AI** coding assistant runs as a native terminal panel inside GarudaNvim via **claudecode.nvim**. Toggle, focus, resume, or continue Claude sessions without ever leaving the editor.
- **Send Code to Claude Instantly:** Add the current buffer or send a visual selection directly to Claude for analysis, refactoring, or explanation — all from inside Neovim with a single keypress.
- **Accept or Deny Diffs:** Claude's suggested edits appear as standard diffs; accept or deny them with `<Space> a a` / `<Space> a d` without touching the mouse.
- **`<Space> a` for All Claude Actions:** A dedicated Which-Key group exposes every Claude command — model selection, session management, and diff controls — making AI assistance fully keyboard-driven.

## <span class="sh-font tsh-color">Terminal & Git Integration</span>
- **ToggleTerm for In-Editor Terminals:** Spin up and toggle multiple terminal instances without leaving Neovim. Pre-configured windows for node, python, htop, and lazygit are ready out of the box.
- **Lazygit for Visual Git Management:** Commit, stash, reset, diff, and browse your full commit history — all from inside Neovim via the Lazygit TUI.
- **Gitsigns for Real-Time Git Feedback:** Added, changed, and deleted lines are marked in the gutter as you type. Blame annotations and staged change indicators are a keypress away.

## <span class="sh-font tsh-color">Multiple Themes Built In</span>
- **Color Schemes for Every Mood:** Choose from **Tokyo Night**, **Tokyo Dark**, **Nordic**, **Dracula**, **Catppuccin**, **Nightfox**, **OneDark Pro**, **Doom One**, and more — match your Neovim vibes with your monitor brightness (or your mood, no judgment here).
- **Instant Theme Preview:** Press `Space + z + t` to browse and switch colorschemes from a table view without touching a config file.

## <span class=”sh-font tsh-color”>Distro Self-Updater</span>
- **Update GarudaNvim From Inside Neovim:** Press `<Space> Z v` to open a floating version info panel showing your current version, the latest stable release, and how far behind you are. No terminal required.
- **Stable or Bleeding-Edge:** `<Space> Z u` updates to the latest stable git tag; `<Space> Z U` pulls the latest commit from main. Both ask for confirmation before touching anything.
- **Safety First:** The updater checks for uncommitted local config changes before running any git command and aborts with a clear message if any are found — your customizations are never at risk.

## <span class=”sh-font tsh-color”>Seamless Plugin Management</span>
- **Lazy for Effortless Plugin Control:** Why “install manually” when you can “install lazily”? With the **Lazy** plugin manager, adding, updating, or removing plugins is as effortless as a lazy Sunday.
- **Mason for LSP Server Management:** Install, update, and manage language servers and formatters through a polished UI (`<Space> u m o`). Mason 2.0 handles everything automatically on first launch.
- **Modular Plugin Structure:** Plugins are organized across separate files by category, making it easy to find, add, or remove individual plugins without scrolling through one monolithic list.
- **Curated Essentials:** Hand-picked plugins for maximum productivity – from **Onedarkpro** for a pleasing default theme to **Telescope** for instant file searching. Only the best make the cut.

## <span class="sh-font tsh-color">Minimal Yet Expandable</span>
- **Core Setup, Endless Potential:** GarudaNvim starts minimal so you can build up as needed. Want a bare-bones environment? Done. Want to add your own collection of plugins and tweak everything? Go wild.
- **Easy Customization:** Adjust options, add new plugins, or play around with settings without having to unearth cryptic files. The setup is designed to be as flexible as a Neovim enthusiast’s ideal config.

## <span class="sh-font tsh-color">Detailed Documentation</span>
- **Knowledge At Your Fingertips:** Whether you’re a Neovim newbie or a seasoned coder, the GarudaNvim Docs cover everything you need to know, from installation to mastering every shortcut. No need to trawl forums for answers.
- **Example-Rich Explanations:** Real examples, quick tips, and straightforward instructions ensure that you spend more time coding and less time deciphering docs.

## <span class="sh-font tsh-color">Updates and Feedback</span>
- **Constant Updates and Improvements:** GarudaNvim is a passion project by Priyanshu Ranjan, supported by a growing community of Neovim enthusiasts. Expect regular improvements, fresh features, and feedback-driven updates.
- **Built by Coders, for Coders:** GarudaNvim grows with the feedback of real-world usage, so everything here is designed with developers' needs in mind.

---

Take GarudaNvim for a spin, and you’ll see – it’s the Neovim setup you didn’t know you needed. It’s efficient, it’s powerful, and yes, it’s a bit sarcastic. But when you’re coding at warp speed, you’ll get it.

<div class="navigation">
    <a href="/installation" class="nav-link">
        <div class="nav-content">
            <span class="arrow">⬅️</span>
            <div class="nav-text left">
                <span class="label">Previous</span>
                <span class="page-name">Installation</span>
            </div>
        </div>
    </a>
    <a href="/plugins" class="nav-link">
        <div class="nav-content">
            <div class="nav-text right">
                <span class="label">Next</span>
                <span class="page-name">Plugins</span>
            </div>
            <span class="arrow">➡️</span>
        </div>
    </a>
</div>
