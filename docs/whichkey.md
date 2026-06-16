<div>
    <h1><span class="th-color h-font"><b>Which-Key Keybindings</b></span></h1>    
</div>

Welcome to the secret stash of keybindings that revolve around everyone's favorite key—the space key! If you thought the keymaps file was all there is to GarudaNvim’s superpowers, well, think again.

This is the page where we take the humble `space` key and transform it into your personal coding Swiss Army Knife. The creator decided that there’s so much the space key can do, it deserved a page all to itself. So, here we are—another chapter in the saga of making your life as a coder easier, one keybinding at a time. Yes, you’ll need some patience to explore all the hidden gems, but hey, it’s way more satisfying than scrolling through endless Stack Overflow posts (you know it’s true).  

Take a deep breath, grab your coffee, and dive in—each keybinding has been placed with the precision of a seasoned developer trying to avoid a merge conflict. You might not even realize how badly you needed these shortcuts until you try them. Seriously, give them a shot. And don’t worry, the space key isn’t overloaded like your browser’s open tabs. It’s just filled with shortcuts that will make you wonder how you ever coded without them.

## <span class="sh-font tsh-color">Keybindings List</span>

### General Shortcuts
- `<Space> e`: Toggle NvimTree (File Explorer)
- `<Space> N`: Open a new buffer
- `<Space> s`: Save the current buffer
- `<Space> q`: Quit GarudaNvim
- `<Space> w`: Close the current buffer
- `<Space> f`: Find files using Telescope
- `<Space> p`: Open recent projects
- `<Space> t`: Open a floating terminal

### Diagnostics
- `<Space> d b`: Show buffer diagnostics
- `<Space> d p`: Show workspace diagnostics
- `<Space> d n`: Jump to next diagnostic
- `<Space> d v`: Jump to previous diagnostic
- `<Space> d o`: Open diagnostic float

### Find Files and More
- `<Space> F a`: Find all files (including hidden and no-ignore files)
- `<Space> F l`: Find text in files
- `<Space> F b`: Find buffers
- `<Space> F h`: Open help page
- `<Space> F o`: Find old files
- `<Space> F k`: Find file types
- `<Space> F c`: Find text in the current buffer

### Terminals
- `<Space> T n`: Open Node terminal
- `<Space> T t`: Open Htop
- `<Space> T p`: Open Python terminal
- `<Space> T h`: Open horizontal terminal
- `<Space> T v`: Open vertical terminal

### Git Shortcuts
- `<Space> g s`: Show git status
- `<Space> g b`: Show git branches
- `<Space> g c`: Show git commits
- `<Space> g f`: Show git files
- `<Space> g h`: Show git stash
- `<Space> g g`: Open Lazygit
- `<Space> g j`: Move to the next git hunk
- `<Space> g v`: Move to the previous git hunk
- `<Space> g l`: Blame current line
- `<Space> g p`: Preview the current hunk
- `<Space> g r`: Reset the current hunk
- `<Space> g R`: Reset the entire buffer
- `<Space> g k`: Stage the current hunk
- `<Space> g d`: Show diff of the current buffer with HEAD
- `<Space> g u`: Undo the stage of the current hunk

### Buffer Management (Barbar Plugin)
- `<Space> B f`: Move to the first buffer
- `<Space> B l`: Move to the last buffer
- `<Space> B p`: Pin/Unpin the buffer
- `<Space> B t`: Restore the last closed buffer
- `<Space> B s`: Move buffer to start
- `<Space> B i`: Pick a buffer
- `<Space> B d`: Delete a picked buffer
- `<Space> B c`: Close all buffers except the current one
- `<Space> B o n`: Order buffers by buffer number
- `<Space> B o d`: Order buffers by directory
- `<Space> B o l`: Order buffers by language
- `<Space> B o w`: Order buffers by window number

### Update/Install Plugins and Language Extensions
- `<Space> u l s`: Sync plugins (Lazy Plugin Manager)
- `<Space> u l k`: Check for plugin updates
- `<Space> u l h`: Open Lazy plugin help
- `<Space> u l c`: Clean unused plugins
- `<Space> u l e`: Check Lazy health
- `<Space> u l l`: Show Lazy logs
- `<Space> u l u`: Update plugins
- `<Space> u l r`: Reload plugins

