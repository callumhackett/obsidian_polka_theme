# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Preview](polka_full_size.png)

<a href="https://www.buymeacoffee.com/callumhackett" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Color Customization

Due to the way the theme shares color values between elements for cohesion, Polka ignores the accent color in your Obsidian settings. You can still choose your own accent color, which will appear in the ribbon and elsewhere, but you'll need to create a CSS snippet and override the `--accent-main` parameter with a raw RGB value (scroll to the bottom for help on setting this up—it's easy!).

For example, you could replace the dark mode's default cyan accent with a pink one:

![Customization](color_customization.png)

## Fonts

Font taste is personal. Polka selects default fonts for Windows (Franklin Gothic) and Mac (Helvetica Neue) but your main font settings (`Appearance > Font`) will override these.

Franklin Gothic is the font you see in the prevew images here. If you want a good, free alternative, try [Rubik](https://fonts.google.com/specimen/Rubik). If you're after a code font, try [iA Writer Mono](https://github.com/iaolo/iA-Fonts/tree/master/iA%20Writer%20Mono), which is a fork of [IBM Plex Mono](https://github.com/IBM/plex) with some minor character adjustments.

## Plugin Support

As well as modifying your workspace, Polka adapts the colors of Obsidian's user interface and the whole suite of core plugins. Additionally, though code syntax colors use the built-in color scheme, the hues have been refined.

Special attention has been given to the following community plugins:

- [Calendar](https://github.com/liamcain/obsidian-calendar-plugin)
- [Dictionary](https://github.com/phibr0/obsidian-dictionary)
- [Execute Code](https://github.com/twibiral/obsidian-execute-code)
- [Kanban](https://github.com/mgmeyers/obsidian-kanban)

Many others will fit in without issue but [tell me](https://github.com/callumhackett/obsidian_polka_theme/issues) if I should support something else.

## CSS Snippets

To set your own accent color (or to apply other modifications):

1. In a file explorer (not inside Obsidian), go to your main vault folder.
2. From there, go to the `/.obsidian/snippets` folder and create a `.css` file with any name.
3. If you don't know CSS but want to replace the accent color, copy and paste the snippet below. Replace `.theme-dark` with `.theme-light` if you want to customize light mode, and replace the numbers with your preferred RGB color:
```
.theme-dark {
    --accent-main: 225, 120, 255 !important;
}
```
4. If you're familiar with CSS, note that the RGB color in the snippet above is not enclosed in brackets.
5. In your main Obsidian settings, go to `Appearance > CSS snippets` and enable your file. If you don't see it, click the reload icon and it should appear.

## Notes

Some UI features and community plugins may use the accent color as defined in your user settings (`Appearance > Accent color`), rather than the accent color of the theme. To avoid clashes, you might want to change the color in your settings to match the theme accent. If you find a color clash like this, [let me know](https://github.com/callumhackett/obsidian_polka_theme/issues) and I'll patch it. Using CSS snippets is strictly for dabblers and should not be required for a good user experience.
