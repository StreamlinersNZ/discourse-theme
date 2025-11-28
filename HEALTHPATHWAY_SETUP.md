# HealthPathway Theme Setup Guide

This theme has been updated to work with Discourse's proper color scheme system. The HealthPathway color scheme is now defined in `about.json`.

## How to Apply the HealthPathway Theme

1. **Upload/Install the Theme**: Make sure this theme is installed in your Discourse instance.

2. **Select the HealthPathways Color Scheme**:
   - Go to **Admin** → **Customize** → **Themes**
   - Select your theme
   - In the **Colour Palette** dropdown, select **"HealthPathways"**
   - Save the theme settings

3. **Verify the Colors**:
   - The HealthPathways color scheme includes:
     - **Primary** (text/links): `#0B213B` (Navy)
     - **Secondary** (backgrounds): `#F8F5F0` (White)
     - **Tertiary** (accents): `#76ADE4` (Blue)
     - **Quaternary** (subtle backgrounds): `#E6E0DB` (Almond)

## Color Scheme Definition

The HealthPathway color scheme is defined in `about.json`:

```json
"color_schemes": {
  "HealthPathways": {
    "primary": "0b213b",
    "secondary": "f8f5f0",
    "tertiary": "76ade4",
    "quaternary": "e6e0db",
    "header_background": "f8f5f0",
    "header_primary": "0b213b",
    "highlight": "76ade4",
    "danger": "d04444",
    "success": "009900",
    "love": "fa6c8d"
  }
}
```

## Custom Theme Variables

The theme also defines custom CSS variables for HealthPathway-specific styling:
- `--redditish-bg-color`: Background color (uses HealthPathway White)
- `--redditish-border-color`: Border color (uses HealthPathway Almond)
- `--redditish-border-highlight-color`: Hover border color (uses HealthPathway Blue)
- `--box-shadow-default`: Default box shadow (Navy with opacity)
- `--box-shadow-hover`: Hover box shadow (Navy with opacity)

## Notes

- This theme is based on the upstream `discourse-redditish-theme`
- All colors use Discourse's standard color scheme system (no `!important` overrides)
- The theme will automatically use the selected color scheme's values
- If you need to customize colors further, edit the color scheme in Discourse admin or modify `about.json`

