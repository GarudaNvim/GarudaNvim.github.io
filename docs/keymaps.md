# Keymaps

In Neovim, different modes allow users to interact with their text and environment in specific ways. GarudaNvim enhances this experience with custom keymaps tailored for efficient workflow ensuring fast navigation and editing. Here’s an overview of the keymaps provided in GarudaNvim.

### Neovim Modes
- **Normal Mode** (`n`): The default mode for most actions, such as moving through text and performing edits.
- **Insert Mode** (`i`): Where text is inserted into the buffer.
- **Visual Mode** (`v`): Used for selecting and manipulating chunks of text.
- **Visual Block Mode** (`x`): A block selection mode for columns of text.
- **Terminal Mode** (`t`): Used within terminal windows in Neovim.
- **Command Mode** (`c`): Where Ex commands are entered.

### General Setup

- **Leader Key**: GarudaNvim remaps the space bar (`<Space>`) as the leader key. This key is used in combination with other keys to trigger custom commands efficiently. 
    ```lua
    map("", "<Space>", "<Nop>", opts)
    vim.g.mapleader = " "
    vim.g.maplocalleader = " "
    ```

---

### Keymaps in Normal Mode

Normal mode is where you’ll spend most of your time in Neovim. These keymaps improve navigation, buffer management, and text manipulation.

- **Better Window Navigation**: Quickly switch between split windows using the control (`<C>`) key and directional keys.
    - `<C-h>`: Move to the window on the left.
    - `<C-j>`: Move to the window below.
    - `<C-k>`: Move to the window above.
    - `<C-l>`: Move to the window on the right.
    ```lua
    map("n", "<C-h>", "<C-w>h", opts)
    ```

- **Resize Windows with Arrows**: Use custom keybindings to resize windows without having to manually adjust them.
    - `<C-q>`: Decrease window height.
    - `<C-w>`: Increase window height.
    - `<C-a>`: Decrease window width.
    - `<C-s>`: Increase window width.
    ```lua
    map("n", "<C-q>", ":resize -1<CR>", opts)
    ```

- **Navigate Buffers**: Efficiently switch between open buffers.
    - `<S-l>`: Move to the next buffer.
    - `<S-h>`: Move to the previous buffer.
    ```lua
    map("n", "<S-l>", ":BufferNext<CR>", opts)
    ```

- **Move Text Up and Down**: Shift entire lines of text up or down.
    - `<S-j>`: Move the current line down.
    - `<S-k>`: Move the current line up.
    ```lua
    map("n", "<S-j>", "<Esc>:m .+1<CR>==gi", opts)
    ```

- **Quick Actions**: Handy shortcuts for common tasks.
    - `<Esc>` or `q`: Clear search highlights.
    - `<C-c>`: Copy the entire file content to the system clipboard.
    - `d`: Delete text without copying it to the clipboard (so it doesn’t replace the current yank).
    - `<Space>e`: Toggle the NvimTree file explorer.
    ```lua
    map("n", "<C-c>", "<cmd> %y+ <CR><CR>", opts)
    ```

- **Go to Beginning and End of Line**: Simplify cursor movement within lines.
    - `<C-e>`: Go to the end of the line.
    - `<C-b>`: Go to the beginning of the line.
    ```lua
    map("n", "<C-e>", "$", opts)
    ```

---

### Keymaps in Insert Mode

Insert mode is for entering text, and these mappings help you navigate and exit this mode more quickly.

- **Exit Insert Mode**: A quick way to exit insert mode by typing `kj`.
    ```lua
    map("i", "kj", "<ESC>", opts)
    ```

- **Move Within Insert Mode**: Use control + arrow keys to move the cursor while staying in insert mode.
    - `<C-h>`: Move left.
    - `<C-l>`: Move right.
    - `<C-j>`: Move down.
    - `<C-k>`: Move up.
    ```lua
    map("i", "<C-h>", "<Left>", opts)
    ```

---

### Keymaps in Visual Mode

Visual mode is for selecting text. GarudaNvim enhances this by allowing you to move and manipulate the selected text more easily.

- **Indenting While Staying in Visual Mode**: Keep text selected while indenting left or right.
    ```lua
    map("v", "<", "<gv", opts)
    ```

- **Move Text**: Shift selected text up or down in the file.
    - `<S-j>`: Move selected text down.
    - `<S-k>`: Move selected text up.
    ```lua
    map("v", "<S-j>", ":m .+1<CR>==", opts)
    ```

- **Pasting Over Text**: When pasting over a selection, the selected text is not yanked, so you can paste the same content multiple times.
    ```lua
    map("v", "p", '"_dP', opts)
    ```

- **Search and Replace**: Initiate a search and replace for the selected text.
    ```lua
    map("v", "<C-r>", '"hy:%s/<C-r>h//gc<left><left><left>', opts)
    ```

---

### Keymaps in Visual Block Mode

Visual block mode is especially useful for selecting columns of text or for editing multiple lines at once.

- **Move Block of Text**: Shift a block of text up or down.
    - `J`: Move the block down.
    - `K`: Move the block up.
    ```lua
    map("x", "J", ":move '>+1<CR>gv-gv", opts)
    ```

---

### Additional Customization

GarudaNvim allows you to modify or extend these keymaps based on your needs. You can easily add your own keymaps to further enhance your coding workflow.
For a complete list of keymaps, check out the `keymaps.lua` file.
