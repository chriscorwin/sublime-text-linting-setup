# Setting up Sublime Text JavaScript Linting



## From user prefs

```
	"color_scheme": "Packages/User/SublimeLinter/Monokai Phoenix (SL).tmTheme",
	"match_brackets_angle": true,
```

## Plugins

 - [Sublime Linter](http://sublimelinter.readthedocs.org)
 - [Sublime Linter Contrib: ESLint](https://github.com/roadhump/SublimeLinter-eslint)

## Sublime Linter Settings

[SublimeLinter.sublime-settings](./sublime-settings-files/SublimeLinter.sublime-settings)

Default Mac OS X path: `~/Library/Application Support/Sublime Text 3/Packages/User/SublimeLinter.sublime-settings`

To edit yours:

![Alt text](./images/sublime-lint-prefs--sublime-linter-prefs-mousing.png "Sublime Text Linting: Mousing to the Sublime Linter Preferences")



## ESLint Formatter Sublime Settings

[ESLint-Formatter.sublime-settings](./sublime-settings-files/ESLint-Formatter.sublime-settings)

Default Mac OS X path: `~/Library/Application Support/Sublime Text 3/Packages/User/ESLint-Formatter.sublime-settings`

To edit yours:

![Alt text](./images/sublime-lint-prefs--eslint-formatter-prefs-mousing.png "Sublime Text Linting: Mousing to the ESLint Formatter Preferences")

Note that the only way I've gotten it to find my local eslint is to set it for a specific project in the formatters "global" file. :( This is annoying, but it works.




From `~/Documents/Workspaces/design-system-react-app-boilerplate/.eslintrc`
