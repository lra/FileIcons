# FileIcons
Colored file icons for Sublime Text.

Adds specific, colored icons for most file types for the sidebar in Sublime Text 3. Supports both the Default and Adaptive themes.

Inspired by [A File Icon](https://packagecontrol.io/packages/A%20File%20Icon), but simpler:

- Doesn't introduce "alias" languages like "Javascript (Gulpfile)"
- No runtime code: no manipulation of settings or themes, no restarting
- No configuration: just uses existing theme override behavior

## Customize

The following changes are made to Adaptive/Default.sublime-theme. You can override them by creating a theme file with the same name in your Packages/User directory.

```json
[
  {
    "class": "icon_file_type",
    "layer0.tint": [255, 255, 255],
    "layer0.opacity": 0.75,
    "content_margin": [8, 8]
  },
  {
    "class": "icon_file_type",
    "parents": [{"class": "tree_row", "attributes": ["hover"]}],
    "layer0.opacity": 0.5
  },
  {
    "class": "icon_file_type",
    "parents": [{"class": "tree_row", "attributes": ["selected"]}],
    "layer0.opacity": 1.0
  }
]
```