<div>
    <h1><span class="pages-heading"><b>Keymaps</b></span></h1>    
</div>

*Welcome to the land of keymaps, where every keystroke counts, and Neovim becomes your playground. We know you're here because you're tired of typing the same old commands a thousand times a day. Well, you've come to the right place! With GarudaNvim's custom keymaps, we’re putting your fingers on the fast lane to efficiency. But before you start flying through your code, remember: with great power comes great responsibility. Use these keybindings wisely, or you might just get too lazy to use the mouse again. No pressure, though.*

Also, don't forget that *this is just the beginning.* After mastering these, head over to the **which-key** page—our beloved menu of shortcuts. Trust us, it’ll make you feel like a coding ninja, minus the actual ninja suit.*

### Neovim Modes
- **Normal Mode** (`n`): The default mode for most actions, like navigating, editing, and breaking stuff (whoops).
- **Insert Mode** (`i`): Where you go when you need to type things (or mess up an entire file).
- **Visual Mode** (`v`): Selecting text to either copy, delete, or wonder why you selected it in the first place.
- **Visual Block Mode** (`x`): For when you need to select columns of text and feel like you're hacking the matrix.
- **Terminal Mode** (`t`): The mode where you're constantly reminded that a terminal lives inside Neovim. Trippy, right?
- **Command Mode** (`c`): Where you talk to Neovim. Or maybe yell at it. No judgment.

---

### General Setup

- **Leader Key**: GarudaNvim uses the space bar (`<Space>`) as the leader key. It’s the most powerful key on your keyboard now, so treat it with respect. Here's how it's mapped:
    ```lua
    map("", "<Space>", "<Nop>", opts)
    vim.g.mapleader = " "
    vim.g.maplocalleader = " "
    ```

---

### Keymaps in Normal Mode

Welcome to normal mode, where the magic happens, and where most of your day will be spent.

- **Better Window Navigation**: Say goodbye to confusing window setups. Move between windows with ease.
    - `<C-h>`: Move to the window on the left.
    - `<C-j>`: Move to the window below.
    - `<C-k>`: Move to the window above.
    - `<C-l>`: Move to the window on the right.
    ```lua
    map("n", "<C-h>", "<C-w>h", opts)
    ```

- **Resize Windows**: Windows need resizing? No problem.
    - `<C-q>`: Decrease window height.
    - `<C-w>`: Increase window height.
    - `<C-a>`: Decrease window width.
    - `<C-s>`: Increase window width.
    ```lua
    map("n", "<C-q>", ":resize -1<CR>", opts)
    ```

- **Navigate Buffers**: Cycle through your open buffers like a pro.
    - `<S-l>`: Move to the next buffer.
    - `<S-h>`: Move to the previous buffer.
    ```lua
    map("n", "<S-l>", ":BufferNext<CR>", opts)
    ```

- **Move Buffers**: Reorganize your buffers in style.
    - `<S-i>`: Move the current buffer to the right.
    - `<S-u>`: Move the current buffer to the left.
    ```lua
    map("n", "<S-i>", ":BufferMoveNext<CR>", opts)
    ```

- **Move Text Up and Down**: Because who needs to retype lines?
    - `<S-j>`: Move the current line down.
    - `<S-k>`: Move the current line up.
    ```lua
    map("n", "<S-j>", "<Esc>:m .+1<CR>==gi", opts)
    ```

- **Quick Actions**: Be the action hero of your Neovim setup.
    - `<Esc>` or `q`: Clear search highlights. 
    - `<C-c>`: Copy the entire file content to the system clipboard. 
    - `d`: Delete without yanking (yes, you can safely delete now).
    - `<Space>e`: Toggle the NvimTree file explorer. 
    ```lua
    map("n", "<C-c>", "<cmd> %y+ <CR><CR>", opts)
    ```

- **Go to Beginning and End of Line**: Quick shortcuts for lazy cursor movers.
    - `<C-i>`: Go to the beginning of the line.
    - `<C-j>`: Go to the end of the line.
    ```lua
    map("n", "<C-i>", "0", opts)
    ```

---

### Keymaps in Insert Mode

Insert mode: for the brave, the bold, and those who actually need to type things.

- **Exit Insert Mode**: Exit insert mode with the magic of `kj`. No more `Esc` key reaching!
    ```lua
    map("i", "kj", "<ESC>", opts)
    ```

- **Move Within Insert Mode**: Navigate around while still in insert mode (yes, it's as cool as it sounds).
    - `<C-h>`: Move left.
    - `<C-l>`: Move right.
    - `<C-j>`: Move down.
    - `<C-k>`: Move up.
    ```lua
    map("i", "<C-h>", "<Left>", opts)
    ```

- **Go to Beginning and End of Line**: Quick shortcuts for lazy cursor movers inside insert mode.
    - `<C-i>`: Go to the beginning of the line.
    - `<C-j>`: Go to the end of the line.
    ```lua
    map("i", "<C-i>", "<ESC>^i", opts) -- beginning of line
    ```

---

### Keymaps in Visual Mode

Visual mode: where selection happens, and text manipulation gets real.

- **Indenting While Staying in Visual Mode**: Keep your selection while indenting. Handy, right?
    - `<`: Indents your selected line to the left
    - `>`: Indents your selected line to the right
    ```lua
    map("v", "<", "<gv", opts)
    ```

- **Move Text**: Shift selected text up or down without losing your mind.
    - `<S-j>`: Move selected text down.
    - `<S-k>`: Move selected text up.
    ```lua
    map("v", "<S-j>", ":m .+1<CR>==", opts)
    ```

- **Pasting Over Text**: Paste over text without yanking it to the void.
    ```lua
    map("v", "p", '"_dP', opts)
    ```

- **Replacement of Texts**: Replaces the selected text via `<C-r>` with a prompt for the new text (global, with confirmation for each instance).
    ```lua
    map("v", "<C-r>", '"hy:%s/<C-r>h//gc<left><left><left>', opts)
    ```

---

### Keymaps in Visual Block Mode

For when you need to manipulate columns of text like a true hacker.

- **Move Block of Text**: Push blocks of text around like it's no big deal.
    - `J`: Move the block down.
    - `K`: Move the block up.
    ```lua
    map("x", "J", ":move '>+1<CR>gv-gv", opts)
    ```

---

### Additional Customization

GarudaNvim allows you to modify or extend these keymaps based on your workflow. We believe in the power of personalization. If these aren’t enough, feel free to dive into the `keymaps.lua` file and add more.
