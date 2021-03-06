# Glot (sublime plugin)

Put/run your code on https://glot.io.

**Requires an api token to work**.
Get your own token at https://glot.io/account/token and put it in settings.

![preview](https://user-images.githubusercontent.com/8097890/51736121-3ec09c80-20c4-11e9-8cb9-9a51a2313e9a.gif)

## Install

### From Package Control

Press <kbd>Ctrl+Shift+P</kbd>, Select `Package Control: Install Package`,
Search for `Glot`, <kbd>Return</kbd>.

### From this repo

Press <kbd>Ctrl+Shift+P</kbd>, Select `Package Control: Add Repository`, Input `https://github.com/hyrious/Glot`, <kbd>Return</kbd>.

Or, in your plugins folder, run `git clone https://github.com/hyrious/Glot`. This way you will not get auto-upgrade provided by Package Control.

## Key Bindings

I haven't got any ideas of using what key bindings, you can add your own by
`Preference - Key Bindings` then add things like:

```json
{ "keys": ["ctrl+k", "ctrl+g"], "command": "glot_run" },
```

Valid commands are: `glot_new_snippet`, `glot_open_snippet`,
`glot_update_snippet`, `glot_delete_snippet`, `glot_run`, `glot_advanced_run`.

## Usage

All messages are displayed at your status bar.

### Create Snippet

<kbd>Ctrl+Shift+P</kbd>, then select `Glot: New Snippet`.
If everything ok, it will ask you for a snippet title.

### Open Snippet

<kbd>Ctrl+Shift+P</kbd>, then select `Glot: Open Snippet`.

### Update Snippet

After open a snippet from previous command, just <kbd>Ctrl+S</kbd> or
<kbd>Ctrl+Shift+P</kbd> then select `Glot: Update Snippet`.

### Delete Snippet

<kbd>Ctrl+Shift+P</kbd>, then select `Glot: Delete Snippet`.

### Run Code

<kbd>Ctrl+Shift+P</kbd>, then select `Glot: Run` or `Glot: Advanced Run`.
Temporary files should work, but may encounter language specific errors.
e.g. Java requires file name must be the same as class name.

## License

MIT.
