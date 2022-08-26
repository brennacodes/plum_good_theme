# [VS Code Plum Good Theme](https://marketplace.visualstudio.com/items?itemName=brennacodes.plum-good-theme)

This theme was created with a focus of being easy on the eyes, while also being easy to read (and cool looking).

*Now with more plum goodness!!!*

Check out the Ruby Soho theme for a more gemtastic version of the Plum Good Theme. Simply install this extension, and then select the Ruby Soho theme from the theme picker.

![Screenshot](/images/plum-good-theme.png)
![Screenshot](/images/ruby-soho-theme.png)

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

## Optional settings - Configure colors manually

If you like the theme as it is, the instructions below won't apply.

This color theme removes many lines and borders by default, if you want you can add them back:

```json5
{
  // Optional - Bring back some lines and borders
  "workbench.colorCustomizations": {
    "sideBar.border": "#insert_hex_number_here",
    "editorGroup.border": "#insert_hex_number_here",
    "editorIndentGuide.background": "#insert_hex_number_here", // Indent lines
    "editorIndentGuide.activeBackground": "#insert_hex_number_here", // Active indent line
  }
}
```

If you don't like the text selection and search highlight colors you can configure them:

```json5
{
  "workbench.colorCustomizations": {
    // Text selection
    "editor.selectionBackground": "#insert_hex_number_here",
    "editor.selectionHighlightBackground": "#insert_hex_number_here",
    "editor.inactiveSelectionBackground": "#insert_hex_number_here",
    // Find results
    "editor.findMatchBackground": "#insert_hex_number_here",
    "editor.findMatchHighlightBackground": "#insert_hex_number_here",
    "editor.findMatchBorder": "#insert_hex_number_here",
    "editor.findMatchHighlightBorder": "#insert_hex_number_here",
    "editor.selectionHighlightBorder": "#insert_hex_number_here",
  }
}
```

## Advanced: Manual Install: Useful for developing and testing the theme

```
cd ~/.vscode/extensions
git clone https://github.com/brennacodes/plum_good_theme 
```