### Treesitter
- `<Space> u t i`: Show Treesitter install info
- `<Space> u t s`: Install parsers (sync)
- `<Space> u t u`: Update all parsers
- `<Space> u t y`: Update parsers (sync)
- `<Space> u t m`: Show Treesitter module info
- `<Space> u t a`: Toggle syntax highlighting
- `<Space> u t b`: Toggle indentation
- `<Space> u t c`: Toggle incremental selection

### Mason — LSP Server Manager
- `<Space> u m o`: Open Mason UI
- `<Space> u m u`: Update Mason registries
- `<Space> u m t`: Install all configured tools
- `<Space> u m T`: Update all installed tools

### Setup Related Shortcuts
- `<Space> z t`: Switch colorschemes using Telescope
- `<Space> z h`: Check GarudaNvim health
- `<Space> z c`: Collapse NvimTree

### GarudaNvim Distro Management
- `<Space> Z v`: Show version info (current, latest stable, remote HEAD)
- `<Space> Z k`: Check for updates (silent notification)
- `<Space> Z u`: Update to latest stable release
- `<Space> Z U`: Update to latest commit on main (bleeding edge)

### LSP
- `<Space> l a`: Code action
- `<Space> l d`: Go to definition (Telescope)
- `<Space> l D`: Go to declaration
- `<Space> l f`: Format buffer
- `<Space> l h`: Hover docs
- `<Space> l i`: LSP info
- `<Space> l n`: Rename symbol
- `<Space> l r`: References (Telescope)
- `<Space> l s`: Signature help
- `<Space> l S`: Stop LSP
- `<Space> l R`: Restart LSP
- `<Space> l t`: Type definition (Telescope)
- `<Space> l y`: Document symbols (Telescope)
- `<Space> l w`: Workspace symbols (Telescope)

### Claude Code AI
- `<Space> a c`: Toggle Claude panel
- `<Space> a f`: Focus Claude panel
- `<Space> a r`: Resume last session
- `<Space> a C`: Continue last session
- `<Space> a m`: Select model
- `<Space> a b`: Add current buffer to Claude
- `<Space> a a`: Accept Claude diff
- `<Space> a d`: Deny Claude diff

### Claude Code AI (Visual Mode)
- `<Space> a s`: Send selection to Claude

## <span class="sh-font tsh-color">Additional Notes from the Which-Key Setup</span>

The **Which-Key** plugin has been configured to provide a clear and helpful interface for key mappings, enhancing productivity with the following features:

- **Marks and Registers**: Which-Key shows marks and registers (`'` and `"`) to make navigation and clipboard use more convenient.
- **Spelling Suggestions**: When pressing `z=`, Which-Key suggests up to 20 spelling corrections.
- **Default Keybinding Help**: It provides help for a variety of default Neovim keybindings such as operators (`d`, `y`, etc.), motions, and text objects.
- **Window Management**: Native bindings for managing windows (e.g., `<c-w>` for window control) are included in the help display.

The setup also includes scroll mapping (`<c-d>` to scroll down, `<c-u>` to scroll up), customizable window borders (`rounded` in this case), and the ability to ignore boilerplate commands (`<cmd>`, `lua`, etc.) to keep the interface clean.

---

This should provide a complete overview of your keybindings and additional details from your `which-key` configuration in a Markdown-friendly format.

<div class="navigation">
    <a href="/keymaps" class="nav-link">
        <div class="nav-content">
            <span class="arrow">⬅️</span>
            <div class="nav-text left">
                <span class="label">Previous</span>
                <span class="page-name">Keymaps</span>
            </div>
        </div>
    </a>
    <a href="/themes" class="nav-link">
        <div class="nav-content">
            <div class="nav-text right">
                <span class="label">Next</span>
                <span class="page-name">Themes</span>
            </div>
            <span class="arrow">➡️</span>
        </div>
    </a>
</div>
