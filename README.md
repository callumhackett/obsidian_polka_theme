# Polka

This theme adds some colorful minimalism to Obsidian in light and dark modes, with characteristic dots in the ribbon.

![Screenshot](polka.png)

## Customization

Due to the way the theme shares color values between elements for coherence, Polka overrides the **accent color** in Obsidian settings. If you want to choose your own color for the dots (and other elements which inherit the color), you need to [create your own CSS snippet](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) and override the `--accent-main` parameter with a raw RGB value. For example:

```
.theme-dark {
  --accent-main: 0, 255, 70 !important;
}
```

Replace `.theme-dark` with `.theme-light` if you are using light mode.

The user is left to determine which **font families** are loaded, although Polka sets table content to inherit your setup's chosen monospace family. The font used in the preview image is Franklin Gothic, which is available as standard on Windows. A good free alternative is Rubik.

## Extra Features

Polka comes with modifications to the default color settings of the **Kanban plugin**, so that it fits the overall palette better.
