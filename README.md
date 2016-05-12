# Setting up Sublime Text JavaScript Linting



## From user prefs

```
	"color_scheme": "Packages/User/SublimeLinter/Monokai Phoenix (SL).tmTheme",
	"match_brackets_angle": true,
```

## Plugins

 - [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)
 - [Sublime​Linter-contrib-eslint](https://packagecontrol.io/packages/SublimeLinter-contrib-eslint)
 - [ESLint-Formatter](https://packagecontrol.io/packages/ESLint-Formatter)


## Sublime Linter Settings

### Installing
[Installing SublimeLinter](http://sublimelinter.readthedocs.io/en/latest/installation.html)

### Settings

For general information on how SublimeLinter works with settings, please see [Settings][settings]. For information on generic linter settings, please see [Linter Settings][linter-settings].


My [SublimeLinter.sublime-settings](./sublime-settings-files/SublimeLinter.sublime-settings)

Default Mac OS X path: `~/Library/Application Support/Sublime Text 3/Packages/User/SublimeLinter.sublime-settings`

To edit yours:

![Alt text](./images/sublime-lint-prefs--sublime-linter-prefs-mousing.png "Sublime Text Linting: Mousing to the Sublime Linter Preferences")



## Sublime Linter Contrib ESLint Settings

### Installing

To install via Package Control, do the following:

1. Within Sublime Text, bring up the [Command Palette][cmd] and type `install`. Among the commands you should see `Package Control: Install Package`. If that command is not highlighted, use the keyboard or mouse to select it. There will be a pause of a few seconds while Package Control fetches the list of available plugins.

1. When the plugin list appears, type `eslint`. Among the entries you should see `SublimeLinter-contrib-eslint`. If that entry is not highlighted, use the keyboard or mouse to select it.

### Settings

My [SublimeLinter.sublime-settings](./sublime-settings-files/SublimeLinter.sublime-settings)

Default Mac OS X path: `~/Library/Application Support/Sublime Text 3/Packages/User/SublimeLinter.sublime-settings`

To edit yours:

![Alt text](./images/sublime-lint-prefs--sublime-linter-prefs-mousing.png "Sublime Text Linting: Mousing to the Sublime Linter Preferences")



## ESLint Formatter Sublime Settings

[ESLint-Formatter.sublime-settings](./sublime-settings-files/ESLint-Formatter.sublime-settings)

Default Mac OS X path: `~/Library/Application Support/Sublime Text 3/Packages/User/ESLint-Formatter.sublime-settings`

**Note this bit from that file:**

```
	// Specify this path to an eslint config file to override the default behavior.
	// Passed to eslint as --config. Read more here:
	// http://eslint.org/docs/user-guide/command-line-interface#c---config
	"config_path": "/Users/ccorwin/Documents/Workspaces/design-system-react-app-boilerplate/node_modules/eslint-config-slds/index.js",
```

Once I pointed it directly to the `eslint-config-slds/index.js` file, it started using the settings correctly. No other amount of voodoo or incantations seemed to work.


To edit yours:

![Alt text](./images/sublime-lint-prefs--eslint-formatter-prefs-mousing.png "Sublime Text Linting: Mousing to the ESLint Formatter Preferences")

Note that the only way I've gotten it to find my local eslint is to set it for a specific project in the formatters "global" file. :( This is annoying, but it works.






From `~/Documents/Workspaces/design-system-react-app-boilerplate/.eslintrc`


[cmd]: http://docs.sublimetext.info/en/sublime-text-3/extensibility/command_palette.html
[settings]: http://sublimelinter.readthedocs.org/en/latest/settings.html
[linter-settings]: http://sublimelinter.readthedocs.org/en/latest/linter_settings.html
