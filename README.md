# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Preview](polka.png)

<a href="https://www.buymeacoffee.com/callumhackett" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## Color Customization

Due to the way the theme shares color values between elements for cohesion, Polka ignores the accent color in your Obsidian settings. You can still choose your own accent color, which will be applied in the ribbon and elsewhere, but you'll need to [create a CSS snippet](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) and override the `--accent-main` parameter with a raw RGB value. For example:

```
.theme-dark {
  --accent-main: 210, 65, 255 !important;
}
```

The above would cause the following changes to accents, among others (the callouts are thrown in for good measure):

![Customization](color_customization.png)

If customizing light mode, use `.theme-light` instead of `.theme-dark`.

## Fonts

The user is left to select which fonts are loaded via the main settings but Polka will use your default monospace font in table content, just in case your body font doesn't have tabular numbers (you can also override this with CSS by targeting the `--table-body-font` parameter).

The font used in the preview images here is Franklin Gothic, which you already have if you have Windows. If you want a good, free alternative, try [Rubik](https://fonts.google.com/specimen/Rubik).

## Plugin Support

In addition to modifying your workspace, Polka has color adaptations throughout Obsidian's user interface and the whole suite of core plugins.

Additionally, though code syntax colors use the built-in color scheme, the hues have been refined.

![Example](code_example.png)

Special attention has also been given to the following community plugins:

- [Calendar](https://github.com/liamcain/obsidian-calendar-plugin)
- [Dictionary](https://github.com/phibr0/obsidian-dictionary)
- [Execute Code](https://github.com/twibiral/obsidian-execute-code)
- [Kanban](https://github.com/mgmeyers/obsidian-kanban)

## Requests

Is there something you'd like to be changed or added? [Let me know](https://github.com/callumhackett/obsidian_polka_theme).
