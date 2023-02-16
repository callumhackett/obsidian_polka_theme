# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Preview](polka_full_size.png)

<a href="https://www.buymeacoffee.com/callumhackett" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Color Customization

Due to the way the theme shares color values between elements for cohesion, Polka ignores the accent color in your Obsidian settings. You can still choose your own accent color, which will be applied in the ribbon and elsewhere, but you'll need to create a CSS snippet that overrides the `--accent-main` parameter with a raw RGB value (scroll to the bottom for instructions on how to set this up).

For example, you could replace the default cyan accent in dark mode with a pink one:

![Customization](color_customization.png)

## Fonts

The user is left to select which fonts are loaded via the main settings. The font used in the preview images here is Franklin Gothic, which you already have if you have Windows. If you want a good, free alternative, try [Rubik](https://fonts.google.com/specimen/Rubik).

## Plugin Support

As well as modifying your workspace, Polka has color adaptations for Obsidian's user interface and the whole suite of core plugins. Additionally, though code syntax colors use the built-in color scheme, the hues have been refined.

Special attention has been given to the following community plugins (many others will fit in without issue):

- [Calendar](https://github.com/liamcain/obsidian-calendar-plugin)
- [Dictionary](https://github.com/phibr0/obsidian-dictionary)
- [Execute Code](https://github.com/twibiral/obsidian-execute-code)
- [Kanban](https://github.com/mgmeyers/obsidian-kanban)

## CSS Snippets

To choose your own accent color, or to otherwise modify the theme:

1. In a file explorer (not inside Obsidian), go to your main vault folder.
2. From there, go to `/.obsidian/snippets` and create a `.css` file with any name.
3. Add new styles to the file. To replace the accent color, use the following rule as a template, setting your own RGB values and using `.theme-light` or `.theme-dark` as appropriate:
```
.theme-dark {
  --accent-main: 225, 120, 255 !important;
}
```
4. Note that the RGB values are not enclosed inside `rgb()` brackets (if you copied the snippet above, you'll be fine).
5. In your main Obsidian settings, go to `Appearance > CSS snippets` and enable your file.

## Notes

Some UI features and community plugins may use whichever accent color is defined in your user settings under `Appearance > Accent color`, rather than the color associated with the theme, so you might want to change the color in your settings to reflect the current theme accent. If you find an inconsistency like this, [let me know through GitHub](https://github.com/callumhackett/obsidian_polka_theme) and I'll patch it.
