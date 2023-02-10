# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Screenshot](polka.png)

## Color Customization

Due to the way the theme shares color values between elements for coherence, Polka ignores the accent color in your Obsidian settings. You can choose your own accent color for the dots (and other elements which inherit the color) but you'll need to [create your own CSS snippet](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) and override the `--accent-main` parameter with a raw RGB value. For example:

```
.theme-dark {
  --accent-main: 0, 255, 70 !important;
}
```

The selector `.theme-dark` is for dark mode. Use `.theme-light` with light mode.

## Fonts

The user is left to select which font families are loaded, although Polka is set up to make table content use whichever is your default monospace font. The font used in the preview image is Franklin Gothic, which is available as standard on Windows. A good free alternative is [Rubik](https://fonts.google.com/specimen/Rubik).

## Features

Polka keeps Obsidian's built-in color scheme for syntax highlighting in code blocks, though the colors have been refined for this theme.

Polka also comes with modifications to the default colors of the [Kanban plugin](https://github.com/mgmeyers/obsidian-kanban).
