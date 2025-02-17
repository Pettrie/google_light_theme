# minimal-animated-light-theme (by MiHme)

A Home Assistant (HA) theme inspired on Google app Light mode.
[Also inspired by Smart Home App - Animation](https://dribbble.com/shots/9828502-Smart-Home-App-Animation)

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)

## Screenshots

1. Desktop sample screenshot
![HA Desktop theme](https://link)

2. Mobile sample screenshot
![HA Mobile theme](https://link)

## Preparation

1. Make sure that under the **configuration.yaml** file you have the following:

```yaml
frontend:
  themes: !include_dir_merge_named ../themes
```

2. Under the Home Assistant **Config** folder, create a new folder named **themes**
3. **Restart** Home assistant to apply the changes.

## HACS installation

1. Go into the Community Store (HACS)
2. Search for `Minimal Animated White Theme` theme
3. Open the theme
4. Press Install
5. Restart Home Assistant

## Manual installation

1. In the Home assistant **themes** folder, create a file named `minimal_animated_white_theme.yaml`
2. In this GitHub repo, go into the **themes** folder, open the `minimal_animated_white_theme.yaml` file and copy the content
3. Paste the content in the `minimal_animated_white_theme.yaml` file created under your Home Assistant themes folder

## Enable theme

1. Open your Home Assistant open your **Profile**
2. Under, **Themes**, select the new `Minimal Animated White Theme`minimal_animated_white_theme

### Custom Header settings

When using the [Custom Header](https://github.com/maykar/custom-header) plugin, add the following into your `lovelace` file to make sure that the header matches the theme.

```yaml
custom_header:
  compact_mode: true
  background: var(--app-header-background-color)
  elements_color: var(--app-header-text-color)
  active_tab_color: var(--state-icon-active-color)
  tab_indicator_color: var(--state-icon-active-color)
```
