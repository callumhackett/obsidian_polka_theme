# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Preview](polka_full_size.png)

<a href="https://www.buymeacoffee.com/callumhackett" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Color Customization

As of v1.2, Polka responds to the accent color in your main settings (under `Appearance > Accent color`), which it will use for the dots in the ribbon, text accents and much else besides. For example, if you choose a pink accent color while in dark mode, the default cyan accent will be replaced in all the ways you can see below (and more):

![Customization](color_customization.png)

You can also change the main background color, although to do this you'll need to create a CSS snippet and play around with some HSL values (scroll to the bottom for help on setting this up—it's actually quite easy!). Here's an example of a different background tone achieved by changing just one number (much more fine-tuning is possible):

![Backgrounds](background_customization.png)

## Fonts

Font taste is personal. Polka selects nice default fonts for Mac and PC but your main font settings (`Appearance > Font`) will override these.

The font in the preview images is Franklin Gothic, which is distributed with Windows. If you want a good, free alternative, try [Rubik](https://fonts.google.com/specimen/Rubik). If you're looking for a code font, my preference (for what it's worth) is [iA Writer Mono](https://github.com/iaolo/iA-Fonts/tree/master/iA%20Writer%20Mono), which is a variant of [IBM Plex Mono](https://github.com/IBM/plex) with some small character adjustments.

## Plugin Support

As well as modifying your workspace, Polka adapts the colors of Obsidian's user interface and the whole suite of core plugins. Additionally, though code syntax colors use the built-in color scheme, the hues have been refined.

Special attention has been given to the following community plugins:

- [Calendar](https://github.com/liamcain/obsidian-calendar-plugin)
- [Dictionary](https://github.com/phibr0/obsidian-dictionary)
- [Execute Code](https://github.com/twibiral/obsidian-execute-code)
- [Kanban](https://github.com/mgmeyers/obsidian-kanban)

Many others will fit in without issue but [tell me](https://github.com/callumhackett/obsidian_polka_theme/issues) if I should support something else.

## CSS Snippets

To set your own accent color:

1. In a file explorer (not Obsidian), go to your main vault folder.
2. From there, go to the `/.obsidian/snippets` folder and create a `.css` file with any name.
3. Copy and paste the code below into your CSS file:
```
.theme-dark {
  --accent-main: 225, 120, 255 !important;
}
```
4. Replace the numbers with those of your preferred RGB color and, if you want to customize light mode, replace `.theme-dark` with `.theme-light` (if you're familiar with CSS, note that the color value is not enclosed in brackets).
5. In your main Obsidian settings, go to `Appearance > CSS snippets` and enable your file. If you don't see it, click the reload icon and it should appear.

## Notes

Some UI features and community plugins may use the accent color as defined in your user settings (`Appearance > Accent color`), rather than the accent color of the theme. To avoid clashes, you might want to change the color in your settings to match the theme accent. If you see a clash, [let me know](https://github.com/callumhackett/obsidian_polka_theme/issues) and I'll patch it; this will help keep CSS snippets unnecessary for those who are happy with the default settings.
