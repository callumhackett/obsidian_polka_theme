# Polka

This customizable theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Preview](polka_full_size.png)

<a href="https://www.buymeacoffee.com/callumhackett" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Color Customization

As of v1.2, Polka responds to the accent color in your main settings (under `Appearance > Accent color`), which it will use for links, highlights, the dots in the ribbon and much else besides. For example, if you choose a pink accent color while in dark mode, the default cyan will be replaced in all the ways you can see below (and more):

![Customization](color_customization.png)

It's also straightforward to change the background color palette, although you'll need to create a CSS snippet (scroll to the bottom for step-by-step instructions—it's quite easy!). Here's an example of how you can change the tone with just one number and still retain cohesion across the entire interface:

![Backgrounds](background_customization.png)

## Fonts

Font taste is personal. Polka selects nice default fonts for Mac and PC but your main font settings (under `Appearance > Font`) will override these.

The font in the preview images here is Franklin Gothic, which is distributed with Windows. If you want a good, free alternative, try [Rubik](https://fonts.google.com/specimen/Rubik). If you're looking for a code font, my own preference is [iA Writer Mono](https://github.com/iaolo/iA-Fonts/tree/master/iA%20Writer%20Mono), which is a variant of [IBM Plex](https://github.com/IBM/plex) with some small character adjustments.

## Plugin Support

As well as modifying your workspace, Polka adapts the colors of Obsidian's user interface and the whole suite of core plugins. Additionally, code syntax highlighting uses the built-in color scheme but the hues have been refined.

Special attention has been given to the following community plugins:

- [Calendar](https://github.com/liamcain/obsidian-calendar-plugin)
- [Dictionary](https://github.com/phibr0/obsidian-dictionary)
- [Execute Code](https://github.com/twibiral/obsidian-execute-code)
- [Kanban](https://github.com/mgmeyers/obsidian-kanban)

Many others will fit in without issue but [let me know](https://github.com/callumhackett/obsidian_polka_theme/issues) if you think I should support something else.

## CSS Snippets

To set your own background colors (or to make other visual adjustments):

1. In a file explorer (not Obsidian), go to your main vault folder.
2. From there, go to the `/.obsidian/snippets` folder and create a `.css` file with any name.
3. Copy and paste the code below into your CSS file, replacing `.theme-dark` with `.theme-light` if you want to customize light mode:
```
.theme-dark {
  --background-h: 180;
  --background-s: 50%;
  --background-l: 25%;
}
```
4. Change the numbers to dial in your own color: `--background-h` ranges from 0-360 and represents a hue, such as red or blue; `--background-s` ranges from 0-100% and is your color's saturation; `--background-l` ranges from 0-100% and is your color's lightness. The color you choose applies directly to the background of the text editor but other colors in the theme are derived from it. You may find it easiest to use an independent HSL color picker.
5. In your main Obsidian settings, go to `Appearance > CSS snippets` and enable your file. If you don't see it, click the reload icon and it should appear.
