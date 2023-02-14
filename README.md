# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Preview](polka_full_size.png)

<a href="https://www.buymeacoffee.com/callumhackett" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Color Customization

Due to the way the theme shares color values between elements for cohesion, Polka ignores the accent color in your Obsidian settings. You can still choose your own accent color, which will be applied in the ribbon and elsewhere, but you'll need to [create a CSS snippet](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) and override the `--accent-main` parameter with a raw RGB value. For example:

```
.theme-dark {
  --accent-main: 225, 120, 255 !important;
}
```

If you compare with the main theme preview, you can see some of the effects that the above snippet would have in the preview below:

![Customization](color_customization.png)

If customizing light mode, use the selector `.theme-light` instead of `.theme-dark`.

Note that some UI features and community plugins may use the accent color as defined in your user settings (Appearance > Accent color), so if you change the theme accent with a CSS snippet, it's recommended that you use the same value in your user settings.

## Fonts

The user is left to select which fonts are loaded via the main settings. The font used in the preview images here is Franklin Gothic, which you already have if you have Windows. If you want a good, free alternative, try [Rubik](https://fonts.google.com/specimen/Rubik).

## Plugin Support

As well as modifying your workspace, Polka has color adaptations for Obsidian's user interface and the whole suite of core plugins. Additionally, though code syntax colors use the built-in color scheme, the hues have been refined.

Special attention has been given to the following community plugins (many others will fit in without issue):

- [Calendar](https://github.com/liamcain/obsidian-calendar-plugin)
- [Dictionary](https://github.com/phibr0/obsidian-dictionary)
- [Execute Code](https://github.com/twibiral/obsidian-execute-code)
- [Kanban](https://github.com/mgmeyers/obsidian-kanban)

## Requests

Is there something you'd like to be changed or added? [Let me know](https://github.com/callumhackett/obsidian_polka_theme).
