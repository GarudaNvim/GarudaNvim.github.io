<div>
    <h1><span class="th-color h-font"><b>Themes</b></span></h1>    
</div>

We know what a good colorscheme can do! It is soothing. </br>
It can make you happy if you are sad and happier if you are already happy :) </br>
GarudaNvim allows you to seamlessly switch themes and customize the look of your editor.

## <span class="sh-font tsh-color">Default Theme</span>
**Onedarkpro**: A sleek dark theme that enhances code visibility.

Note - Selected and configured by the author. Feel free to change it at `~/.config/nvim/lua/graudanvim/plugin_config/color_config/init.lua`

## <span class="sh-font tsh-color">Available Themes</span>

### Pre-Installed

Neovim and Vim come with several built-in colorschemes. These are fairly minimal compared to custom themes but are reliable for basic color support. Here’s a list of the default colorschemes:

- **default**: The standard colorscheme if no other is specified.
- **delek**: A bright and readable scheme, often with green and blue tones.
- **desert**: A dark, low-contrast scheme, easy on the eyes.
- **elflord**: A high-contrast theme with blue and green highlights.
- **evening**: A darker theme with blue-gray tones, great for low-light settings.
- **industry**: A blue and green scheme with high contrast.
- **koehler**: A high-contrast, sharp theme with bright yellow highlights.
- **morning**: A light theme with pastel colors.
- **murphy**: A classic dark theme with muted colors.
- **pablo**: A low-contrast, grayish theme, easier on the eyes.
- **peachpuff**: A light and pastel-colored theme.
- **ron**: A warm, dark scheme with brown and green highlights.
- **shine**: A theme with light colors, good for readability.
- **slate**: A soft, dark theme with a slight blue tint.
- **torte**: A mostly light-colored theme with subtle highlights.
  
### Externally Added

Beyond the built-in options, GarudaNvim brings additional color-rich themes that enhance the visual experience. Here’s a selection of popular externally added themes:

- **OneDarkPro**: Vibrant, professional, and easy on the eyes.
- **Dracula**: Dark with purple-pink highlights, gentle on eyes.
- **Nordic**: Cool blues and grays, minimalist vibe.
- **Tokyonight**: Inspired by Tokyo’s nightlife, moody and dark.
- **Tokyodark**: Deep blacks and blues, high contrast.
- **Catppuccin**: Warm pastels, cozy and relaxing.
- **Nightfox**: Dark themes with harmonious color accents. 

## <span class="sh-font tsh-color">Switching Themes</span>

Ah, the joy of theme-switching – like picking out a new outfit for your code! For the best experience, we highly recommend using the custom keymap that makes it effortless to try out different themes and get a live preview, all with a few taps.

### GarudaNvim Way
To switch themes instantly, just hit:
```
<space> + z + t
```
Your `which-key` setup has this mapped beautifully, so go ahead and tap away to preview themes on the fly! Why use this? Because it’s more satisfying than typing commands like it’s the 90s. Plus, who doesn’t love a shortcut? 

<div align="center">OR</div>

### The Traditional Way
Still a fan of the classics? You can switch themes the old-school way with this command:

```vim
:colorscheme <scheme-name>
```

Simply replace `<scheme-name>` with the name of your desired theme, like `:colorscheme desert`.

**Pro Tip**: Remember, a good theme isn’t just for looks – it’s a vibe. Choose what suits you best!

## <span class="sh-font tsh-color">Customizing Themes</span>

To tweak an existing theme, modify the respective configuration file at:
```
~/.config/nvim/lua/garudanvim/plugin_config/color_config/
```

In this file, you can change colors, contrasts, and more to match your preference.

<div class="navigation">
    <a href="/whichkey" class="nav-link">
        <div class="nav-content">
            <span class="arrow">⬅️</span>
            <div class="nav-text left">
                <span class="label">Previous</span>
                <span class="page-name">Which-Key</span>
            </div>
        </div>
    </a>
    <a href="/releases" class="nav-link">
        <div class="nav-content">
            <div class="nav-text right">
                <span class="label">Next</span>
                <span class="page-name">Releases</span>
            </div>
            <span class="arrow">➡️</span>
        </div>
    </a>
</div>
