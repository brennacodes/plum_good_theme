# [VS Code Plum Good Theme](https://marketplace.visualstudio.com/items?itemName=brennacodes.plum-good-theme)

This theme was created with a focus of being easy on the eyes, while also being easy to read (and cool looking).

![Screenshot](/images/plum-good-theme.png)

## Install

Follow the instructions in the [marketplace](https://marketplace.visualstudio.com/items?itemName=brennacodes.plum-good-theme) or install directly from the editor:

Press `Ctrl+Shift+P` (or `Cmd+Shift+P`)   
Select `Extensions: Install Extensions`  
Search for `Plum Good`  

## Activate

With VS Code open:  
Press `Ctrl+Shift+P` (or `Cmd+Shift+P`) 
Select `Preferences: Color Theme`  
Select `Plum Good`.

## Enable additional darkness

Some features cannot be enabled automatically by a theme and must be configured manually in the user settings.

To access the user settings: Press `Ctrl+Shift+P` (or `Cmd+Shift+P`).
Select: `Preferences: Open Settings (JSON)`.  
Add this into the settings file:

```json5
{
  // Pitch black - Title bar (Allow the title bar to be styled by the color theme)
  "window.titleBarStyle": "custom",
  // Pitch plack - Hide border next to scroll bar that separates panes
  "editor.overviewRulerBorder": false,
}
```

## Optional settings - Configure some colors manually

If you like the theme as it is, the instructions below will not apply.

This color theme removes many lines and borders by default, if you want you can add them back:

```json5
{
  // Optional - Bring back some lines and borders
  "workbench.colorCustomizations": {
    "sideBar.border": "#222",
    "editorGroup.border": "#222",
    "editorIndentGuide.background": "#222", // Indent lines
    "editorIndentGuide.activeBackground": "#333", // Active indent line
  }
}
```

If you don't like the text selection and search highlight colors you can configure them:

```json5
{
  "workbench.colorCustomizations": {
    // Text selection
    "editor.selectionBackground": "#007acc",
    "editor.selectionHighlightBackground": "#007acc",
    "editor.inactiveSelectionBackground": "#007acc",
    // Find results
    "editor.findMatchBackground": "#fa05",
    "editor.findMatchHighlightBackground": "#fa05",
    "editor.findMatchBorder": "#fe0",
    "editor.findMatchHighlightBorder": "#fe0",
    "editor.selectionHighlightBorder": "#fe0",
  }
}
```

## Advanced: Manual Install: Useful for developing and testing the theme

```
cd ~/.vscode/extensions
git clone https://github.com/brennacodes/plum_master_p_theme 
```